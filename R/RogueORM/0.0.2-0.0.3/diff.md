# Comparing `tmp/RogueORM-0.0.2.tar.gz` & `tmp/RogueORM-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RogueORM-0.0.2.tar", last modified: Mon Apr 10 17:02:40 2023, max compression
+gzip compressed data, was "RogueORM-0.0.3.tar", last modified: Mon Apr 10 23:21:59 2023, max compression
```

## Comparing `RogueORM-0.0.2.tar` & `RogueORM-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.297160 RogueORM-0.0.2/
--rw-rw-rw-   0        0        0     1093 2022-12-06 23:54:36.000000 RogueORM-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     3835 2023-04-10 17:02:40.296186 RogueORM-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2053 2023-04-10 16:30:27.000000 RogueORM-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.279016 RogueORM-0.0.2/RogueORM.egg-info/
--rw-rw-rw-   0        0        0     3835 2023-04-10 17:02:40.000000 RogueORM-0.0.2/RogueORM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-10 17:02:40.000000 RogueORM-0.0.2/RogueORM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 17:02:40.000000 RogueORM-0.0.2/RogueORM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-10 17:02:40.000000 RogueORM-0.0.2/RogueORM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-10 17:02:40.000000 RogueORM-0.0.2/RogueORM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1185 2023-04-10 17:00:56.000000 RogueORM-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.280965 RogueORM-0.0.2/rogue/
--rw-rw-rw-   0        0        0        0 2022-12-07 00:00:53.000000 RogueORM-0.0.2/rogue/__init__.py
--rw-rw-rw-   0        0        0      484 2023-04-10 16:29:25.000000 RogueORM-0.0.2/rogue/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.283896 RogueORM-0.0.2/rogue/backends/
--rw-rw-rw-   0        0        0        0 2022-12-09 00:39:38.000000 RogueORM-0.0.2/rogue/backends/__init__.py
--rw-rw-rw-   0        0        0     4367 2023-04-10 16:29:28.000000 RogueORM-0.0.2/rogue/backends/base.py
--rw-rw-rw-   0        0        0      155 2022-12-21 23:27:34.000000 RogueORM-0.0.2/rogue/backends/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.286860 RogueORM-0.0.2/rogue/backends/sqlite/
--rw-rw-rw-   0        0        0        0 2022-12-09 00:40:15.000000 RogueORM-0.0.2/rogue/backends/sqlite/__init__.py
--rw-rw-rw-   0        0        0      601 2022-12-23 18:49:28.000000 RogueORM-0.0.2/rogue/backends/sqlite/client.py
--rw-rw-rw-   0        0        0     2704 2023-01-05 21:20:18.000000 RogueORM-0.0.2/rogue/backends/sqlite/query.py
--rw-rw-rw-   0        0        0     1114 2023-04-10 16:29:28.000000 RogueORM-0.0.2/rogue/backends/sqlite/schema.py
--rw-rw-rw-   0        0        0       45 2022-12-21 18:46:55.000000 RogueORM-0.0.2/rogue/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.289789 RogueORM-0.0.2/rogue/managers/
--rw-rw-rw-   0        0        0      128 2023-01-05 21:19:29.000000 RogueORM-0.0.2/rogue/managers/__init__.py
--rw-rw-rw-   0        0        0     5853 2023-01-05 21:20:21.000000 RogueORM-0.0.2/rogue/managers/base.py
--rw-rw-rw-   0        0        0      152 2022-12-21 18:47:09.000000 RogueORM-0.0.2/rogue/managers/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.290766 RogueORM-0.0.2/rogue/migrations/
--rw-rw-rw-   0        0        0       66 2023-04-10 16:29:25.000000 RogueORM-0.0.2/rogue/migrations/__init__.py
--rw-rw-rw-   0        0        0      952 2023-04-10 16:38:02.000000 RogueORM-0.0.2/rogue/migrations/base.py
-drwxrwxrwx   0        0        0        0 2023-04-10 17:02:40.295201 RogueORM-0.0.2/rogue/models/
--rw-rw-rw-   0        0        0       84 2022-12-18 20:54:58.000000 RogueORM-0.0.2/rogue/models/__init__.py
--rw-rw-rw-   0        0        0     7540 2023-01-05 21:23:17.000000 RogueORM-0.0.2/rogue/models/base.py
--rw-rw-rw-   0        0        0      332 2022-12-21 23:59:31.000000 RogueORM-0.0.2/rogue/models/errors.py
--rw-rw-rw-   0        0        0     8001 2023-01-05 21:19:29.000000 RogueORM-0.0.2/rogue/models/fields.py
--rw-rw-rw-   0        0        0     1118 2022-12-23 19:43:17.000000 RogueORM-0.0.2/rogue/models/utils.py
--rw-rw-rw-   0        0        0       42 2023-04-10 17:02:40.297160 RogueORM-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.557810 RogueORM-0.0.3/
+-rw-rw-rw-   0        0        0     1093 2022-12-06 23:54:36.000000 RogueORM-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3853 2023-04-10 23:21:59.557810 RogueORM-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2071 2023-04-10 23:07:27.000000 RogueORM-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.537101 RogueORM-0.0.3/RogueORM.egg-info/
+-rw-rw-rw-   0        0        0     3853 2023-04-10 23:21:59.000000 RogueORM-0.0.3/RogueORM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      752 2023-04-10 23:21:59.000000 RogueORM-0.0.3/RogueORM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 23:21:59.000000 RogueORM-0.0.3/RogueORM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-10 23:21:59.000000 RogueORM-0.0.3/RogueORM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-10 23:21:59.000000 RogueORM-0.0.3/RogueORM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1212 2023-04-10 23:21:29.000000 RogueORM-0.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.539062 RogueORM-0.0.3/rogue/
+-rw-rw-rw-   0        0        0        0 2022-12-07 00:00:53.000000 RogueORM-0.0.3/rogue/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-04-10 23:07:27.000000 RogueORM-0.0.3/rogue/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.541991 RogueORM-0.0.3/rogue/backends/
+-rw-rw-rw-   0        0        0        0 2022-12-09 00:39:38.000000 RogueORM-0.0.3/rogue/backends/__init__.py
+-rw-rw-rw-   0        0        0     4665 2023-04-10 23:21:08.000000 RogueORM-0.0.3/rogue/backends/base.py
+-rw-rw-rw-   0        0        0      155 2022-12-21 23:27:34.000000 RogueORM-0.0.3/rogue/backends/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.545971 RogueORM-0.0.3/rogue/backends/sqlite/
+-rw-rw-rw-   0        0        0        0 2022-12-09 00:40:15.000000 RogueORM-0.0.3/rogue/backends/sqlite/__init__.py
+-rw-rw-rw-   0        0        0      640 2023-04-10 19:11:29.000000 RogueORM-0.0.3/rogue/backends/sqlite/client.py
+-rw-rw-rw-   0        0        0     2704 2023-01-05 21:20:18.000000 RogueORM-0.0.3/rogue/backends/sqlite/query.py
+-rw-rw-rw-   0        0        0     4277 2023-04-10 23:07:27.000000 RogueORM-0.0.3/rogue/backends/sqlite/schema.py
+-rw-rw-rw-   0        0        0       45 2022-12-21 18:46:55.000000 RogueORM-0.0.3/rogue/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.547925 RogueORM-0.0.3/rogue/managers/
+-rw-rw-rw-   0        0        0      128 2023-01-05 21:19:29.000000 RogueORM-0.0.3/rogue/managers/__init__.py
+-rw-rw-rw-   0        0        0     5853 2023-01-05 21:20:21.000000 RogueORM-0.0.3/rogue/managers/base.py
+-rw-rw-rw-   0        0        0      152 2022-12-21 18:47:09.000000 RogueORM-0.0.3/rogue/managers/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.550855 RogueORM-0.0.3/rogue/migrations/
+-rw-rw-rw-   0        0        0       86 2023-04-10 23:07:27.000000 RogueORM-0.0.3/rogue/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4450 2023-04-10 23:07:27.000000 RogueORM-0.0.3/rogue/migrations/base.py
+drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.554873 RogueORM-0.0.3/rogue/models/
+-rw-rw-rw-   0        0        0       84 2022-12-18 20:54:58.000000 RogueORM-0.0.3/rogue/models/__init__.py
+-rw-rw-rw-   0        0        0     7583 2023-04-10 19:23:26.000000 RogueORM-0.0.3/rogue/models/base.py
+-rw-rw-rw-   0        0        0      332 2022-12-21 23:59:31.000000 RogueORM-0.0.3/rogue/models/errors.py
+-rw-rw-rw-   0        0        0     8001 2023-04-10 19:33:23.000000 RogueORM-0.0.3/rogue/models/fields.py
+-rw-rw-rw-   0        0        0     1920 2023-04-10 19:11:29.000000 RogueORM-0.0.3/rogue/models/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 23:21:59.556832 RogueORM-0.0.3/rogue/settings/
+-rw-rw-rw-   0        0        0     1117 2023-04-10 19:11:29.000000 RogueORM-0.0.3/rogue/settings/__init__.py
+-rw-rw-rw-   0        0        0       90 2023-04-10 19:11:29.000000 RogueORM-0.0.3/rogue/settings/default_settings.py
+-rw-rw-rw-   0        0        0       42 2023-04-10 23:21:59.558789 RogueORM-0.0.3/setup.cfg
```

### Comparing `RogueORM-0.0.2/LICENSE` & `RogueORM-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `RogueORM-0.0.2/PKG-INFO` & `RogueORM-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RogueORM
-Version: 0.0.2
+Version: 0.0.3
 Summary: An ORM that strives to eradicate N+1 issues.
 Author-email: Maxime Toussaint <m.toussaint@mail.com>
 License: MIT License
         
         Copyright (c) 2022 Maxime Toussaint
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,15 +47,15 @@
 
 ## Development Roadmap
  1. Define a clear syntax taking advantage of Python 3.10 and later's typing syntax. Status: Done
  2. Define models, managers and fields. Status: Done
  3. Add support for basic SQLite operation: SELECT, INSERT, UPDATE, DELETE. Status: Done
  4. Add support for Foreign Keys. Status: Done
  5. Add support for ManyToMany relationships using a joining table. Status: Done (Testing has to be improved)
- 6. Add a migration system. Status: Started, PR #11
+ 6. Add a migration system. Status: Done (Testing has to be improved)
  7. Add support for relation lookup using a similar method to Django's, with __ being put between field names. Status: Not started
  8. Add support for JOIN, UNION and GROUP BY, with an interface to build them. Status: Not started
  9. Add logic for batch fetching in loops. Status: Not started
  10. Add logic for select_related. By design, prefetch_related will never be part of this ORM, preferring a 'fetch in batch when needed' approach. Status: Not started
  11. Look into supporting up to Python 3.7 by taking into account the possible usage of *Union* and *Optional* Maybe import from future? Status: Not started
  12. Improve testing by adding a way to catch queries made to the database, to make sure we lower them as much as possible. Status: Not started
  13. Add support for postgresql. Status: Not started
```

### Comparing `RogueORM-0.0.2/README.md` & `RogueORM-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ## Development Roadmap
  1. Define a clear syntax taking advantage of Python 3.10 and later's typing syntax. Status: Done
  2. Define models, managers and fields. Status: Done
  3. Add support for basic SQLite operation: SELECT, INSERT, UPDATE, DELETE. Status: Done
  4. Add support for Foreign Keys. Status: Done
  5. Add support for ManyToMany relationships using a joining table. Status: Done (Testing has to be improved)
- 6. Add a migration system. Status: Started, PR #11
+ 6. Add a migration system. Status: Done (Testing has to be improved)
  7. Add support for relation lookup using a similar method to Django's, with __ being put between field names. Status: Not started
  8. Add support for JOIN, UNION and GROUP BY, with an interface to build them. Status: Not started
  9. Add logic for batch fetching in loops. Status: Not started
  10. Add logic for select_related. By design, prefetch_related will never be part of this ORM, preferring a 'fetch in batch when needed' approach. Status: Not started
  11. Look into supporting up to Python 3.7 by taking into account the possible usage of *Union* and *Optional* Maybe import from future? Status: Not started
  12. Improve testing by adding a way to catch queries made to the database, to make sure we lower them as much as possible. Status: Not started
  13. Add support for postgresql. Status: Not started
```

### Comparing `RogueORM-0.0.2/RogueORM.egg-info/PKG-INFO` & `RogueORM-0.0.3/RogueORM.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RogueORM
-Version: 0.0.2
+Version: 0.0.3
 Summary: An ORM that strives to eradicate N+1 issues.
 Author-email: Maxime Toussaint <m.toussaint@mail.com>
 License: MIT License
         
         Copyright (c) 2022 Maxime Toussaint
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,15 +47,15 @@
 
 ## Development Roadmap
  1. Define a clear syntax taking advantage of Python 3.10 and later's typing syntax. Status: Done
  2. Define models, managers and fields. Status: Done
  3. Add support for basic SQLite operation: SELECT, INSERT, UPDATE, DELETE. Status: Done
  4. Add support for Foreign Keys. Status: Done
  5. Add support for ManyToMany relationships using a joining table. Status: Done (Testing has to be improved)
- 6. Add a migration system. Status: Started, PR #11
+ 6. Add a migration system. Status: Done (Testing has to be improved)
  7. Add support for relation lookup using a similar method to Django's, with __ being put between field names. Status: Not started
  8. Add support for JOIN, UNION and GROUP BY, with an interface to build them. Status: Not started
  9. Add logic for batch fetching in loops. Status: Not started
  10. Add logic for select_related. By design, prefetch_related will never be part of this ORM, preferring a 'fetch in batch when needed' approach. Status: Not started
  11. Look into supporting up to Python 3.7 by taking into account the possible usage of *Union* and *Optional* Maybe import from future? Status: Not started
  12. Improve testing by adding a way to catch queries made to the database, to make sure we lower them as much as possible. Status: Not started
  13. Add support for postgresql. Status: Not started
```

### Comparing `RogueORM-0.0.2/RogueORM.egg-info/SOURCES.txt` & `RogueORM-0.0.3/RogueORM.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,8 +21,10 @@
 rogue/managers/errors.py
 rogue/migrations/__init__.py
 rogue/migrations/base.py
 rogue/models/__init__.py
 rogue/models/base.py
 rogue/models/errors.py
 rogue/models/fields.py
-rogue/models/utils.py
+rogue/models/utils.py
+rogue/settings/__init__.py
+rogue/settings/default_settings.py
```

### Comparing `RogueORM-0.0.2/pyproject.toml` & `RogueORM-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ['setuptools>=61.0.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'RogueORM'
-version = '0.0.2'
+version = '0.0.3'
 description = 'An ORM that strives to eradicate N+1 issues.'
 readme = 'README.md'
 authors = [{name = 'Maxime Toussaint', email = 'm.toussaint@mail.com'}]
 license = {file = 'LICENSE'}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["orm", "database"]
-dependencies = []
+dependencies = ["python-dotenv", "sqlparse"]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/MaxDude132/RogueORM"
```

### Comparing `RogueORM-0.0.2/rogue/backends/base.py` & `RogueORM-0.0.3/rogue/backends/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from abc import ABCMeta, abstractmethod
 from collections.abc import Iterable
 from dataclasses import dataclass
 from typing import Any
 
+from rogue.settings import settings
+
 from .errors import OperationalError, InvalidComparisonError
 
 
 class BaseDatabaseClient(metaclass=ABCMeta):
     _instances = {}
     _db_name = None
 
-    def __new__(cls, db_name):
+    def __new__(cls, db_name=settings.DATABASE_NAME):
         if db_name not in cls._instances:
             cls._instances[db_name] = super().__new__(cls)
 
         return cls._instances[db_name]
 
-    def __init__(self, db_name):
+    def __init__(self, db_name=settings.DATABASE_NAME):
         self._db_name = db_name
 
         self._connection = None
 
     @abstractmethod
     def get_connection(self):  # pragma: no cover
         pass
@@ -166,17 +168,22 @@
         pass
 
     def _validate_data(self, data):
         assert data is not None, "Cannot insert without data."
 
 
 class BaseDatabaseSchemaEditor(metaclass=ABCMeta):
-    pass
+    def __init__(self, db_client: BaseDatabaseClient) -> None:
+        self._db_client = db_client
 
 
 class BaseDatabaseSchemaReader(metaclass=ABCMeta):
-    def __init__(self, db_client):
+    def __init__(self, db_client: BaseDatabaseClient) -> None:
         self._db_client = db_client
 
     @abstractmethod
     def get_tables(self):  # pragma: no cover
         pass
+
+    @abstractmethod
+    def get_rows(self, table_name):  # pragma: no cover
+        pass
```

### Comparing `RogueORM-0.0.2/rogue/backends/sqlite/client.py` & `RogueORM-0.0.3/rogue/backends/sqlite/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from rogue.settings import settings
+
 from ..base import BaseDatabaseClient
 import sqlite3
 
 from ..errors import OperationalError
 
 
 class DatabaseClient(BaseDatabaseClient):
```

### Comparing `RogueORM-0.0.2/rogue/backends/sqlite/query.py` & `RogueORM-0.0.3/rogue/backends/sqlite/query.py`

 * *Files identical despite different names*

### Comparing `RogueORM-0.0.2/rogue/managers/base.py` & `RogueORM-0.0.3/rogue/managers/base.py`

 * *Files identical despite different names*

### Comparing `RogueORM-0.0.2/rogue/models/base.py` & `RogueORM-0.0.3/rogue/models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from copy import copy
 from typing import Any
 import re
 
 from rogue.managers import Manager, RelationManager, ManyToManyManager
+from rogue.settings import settings
 
 from .fields import (
     BaseField,
     Field,
     RelationField,
     OneToOneWrapper,
     BaseWrapper,
@@ -47,15 +48,15 @@
 
     @classmethod
     def _get_table_name(cls, name):
         return "_".join(re.sub(r"([A-Z])", r" \1", name).split()).lower()
 
 
 class Model(metaclass=ModelMeta):
-    db_name = "default.sqlite"
+    db_name = settings.DATABASE_NAME
 
     def __init__(self, **kwargs):
         self._foreign_relations = {}
 
         id_ = kwargs.get("id")
 
         self._set_related_managers()
```

### Comparing `RogueORM-0.0.2/rogue/models/fields.py` & `RogueORM-0.0.3/rogue/models/fields.py`

 * *Files identical despite different names*

