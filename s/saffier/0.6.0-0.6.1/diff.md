# Comparing `tmp/saffier-0.6.0.tar.gz` & `tmp/saffier-0.6.1.tar.gz`

## Comparing `saffier-0.6.0.tar` & `saffier-0.6.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/__init__.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/exceptions.py
--rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/fields.py
--rw-r--r--   0        0        0    12230 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/metaclass.py
--rw-r--r--   0        0        0     7411 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/models.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/py.typed
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/testclient.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/core/__init__.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/core/base.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/core/datastructures.py
--rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/core/formats.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/core/registry.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/core/schemas.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/core/unique.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/core/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/db/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/db/connection.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/db/constants.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/db/datastructures.py
--rw-r--r--   0        0        0    15804 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/db/fields.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/db/manager.py
--rw-r--r--   0        0        0    23137 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/db/queryset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/db/query/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/db/query/protocols.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/__init__.py
--rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/base.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/cli.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/constants.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/decorators.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/env.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/__init__.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/branches.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/check.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/current.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/downgrade.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/edit.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/heads.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/history.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/init.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/list_templates.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/makemigrations.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/merge.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/migrate.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/revision.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/show.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/operations/stamp.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/templates/default/README
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/templates/default/alembic.ini.mako
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/templates/default/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/migrations/templates/default/script.py.mako
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/sqlalchemy/fields.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/sqlalchemy/protocols.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.6.0/saffier/sqlalchemy/types.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.6.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.6.0/LICENSE
--rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.6.0/README.md
--rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 saffier-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    10972 2020-02-02 00:00:00.000000 saffier-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/__init__.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/exceptions.py
+-rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/fields.py
+-rw-r--r--   0        0        0    12230 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/metaclass.py
+-rw-r--r--   0        0        0     7411 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/models.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/py.typed
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/testclient.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/__init__.py
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/base.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/datastructures.py
+-rw-r--r--   0        0        0     6366 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/formats.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/registry.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/schemas.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/unique.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/core/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/__init__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/connection.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/constants.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/datastructures.py
+-rw-r--r--   0        0        0    15804 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/fields.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/manager.py
+-rw-r--r--   0        0        0    23137 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/queryset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/query/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/db/query/protocols.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/__init__.py
+-rw-r--r--   0        0        0    11109 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/base.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/cli.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/constants.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/decorators.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/env.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/__init__.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/branches.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/check.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/current.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/downgrade.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/edit.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/heads.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/history.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/init.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/list_templates.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/makemigrations.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/merge.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/migrate.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/revision.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/show.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/operations/stamp.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/templates/default/README
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/templates/default/alembic.ini.mako
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/templates/default/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/migrations/templates/default/script.py.mako
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/sqlalchemy/fields.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/sqlalchemy/protocols.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 saffier-0.6.1/saffier/sqlalchemy/types.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 saffier-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 saffier-0.6.1/LICENSE
+-rw-r--r--   0        0        0     6706 2020-02-02 00:00:00.000000 saffier-0.6.1/README.md
+-rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 saffier-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    10972 2020-02-02 00:00:00.000000 saffier-0.6.1/PKG-INFO
```

### Comparing `saffier-0.6.0/saffier/__init__.py` & `saffier-0.6.1/saffier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 from .core.registry import Registry
 from .db.connection import Database
 from .db.constants import CASCADE, RESTRICT, SET_NULL
 from .db.datastructures import Index, UniqueConstraint
 from .db.manager import Manager
 from .db.queryset import QuerySet
```

### Comparing `saffier-0.6.0/saffier/exceptions.py` & `saffier-0.6.1/saffier/exceptions.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/fields.py` & `saffier-0.6.1/saffier/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Decimal,
     Email,
     Float,
     Integer,
 )
 from saffier.db.fields import IPAddress as CoreIPAddress
 from saffier.db.fields import Password, SaffierField, String, Time
-from saffier.sqlalchemy.fields import GUID, IPAddress
+from saffier.sqlalchemy.fields import IPAddress
 
 
 class Field:
     """
     Base field for the model declaration fields.
     """
 
@@ -343,16 +343,16 @@
     """
     Representation of UUID
     """
 
     def get_validator(self, **kwargs: typing.Any) -> SaffierField:
         return UUID(**kwargs)
 
-    def get_column_type(self) -> GUID:
-        return GUID()
+    def get_column_type(self) -> sqlalchemy.UUID:
+        return sqlalchemy.UUID()
 
 
 class PasswordField(CharField):
     """
     Representation of a Password
     """
```

### Comparing `saffier-0.6.0/saffier/metaclass.py` & `saffier-0.6.1/saffier/metaclass.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/models.py` & `saffier-0.6.1/saffier/models.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/core/base.py` & `saffier-0.6.1/saffier/core/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/core/datastructures.py` & `saffier-0.6.1/saffier/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/core/formats.py` & `saffier-0.6.1/saffier/core/formats.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/core/registry.py` & `saffier-0.6.1/saffier/core/registry.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/core/schemas.py` & `saffier-0.6.1/saffier/core/schemas.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/core/unique.py` & `saffier-0.6.1/saffier/core/unique.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/core/utils.py` & `saffier-0.6.1/saffier/core/utils.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/db/datastructures.py` & `saffier-0.6.1/saffier/db/datastructures.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/db/fields.py` & `saffier-0.6.1/saffier/db/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/db/manager.py` & `saffier-0.6.1/saffier/db/manager.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/db/queryset.py` & `saffier-0.6.1/saffier/db/queryset.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/db/query/protocols.py` & `saffier-0.6.1/saffier/db/query/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/base.py` & `saffier-0.6.1/saffier/migrations/base.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/cli.py` & `saffier-0.6.1/saffier/migrations/cli.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/env.py` & `saffier-0.6.1/saffier/migrations/env.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/operations/__init__.py` & `saffier-0.6.1/saffier/migrations/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/operations/branches.py` & `saffier-0.6.1/saffier/migrations/operations/branches.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/operations/current.py` & `saffier-0.6.1/saffier/migrations/operations/current.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/operations/downgrade.py` & `saffier-0.6.1/saffier/migrations/operations/downgrade.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/operations/heads.py` & `saffier-0.6.1/saffier/migrations/operations/heads.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/operations/history.py` & `saffier-0.6.1/saffier/migrations/operations/history.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/operations/init.py` & `saffier-0.6.1/saffier/migrations/operations/init.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/operations/makemigrations.py` & `saffier-0.6.1/saffier/migrations/operations/makemigrations.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/operations/merge.py` & `saffier-0.6.1/saffier/migrations/operations/merge.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/operations/migrate.py` & `saffier-0.6.1/saffier/migrations/operations/migrate.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/operations/revision.py` & `saffier-0.6.1/saffier/migrations/operations/revision.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/operations/show.py` & `saffier-0.6.1/saffier/migrations/operations/show.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/operations/stamp.py` & `saffier-0.6.1/saffier/migrations/operations/stamp.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/templates/default/alembic.ini.mako` & `saffier-0.6.1/saffier/migrations/templates/default/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/migrations/templates/default/env.py` & `saffier-0.6.1/saffier/migrations/templates/default/env.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/sqlalchemy/fields.py` & `saffier-0.6.1/saffier/sqlalchemy/fields.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/saffier/sqlalchemy/protocols.py` & `saffier-0.6.1/saffier/sqlalchemy/protocols.py`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/LICENSE` & `saffier-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/README.md` & `saffier-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/pyproject.toml` & `saffier-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `saffier-0.6.0/PKG-INFO` & `saffier-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saffier
-Version: 0.6.0
+Version: 0.6.1
 Summary: The only python ORM you will ever need.
 Project-URL: Homepage, https://github.com/tarsil/saffier
 Project-URL: Documentation, https://saffier.tarsild.io/
 Project-URL: Changelog, https://saffier.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/saffier
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
```

