# Comparing `tmp/fastapi-listing-0.0.0.tar.gz` & `tmp/fastapi-listing-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-listing-0.0.0.tar", last modified: Sat Mar 25 09:06:15 2023, max compression
+gzip compressed data, was "fastapi-listing-0.0.1.tar", last modified: Tue Apr 11 07:55:43 2023, max compression
```

## Comparing `fastapi-listing-0.0.0.tar` & `fastapi-listing-0.0.1.tar`

### file list

```diff
@@ -1,41 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 09:06:15.770006 fastapi-listing-0.0.0/
--rw-rw-rw-   0        0        0      840 2023-03-25 09:06:15.769005 fastapi-listing-0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-25 09:06:15.739350 fastapi-listing-0.0.0/fastapi_listing/
--rw-rw-rw-   0        0        0       28 2023-03-25 08:33:42.000000 fastapi-listing-0.0.0/fastapi_listing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 09:06:15.761999 fastapi-listing-0.0.0/fastapi_listing/abstracts/
--rw-rw-rw-   0        0        0      453 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/abstracts/__init__.py
--rw-rw-rw-   0        0        0      327 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/abstracts/base_query.py
--rw-rw-rw-   0        0        0      576 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/abstracts/dao.py
--rw-rw-rw-   0        0        0      174 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/abstracts/filter.py
--rw-rw-rw-   0        0        0      855 2023-03-24 11:31:41.000000 fastapi-listing-0.0.0/fastapi_listing/abstracts/listing.py
--rw-rw-rw-   0        0        0      582 2023-03-24 11:34:09.000000 fastapi-listing-0.0.0/fastapi_listing/abstracts/listing_meta_info.py
--rw-rw-rw-   0        0        0      241 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/abstracts/paginator.py
--rw-rw-rw-   0        0        0      189 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/abstracts/sorter.py
--rw-rw-rw-   0        0        0     2867 2023-03-25 08:20:57.000000 fastapi-listing-0.0.0/fastapi_listing/dao_demo.py
--rw-rw-rw-   0        0        0      177 2023-03-24 11:31:41.000000 fastapi-listing-0.0.0/fastapi_listing/errors.py
-drwxrwxrwx   0        0        0        0 2023-03-25 09:06:15.764001 fastapi-listing-0.0.0/fastapi_listing/factory/
--rw-rw-rw-   0        0        0      120 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/factory/__init__.py
--rw-rw-rw-   0        0        0      502 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/factory/filter.py
--rw-rw-rw-   0        0        0      658 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/factory/strategy.py
-drwxrwxrwx   0        0        0        0 2023-03-25 09:06:15.765002 fastapi-listing-0.0.0/fastapi_listing/filters/
--rw-rw-rw-   0        0        0      507 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/filters/__init__.py
--rw-rw-rw-   0        0        0     4747 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/filters/generic_filters.py
--rw-rw-rw-   0        0        0     6600 2023-03-24 18:47:53.000000 fastapi-listing-0.0.0/fastapi_listing/listing_main.py
--rw-rw-rw-   0        0        0        0 2023-03-24 11:05:00.000000 fastapi-listing-0.0.0/fastapi_listing/logger.py
-drwxrwxrwx   0        0        0        0 2023-03-25 09:06:15.767003 fastapi-listing-0.0.0/fastapi_listing/paginator/
--rw-rw-rw-   0        0        0       80 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/paginator/__init__.py
--rw-rw-rw-   0        0        0     1362 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/paginator/naive_page_builder.py
--rw-rw-rw-   0        0        0       25 2023-03-24 18:10:43.000000 fastapi-listing-0.0.0/fastapi_listing/py.typed
-drwxrwxrwx   0        0        0        0 2023-03-25 09:06:15.768005 fastapi-listing-0.0.0/fastapi_listing/sorter/
--rw-rw-rw-   0        0        0      189 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/sorter/__init__.py
--rw-rw-rw-   0        0        0     2273 2023-03-25 08:33:42.000000 fastapi-listing-0.0.0/fastapi_listing/sorter/naive_page_sorter.py
--rw-rw-rw-   0        0        0      384 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/typing.py
--rw-rw-rw-   0        0        0      184 2023-03-24 09:55:15.000000 fastapi-listing-0.0.0/fastapi_listing/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-25 09:06:15.755365 fastapi-listing-0.0.0/fastapi_listing.egg-info/
--rw-rw-rw-   0        0        0      840 2023-03-25 09:06:15.000000 fastapi-listing-0.0.0/fastapi_listing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1074 2023-03-25 09:06:15.000000 fastapi-listing-0.0.0/fastapi_listing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 09:06:15.000000 fastapi-listing-0.0.0/fastapi_listing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2023-03-25 09:06:15.000000 fastapi-listing-0.0.0/fastapi_listing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-25 09:06:15.000000 fastapi-listing-0.0.0/fastapi_listing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-25 09:06:15.770006 fastapi-listing-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1813 2023-03-25 08:46:01.000000 fastapi-listing-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.723464 fastapi-listing-0.0.1/fastapi_listing/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.727464 fastapi-listing-0.0.1/fastapi_listing/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/base_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/listing_meta_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/abstracts/sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.727464 fastapi-listing-0.0.1/fastapi_listing/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/factory/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/factory/generic_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/factory/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.727464 fastapi-listing-0.0.1/fastapi_listing/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/filters/generic_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/generic_dao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/fastapi_listing/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10969 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/listing_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/fastapi_listing/paginator/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/paginator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/paginator/naive_page_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/fastapi_listing/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/plugins/filter_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/plugins/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/plugins/sorter_machanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/fastapi_listing/sorter/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/sorter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/sorter/naive_page_sorter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/fastapi_listing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:55:43.723464 fastapi-listing-0.0.1/fastapi_listing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-11 07:55:43.000000 fastapi-listing-0.0.1/fastapi_listing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-11 07:55:43.000000 fastapi-listing-0.0.1/fastapi_listing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:55:43.000000 fastapi-listing-0.0.1/fastapi_listing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-11 07:55:43.000000 fastapi-listing-0.0.1/fastapi_listing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 07:55:43.000000 fastapi-listing-0.0.1/fastapi_listing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 07:55:43.731464 fastapi-listing-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-11 07:55:30.000000 fastapi-listing-0.0.1/setup.py
```

### Comparing `fastapi-listing-0.0.0/fastapi_listing/abstracts/dao.py` & `fastapi-listing-0.0.1/fastapi_listing/abstracts/dao.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from abc import ABCMeta, abstractmethod
 
-from fastapi_listing.typing import TableModelTyp
+from fastapi_listing.typing import SqlAlchemyModel
 
 
 class DaoAbstract(metaclass=ABCMeta):
 
     @abstractmethod
-    def create(self, values: dict[str, str | int]) -> TableModelTyp:
+    def create(self, values: dict[str, str | int]) -> SqlAlchemyModel:
         pass
 
     @abstractmethod
     def update(self, identifier: dict[str, str | int | list], values: dict) -> bool:
         pass
 
     @abstractmethod
-    def read(self, identifier: dict[str, str | int | list], fields: list | str = "__all__") -> TableModelTyp:
+    def read(self, identifier: dict[str, str | int | list], fields: list | str = "__all__") -> SqlAlchemyModel:
         pass
 
     @abstractmethod
     def delete(self, ids: list[int]) -> bool:
         pass
```

### Comparing `fastapi-listing-0.0.0/fastapi_listing/dao_demo.py` & `fastapi-listing-0.0.1/fastapi_listing/generic_dao.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from fastapi_listing.abstracts import DaoAbstract
-from sqlalchemy.orm import Session
-
-from fastapi_listing.typing import TableModelTyp
-
-
-class DaoDemo(DaoAbstract):
-
-    """
-    Dao stands for data access object.
-    This layers encapsulates all logic that a user may write
-    in order to interact with databases.
-    Dao has only one responsibility that is to communicate with
-    database, all logic regarding data manipulation should live at
-    service layer. This also acts as a gateway to database
-    a wrapper on top of existing orm where generic logic could be defined.
-
-    This is a demo class showing how one can benefit from it.
-    Please note that this is just a basic implementation
-    i.e., a basic recipe, if one want they can spice it up as they like.
-
-    A dao should only have a primary table as we are speaking in terms of orm
-    we will call it a model.
-    so a dao should only be associated with single model or model class.
-    i.e., one primary model per dao instance. please note that this is different from
-    joining multiple models or tables. we are strictly  speaking in terms of
-    objects context here that one dao object should only have one primary model
-    but one dao object can talk to multiple models with having first primary model.
-
-    Note - no data validation should happen at this layer. That should be prior to pushing
-    at this layer.
-    """
-
-    def __init__(self, model, **kwargs):
-        # considering that we are dealing with separate read and write dbs.
-        # we must have two sessions one for read replica and one for master or write replica
-        # we should define our reusable attributes here that we will use in each dao method definition
-        self._read_db: Session = kwargs.get("read_db_session")
-        self._write_db: Session = kwargs.get("write_db_session")
-        self.model = model
-
-    def create(self, values: dict[str, str | int]) -> TableModelTyp:
-        """
-        A light method that enters values in primary model table.
-        single value at a time receives a dict implementation could map the dict with model values and
-        insert that mapping or single row into the table.
-        :param values: dict of values where keys are columns of table and value should be row values
-        :return: created object i.e., instrumented row object.
-        """
-        pass
-
-    def update(self, identifier: dict[str, str | int | list], values: dict) -> bool:
-        """
-        Similar to create method this receives an identifier
-        :param identifier:
-        :param values:
-        :return:
-        """
-        pass
-
-    def read(self, identifier: dict[str, str | int | list], fields: list | str = "__all__") -> TableModelTyp:
-        pass
-
-    def delete(self, ids: list[int]) -> bool:
-        pass
+from fastapi_listing.abstracts import DaoAbstract
+from sqlalchemy.orm import Session
+
+from fastapi_listing.typing import SqlAlchemyModel
+
+
+class GenericDao(DaoAbstract):
+
+    """
+    Dao stands for data access object.
+    This layers encapsulates all logic that a user may write
+    in order to interact with databases.
+    Dao has only one responsibility that is to communicate with
+    database, all logic regarding data manipulation should live at
+    service layer. This also acts as a gateway to database
+    a wrapper on top of existing orm where generic logic could be defined.
+
+    This is a demo class showing how one can benefit from it.
+    Please note that this is just a basic implementation
+    i.e., a basic recipe, if one want they can spice it up as they like.
+
+    A dao should only have a primary table as we are speaking in terms of orm
+    we will call it a model.
+    so a dao should only be associated with single model or model class.
+    i.e., one primary model per dao instance. please note that this is different from
+    joining multiple models or tables. we are strictly  speaking in terms of
+    objects context here that one dao object should only have one primary model
+    but one dao object can talk to multiple models with having first primary model.
+
+    Note - no data validation should happen at this layer. That should be prior to pushing
+    at this layer.
+    """
+
+    def __init__(self, model, **kwargs):
+        # considering that we are dealing with separate read and write dbs.
+        # we must have two sessions one for read replica and one for master or write replica
+        # we should define our reusable attributes here that we will use in each dao method definition
+        self._read_db: Session = kwargs.get("read_db_session")
+        self._write_db: Session = kwargs.get("write_db_session")
+        self.model = model
+
+    def create(self, values: dict[str, str | int]) -> SqlAlchemyModel:
+        """
+        A light method that enters values in primary model table.
+        single value at a time receives a dict implementation could map the dict with model values and
+        insert that mapping or single row into the table.
+        :param values: dict of values where keys are columns of table and value should be row values
+        :return: created object i.e., instrumented row object.
+        """
+        pass
+
+    def update(self, identifier: dict[str, str | int | list], values: dict) -> bool:
+        """
+        Similar to create method this receives an identifier
+        :param identifier:
+        :param values:
+        :return:
+        """
+        pass
+
+    def read(self, identifier: dict[str, str | int | list], fields: list | str = "__all__") -> SqlAlchemyModel:
+        pass
+
+    def delete(self, ids: list[int]) -> bool:
+        pass
```

### Comparing `fastapi-listing-0.0.0/fastapi_listing/factory/strategy.py` & `fastapi-listing-0.0.1/fastapi_listing/factory/strategy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 
 class StrategyObjectFactory:
     def __init__(self):
         self._strategy = {}
 
-    def register_strategy(self, key, builder):
+    def register_strategy(self, key: str, builder: type):
         if key in self._strategy:
             raise ValueError(f"strategy name already in use with {self._strategy[key].__name__}!")
         if not isinstance(builder, object):
             raise ValueError(f"builder is not a valid callable!")
         self._strategy[key] = builder
 
-    def create(self, key, *args, **kwargs) -> object:
+    def create(self, key: str, *args, **kwargs) -> object:
         strategy_ = self._strategy.get(key)
         if not strategy_:
             raise ValueError(key)
         return strategy_(*args, **kwargs)
 
 
 strategy_factory = StrategyObjectFactory()
```

### Comparing `fastapi-listing-0.0.0/fastapi_listing/filters/generic_filters.py` & `fastapi-listing-0.0.1/fastapi_listing/filters/generic_filters.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.0/fastapi_listing/paginator/naive_page_builder.py` & `fastapi-listing-0.0.1/fastapi_listing/paginator/naive_page_builder.py`

 * *Files identical despite different names*

### Comparing `fastapi-listing-0.0.0/fastapi_listing.egg-info/SOURCES.txt` & `fastapi-listing-0.0.1/fastapi_listing.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+README.md
 setup.py
 fastapi_listing/__init__.py
-fastapi_listing/dao_demo.py
 fastapi_listing/errors.py
+fastapi_listing/generic_dao.py
 fastapi_listing/listing_main.py
 fastapi_listing/logger.py
 fastapi_listing/py.typed
 fastapi_listing/typing.py
 fastapi_listing/utils.py
 fastapi_listing.egg-info/PKG-INFO
 fastapi_listing.egg-info/SOURCES.txt
@@ -18,14 +19,20 @@
 fastapi_listing/abstracts/filter.py
 fastapi_listing/abstracts/listing.py
 fastapi_listing/abstracts/listing_meta_info.py
 fastapi_listing/abstracts/paginator.py
 fastapi_listing/abstracts/sorter.py
 fastapi_listing/factory/__init__.py
 fastapi_listing/factory/filter.py
+fastapi_listing/factory/generic_factory.py
 fastapi_listing/factory/strategy.py
 fastapi_listing/filters/__init__.py
 fastapi_listing/filters/generic_filters.py
+fastapi_listing/interface/__init__.py
 fastapi_listing/paginator/__init__.py
 fastapi_listing/paginator/naive_page_builder.py
+fastapi_listing/plugins/__init__.py
+fastapi_listing/plugins/filter_mechanics.py
+fastapi_listing/plugins/loader.py
+fastapi_listing/plugins/sorter_machanics.py
 fastapi_listing/sorter/__init__.py
 fastapi_listing/sorter/naive_page_sorter.py
```

