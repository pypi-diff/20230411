# Comparing `tmp/sqlalchemy_extras-2.0.0.tar.gz` & `tmp/sqlalchemy_extras-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_extras-2.0.0.tar", max compression
+gzip compressed data, was "sqlalchemy_extras-2.0.1.tar", max compression
```

## Comparing `sqlalchemy_extras-2.0.0.tar` & `sqlalchemy_extras-2.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.0/README.md
--rw-r--r--   0        0        0      790 2023-04-11 17:49:09.114293 sqlalchemy_extras-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      183 2023-03-09 19:01:38.717890 sqlalchemy_extras-2.0.0/sqlalchemy_extras/__init__.py
--rw-r--r--   0        0        0     6662 2023-04-11 17:48:37.793160 sqlalchemy_extras-2.0.0/sqlalchemy_extras/fastapi.py
--rw-r--r--   0        0        0     5349 2023-04-11 17:48:37.793160 sqlalchemy_extras-2.0.0/sqlalchemy_extras/models.py
--rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.0/sqlalchemy_extras/py.typed
--rw-r--r--   0        0        0     2092 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.0/sqlalchemy_extras/utils.py
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 sqlalchemy_extras-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.1/README.md
+-rw-r--r--   0        0        0      790 2023-04-11 18:37:54.577136 sqlalchemy_extras-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-03-09 19:01:38.717890 sqlalchemy_extras-2.0.1/sqlalchemy_extras/__init__.py
+-rw-r--r--   0        0        0     6662 2023-04-11 17:48:37.793160 sqlalchemy_extras-2.0.1/sqlalchemy_extras/fastapi.py
+-rw-r--r--   0        0        0     5402 2023-04-11 18:37:10.574642 sqlalchemy_extras-2.0.1/sqlalchemy_extras/models.py
+-rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.1/sqlalchemy_extras/py.typed
+-rw-r--r--   0        0        0     2092 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.1/sqlalchemy_extras/utils.py
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 sqlalchemy_extras-2.0.1/PKG-INFO
```

### Comparing `sqlalchemy_extras-2.0.0/pyproject.toml` & `sqlalchemy_extras-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 authors = ["Francisco Del Roio <francipvb@hotmail.com>"]
 description = ""
 name = "sqlalchemy-extras"
 readme = "README.md"
-version = "2.0.0"
+version = "2.0.1"
 
 [tool.poetry.dependencies]
 sqlalchemy = "^2.0.9"
 fastapi = { version = ">=0.60.0,<1.0.0", optional = true }
 python = ">=3.10.0, <4"
 
 [tool.poetry.extras]
```

### Comparing `sqlalchemy_extras-2.0.0/sqlalchemy_extras/fastapi.py` & `sqlalchemy_extras-2.0.1/sqlalchemy_extras/fastapi.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_extras-2.0.0/sqlalchemy_extras/models.py` & `sqlalchemy_extras-2.0.1/sqlalchemy_extras/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # pylint: disable=not-callable
+from datetime import datetime
 import typing
 
-from sqlalchemy import TIMESTAMP, Boolean, false, func, Column, orm
+from sqlalchemy import TIMESTAMP, false, func, orm
 from sqlalchemy.types import TypeEngine
 
 from .utils import pluralize
 
 _TId = typing.TypeVar("_TId")
 
 
@@ -41,18 +42,16 @@
       ...
     AssertionError: ...
     >>>
     """
 
     __abstract__ = True
 
-    is_removed = Column(
-        Boolean,
+    is_removed: orm.Mapped[bool] = orm.mapped_column(
         index=True,
-        nullable=False,
         server_default=false(),
         comment="Soft deletion flag.",
     )
 
     def mark_removed(self):
         assert not self.is_removed, "Already marked."
         self.is_removed = True
@@ -78,25 +77,23 @@
     >>> item.updated
 
     >>>
     """
 
     __abstract__ = True
 
-    created = Column(
-        TIMESTAMP(),
+    created: orm.Mapped[datetime] = orm.mapped_column(
+        type_=TIMESTAMP(),
         server_default=func.current_timestamp(),
-        nullable=False,
         comment="When a row were added.",
     )
-    updated = Column(
-        TIMESTAMP(),
+    updated: orm.Mapped[datetime | None] = orm.mapped_column(
+        type_=TIMESTAMP(),
         onupdate=func.current_timestamp(),
         comment="Last row update date and time.",
-        nullable=True,
         default=None,
     )
 
     def touch(self):
         """Update the `updated` timestamp.
 
         This just sets the `updated` field to the `current_timestamp` function.
@@ -110,15 +107,15 @@
         ...
         >>> item=Item()
         >>> item.touch()
         >>> item.updated
         <sqlalchemy.sql.functions.current_timestamp at ...>
         >>>
         """
-        self.updated = func.current_timestamp()
+        self.updated = func.current_timestamp()  # type: ignore
 
 
 class Autonamed:
     """Auto-name table.
 
     >>> from sqlalchemy.orm import DeclarativeBase
     >>> class Base(DeclarativeBase):
@@ -159,15 +156,15 @@
     __abstract__ = True
 
     __pk_type__: typing.ClassVar[typing.Optional[TypeEngine[typing.Any]]] = None
     __pk_kwargs__: typing.ClassVar[
         typing.Optional[typing.Mapping[str, typing.Any]]
     ] = None
 
-    # id: orm.Mapped[_TId]
+    id: orm.Mapped[_TId]
 
     def __init_subclass__(cls, *args: typing.Any, **kwargs: typing.Any) -> None:
         orig_bases: typing.Tuple[typing.Any, ...] = cls.__orig_bases__  # type: ignore
         entity_name: str = cls.__name__.lower()  # type: ignore
 
         column_kwargs: typing.Dict[str, typing.Any] = (
             dict(cls.__pk_kwargs__) if cls.__pk_kwargs__ is not None else dict()
```

### Comparing `sqlalchemy_extras-2.0.0/sqlalchemy_extras/utils.py` & `sqlalchemy_extras-2.0.1/sqlalchemy_extras/utils.py`

 * *Files identical despite different names*

