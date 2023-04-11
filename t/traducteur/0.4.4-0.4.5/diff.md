# Comparing `tmp/traducteur-0.4.4.tar.gz` & `tmp/traducteur-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traducteur-0.4.4.tar", max compression
+gzip compressed data, was "traducteur-0.4.5.tar", max compression
```

## Comparing `traducteur-0.4.4.tar` & `traducteur-0.4.5.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0     1072 2023-04-11 19:25:11.123111 traducteur-0.4.4/LICENSE
--rw-r--r--   0        0        0     3588 2023-04-11 19:25:11.123111 traducteur-0.4.4/README.md
--rw-r--r--   0        0        0      756 2023-04-11 19:25:11.123111 traducteur-0.4.4/pyproject.toml
--rw-r--r--   0        0        0       37 2023-04-11 19:25:11.123111 traducteur-0.4.4/traducteur/context/__init__.py
--rw-r--r--   0        0        0      253 2023-04-11 19:25:11.123111 traducteur-0.4.4/traducteur/context/base.py
--rw-r--r--   0        0        0      606 2023-04-11 19:25:11.123111 traducteur-0.4.4/traducteur/context/mongo.py
--rw-r--r--   0        0        0      523 2023-04-11 19:25:11.123111 traducteur-0.4.4/traducteur/context/sqlite.py
--rw-r--r--   0        0        0       71 2023-04-11 19:25:11.123111 traducteur-0.4.4/traducteur/exceptions/tasks/__init__.py
--rw-r--r--   0        0        0       40 2023-04-11 19:25:11.123111 traducteur-0.4.4/traducteur/exceptions/tasks/base.py
--rw-r--r--   0        0        0       46 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/exceptions/tasks/worker.py
--rw-r--r--   0        0        0       34 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/__init__.py
--rw-r--r--   0        0        0      189 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/base.py
--rw-r--r--   0        0        0      264 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/base.py
--rw-r--r--   0        0        0      164 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/types/__init__.py
--rw-r--r--   0        0        0       73 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/types/base.py
--rw-r--r--   0        0        0      204 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/types/datetime_filter.py
--rw-r--r--   0        0        0      133 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/types/exists_filter.py
--rw-r--r--   0        0        0      189 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/types/number_filter.py
--rw-r--r--   0        0        0      229 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/types/string_filter.py
--rw-r--r--   0        0        0     3041 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/mongo.py
--rw-r--r--   0        0        0       33 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/query/__init__.py
--rw-r--r--   0        0        0     3798 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/query/sql.py
--rw-r--r--   0        0        0     2134 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/sql.py
--rw-r--r--   0        0        0       68 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/base/__init__.py
--rw-r--r--   0        0        0      805 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/base/base.py
--rw-r--r--   0        0        0      731 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/base/database.py
--rw-r--r--   0        0        0       68 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/document/__init__.py
--rw-r--r--   0        0        0     2828 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/document/mongo.py
--rw-r--r--   0        0        0      676 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/document/redis.py
--rw-r--r--   0        0        0     2301 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/relational/sql.py
--rw-r--r--   0        0        0       27 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/base/__init__.py
--rw-r--r--   0        0        0     1475 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/base/base.py
--rw-r--r--   0        0        0      548 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/base/lifetime.py
--rw-r--r--   0        0        0      130 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/base/status.py
--rw-r--r--   0        0        0       28 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/task/__init__.py
--rw-r--r--   0        0        0     1991 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/task/redis.py
--rw-r--r--   0        0        0      103 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/worker/base.py
--rw-r--r--   0        0        0     1138 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/worker/redis.py
--rw-r--r--   0        0        0     4634 1970-01-01 00:00:00.000000 traducteur-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-11 20:42:57.015424 traducteur-0.4.5/LICENSE
+-rw-r--r--   0        0        0     3588 2023-04-11 20:42:57.015424 traducteur-0.4.5/README.md
+-rw-r--r--   0        0        0      756 2023-04-11 20:42:57.015424 traducteur-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-04-11 20:42:57.015424 traducteur-0.4.5/traducteur/context/__init__.py
+-rw-r--r--   0        0        0      253 2023-04-11 20:42:57.015424 traducteur-0.4.5/traducteur/context/base.py
+-rw-r--r--   0        0        0      606 2023-04-11 20:42:57.015424 traducteur-0.4.5/traducteur/context/mongo.py
+-rw-r--r--   0        0        0      523 2023-04-11 20:42:57.015424 traducteur-0.4.5/traducteur/context/sqlite.py
+-rw-r--r--   0        0        0       71 2023-04-11 20:42:57.015424 traducteur-0.4.5/traducteur/exceptions/tasks/__init__.py
+-rw-r--r--   0        0        0       40 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/exceptions/tasks/base.py
+-rw-r--r--   0        0        0       46 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/exceptions/tasks/worker.py
+-rw-r--r--   0        0        0       34 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/__init__.py
+-rw-r--r--   0        0        0      189 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/base.py
+-rw-r--r--   0        0        0      264 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/base.py
+-rw-r--r--   0        0        0      164 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/types/__init__.py
+-rw-r--r--   0        0        0       73 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/types/base.py
+-rw-r--r--   0        0        0      204 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/types/datetime_filter.py
+-rw-r--r--   0        0        0      133 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/types/exists_filter.py
+-rw-r--r--   0        0        0      189 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/types/number_filter.py
+-rw-r--r--   0        0        0      229 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/filters/types/string_filter.py
+-rw-r--r--   0        0        0     3041 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/mongo.py
+-rw-r--r--   0        0        0       33 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/query/__init__.py
+-rw-r--r--   0        0        0     3798 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/query/sql.py
+-rw-r--r--   0        0        0     2136 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/managers/sql.py
+-rw-r--r--   0        0        0       68 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/models/base/__init__.py
+-rw-r--r--   0        0        0      805 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/models/base/base.py
+-rw-r--r--   0        0        0      731 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/models/base/database.py
+-rw-r--r--   0        0        0     2942 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/models/document/mongo.py
+-rw-r--r--   0        0        0      676 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/models/document/redis.py
+-rw-r--r--   0        0        0     2495 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/models/relational/sql.py
+-rw-r--r--   0        0        0       27 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/base/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/base/base.py
+-rw-r--r--   0        0        0      548 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/base/lifetime.py
+-rw-r--r--   0        0        0      130 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/base/status.py
+-rw-r--r--   0        0        0       28 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/task/__init__.py
+-rw-r--r--   0        0        0     1991 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/task/redis.py
+-rw-r--r--   0        0        0      103 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/worker/base.py
+-rw-r--r--   0        0        0     1138 2023-04-11 20:42:57.019424 traducteur-0.4.5/traducteur/tasks/worker/redis.py
+-rw-r--r--   0        0        0     4634 1970-01-01 00:00:00.000000 traducteur-0.4.5/PKG-INFO
```

### Comparing `traducteur-0.4.4/LICENSE` & `traducteur-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.4/README.md` & `traducteur-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.4/pyproject.toml` & `traducteur-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "traducteur"
-version = "0.4.4"
+version = "0.4.5"
 description = "Traducteur is the middle man to handle your basic data needs."
 authors = ["Seppe De Langhe <seppedelanghe@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.10.4"
```

### Comparing `traducteur-0.4.4/traducteur/context/mongo.py` & `traducteur-0.4.5/traducteur/context/mongo.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.4/traducteur/context/sqlite.py` & `traducteur-0.4.5/traducteur/context/sqlite.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.4/traducteur/managers/mongo.py` & `traducteur-0.4.5/traducteur/managers/mongo.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.4/traducteur/managers/query/sql.py` & `traducteur-0.4.5/traducteur/managers/query/sql.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.4/traducteur/managers/sql.py` & `traducteur-0.4.5/traducteur/managers/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,15 @@
             return session.query(exists().where(cls.id == id)).scalar()
 
     def all(self, cls, **kwargs) -> List[T]:
         with self.session() as session:
             qb = SQLQueryBuilder(session, cls)
             return qb.build(**kwargs).all()
 
-    def paginate(self, cls, page: int, per_page: int = 30, **kwargs) -> List[T]:
+    def paginate(self, cls, page: int = 0, per_page: int = 30, **kwargs) -> List[T]:
         with self.session() as session:
             qb = SQLQueryBuilder(session, cls).build(**kwargs)
             return qb.paginate(page, per_page)
 
     def query(self, query, one: bool = False, **kwargs) -> Union[Iterable[T], T]:
         with self.session() as session:
             return session.scalars(query).one() if one else session.scalars(query)
-
-
```

### Comparing `traducteur-0.4.4/traducteur/models/base/base.py` & `traducteur-0.4.5/traducteur/models/base/base.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.4/traducteur/models/base/database.py` & `traducteur-0.4.5/traducteur/models/base/database.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.4/traducteur/models/document/mongo.py` & `traducteur-0.4.5/traducteur/models/document/mongo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from bson import ObjectId
-from typing import Optional
 from pydantic import Field
+from typing import Optional, List
 
 from ..base import BaseDatabaseModel
 from ...managers.mongo import MongoModelManager
 
 
 class PydanticObjectId(ObjectId):
     @classmethod
@@ -52,40 +52,40 @@
     @classmethod
     def __get_manager(cls) -> MongoModelManager:
         con_str = os.environ['MONGO_CONNECTION_STR']
         db_name = os.environ['MONGO_DATABASE_NAME']
         return MongoModelManager(con_str, db_name)
 
     @classmethod
-    def get(cls, id: str):
+    def get(cls, id: str) -> Optional['BaseMongoModel']:
         manager = cls.__get_manager()
         result = manager.get_one(cls.__name__, id)
         return cls.from_dict(result) if result else None
 
     @classmethod
     def get_where_raw(cls, query, **kwargs):
         manager = cls.__get_manager()
         return manager.get_many(cls.__name__, query, **kwargs)
 
     @classmethod
-    def get_where(cls, query, **kwargs):
+    def get_where(cls, query, **kwargs) -> List['BaseMongoModel']:
         result = cls.get_where_raw(query, **kwargs)
-        return [cls.from_dict(i) for i in result] if len(result) > 0 else None
+        return [cls.from_dict(i) for i in result] if len(result) > 0 else []
 
     @classmethod
-    def get_one_where(cls, query, **kwargs):
+    def get_one_where(cls, query, **kwargs) -> Optional['BaseMongoModel']:
         manager = cls.__get_manager()
         result = manager.get_one(cls.__name__, query, **kwargs)
         return cls.from_dict(result) if result else None
 
     @classmethod
-    def all(cls, **kwargs):
+    def all(cls, **kwargs) -> List['BaseMongoModel']:
         manager = cls.__get_manager()
         result = manager.get_all(cls.__name__, **kwargs)
-        return [cls.from_dict(i) for i in result] if len(result) > 0 else None
+        return [cls.from_dict(i) for i in result] if len(result) > 0 else []
 
     @classmethod
     def exists(cls, id: str) -> bool:
         try:
             return cls.__get_manager().exists(cls.__name__, id=id)
         except Exception:
             return False
```

### Comparing `traducteur-0.4.4/traducteur/models/document/redis.py` & `traducteur-0.4.5/traducteur/models/document/redis.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.4/traducteur/models/relational/sql.py` & `traducteur-0.4.5/traducteur/models/relational/sql.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import json
 import os
+import json
 
-from datetime import datetime
-from typing import Any, TypeVar
 from uuid import uuid4
+from datetime import datetime
+from typing import TypeVar, List
 
-from sqlalchemy import String, Column, DATETIME
 from sqlalchemy.orm import declarative_base
+from sqlalchemy import String, Column, DATETIME
 
 from ..base import BaseDatabaseModel
 from ...managers.sql import SQLModelManager
 
 T = TypeVar('T')
 
 
@@ -41,15 +41,15 @@
             self.created_at = datetime.utcnow()
             self.updated_at = datetime.utcnow()
             return self.manager().insert(self)
 
     def delete(self):
         return self.manager().delete(self)
 
-    def map_to(self, cls):
+    def map_to(self, cls: 'BaseSQLModel'):
         return cls.from_dict(self.dict())
 
     def dict(self):
         return self.__dict__
 
     """
         Properties
@@ -58,40 +58,40 @@
     def classname(self) -> str:
         return self.__class__.__name__
 
     """
         Class methods
     """
     @classmethod
-    def map_from(cls, item: BaseDatabaseModel):
+    def map_from(cls, item: BaseDatabaseModel) -> 'BaseSQLModel':
         return cls.from_dict(item.dict())
 
     @classmethod
-    def from_dict(cls, values: dict) -> Any:
+    def from_dict(cls, values: dict) -> 'BaseSQLModel':
         return cls(**values)
 
     @classmethod
-    def from_json(cls, data: str) -> Any:
+    def from_json(cls, data: str) -> 'BaseSQLModel':
         return cls.from_dict(json.loads(data))
 
     @classmethod
-    def get(cls, id: str):
+    def get(cls, id: str) -> 'BaseSQLModel':
         return cls.manager().get(cls, id)
 
     @classmethod
-    def all(cls, *args, **kwargs):
+    def all(cls, **kwargs) -> List['BaseSQLModel']:
         return cls.manager().all(cls, **kwargs)
 
     @classmethod
-    def paginate(cls, *args, **kwargs):
-        return cls.manager().paginate(cls, *args, **kwargs)
+    def paginate(cls, page: int = 0, per_page: int = 30, *args, **kwargs) -> List['BaseSQLModel']:
+        return cls.manager().paginate(cls, page, per_page, *args, **kwargs)
 
     @classmethod
-    def exists(cls, id: str):
+    def exists(cls, id: str) -> bool:
         return cls.manager().exists(cls, id)
 
     @classmethod
-    def manager(cls):
+    def manager(cls) -> SQLModelManager:
         return SQLModelManager[cls](os.environ.get('SQL_CONNECTION_STRING'))
 
 
 SQLBase = declarative_base(cls=BaseSQLModel)
```

### Comparing `traducteur-0.4.4/traducteur/tasks/base/base.py` & `traducteur-0.4.5/traducteur/tasks/base/base.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.4/traducteur/tasks/base/lifetime.py` & `traducteur-0.4.5/traducteur/tasks/base/lifetime.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.4/traducteur/tasks/task/redis.py` & `traducteur-0.4.5/traducteur/tasks/task/redis.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.4/traducteur/tasks/worker/redis.py` & `traducteur-0.4.5/traducteur/tasks/worker/redis.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.4/PKG-INFO` & `traducteur-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traducteur
-Version: 0.4.4
+Version: 0.4.5
 Summary: Traducteur is the middle man to handle your basic data needs.
 Author: Seppe De Langhe
 Author-email: seppedelanghe@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

