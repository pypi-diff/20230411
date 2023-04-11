# Comparing `tmp/traducteur-0.4.3.tar.gz` & `tmp/traducteur-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traducteur-0.4.3.tar", max compression
+gzip compressed data, was "traducteur-0.4.4.tar", max compression
```

## Comparing `traducteur-0.4.3.tar` & `traducteur-0.4.4.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0     1072 2023-01-28 14:36:20.793000 traducteur-0.4.3/LICENSE
--rw-r--r--   0        0        0     3588 2023-01-28 14:36:20.793000 traducteur-0.4.3/README.md
--rw-r--r--   0        0        0      756 2023-01-28 14:36:20.793000 traducteur-0.4.3/pyproject.toml
--rw-r--r--   0        0        0       37 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/context/__init__.py
--rw-r--r--   0        0        0      253 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/context/base.py
--rw-r--r--   0        0        0      606 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/context/mongo.py
--rw-r--r--   0        0        0      523 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/context/sqlite.py
--rw-r--r--   0        0        0       71 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/exceptions/tasks/__init__.py
--rw-r--r--   0        0        0       40 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/exceptions/tasks/base.py
--rw-r--r--   0        0        0       46 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/exceptions/tasks/worker.py
--rw-r--r--   0        0        0       34 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/managers/__init__.py
--rw-r--r--   0        0        0      189 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/managers/base.py
--rw-r--r--   0        0        0      264 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/managers/filters/base.py
--rw-r--r--   0        0        0      164 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/managers/filters/types/__init__.py
--rw-r--r--   0        0        0       73 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/managers/filters/types/base.py
--rw-r--r--   0        0        0      204 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/managers/filters/types/datetime_filter.py
--rw-r--r--   0        0        0      133 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/managers/filters/types/exists_filter.py
--rw-r--r--   0        0        0      189 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/managers/filters/types/number_filter.py
--rw-r--r--   0        0        0      229 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/managers/filters/types/string_filter.py
--rw-r--r--   0        0        0     3041 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/managers/mongo.py
--rw-r--r--   0        0        0       33 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/managers/query/__init__.py
--rw-r--r--   0        0        0     3798 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/managers/query/sql.py
--rw-r--r--   0        0        0     2134 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/managers/sql.py
--rw-r--r--   0        0        0       68 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/models/base/__init__.py
--rw-r--r--   0        0        0      805 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/models/base/base.py
--rw-r--r--   0        0        0      731 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/models/base/database.py
--rw-r--r--   0        0        0       68 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/models/document/__init__.py
--rw-r--r--   0        0        0     2828 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/models/document/mongo.py
--rw-r--r--   0        0        0      672 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/models/document/redis.py
--rw-r--r--   0        0        0     2301 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/models/relational/sql.py
--rw-r--r--   0        0        0       27 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/tasks/base/__init__.py
--rw-r--r--   0        0        0     1475 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/tasks/base/base.py
--rw-r--r--   0        0        0      548 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/tasks/base/lifetime.py
--rw-r--r--   0        0        0      130 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/tasks/base/status.py
--rw-r--r--   0        0        0       28 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/tasks/task/__init__.py
--rw-r--r--   0        0        0     1991 2023-01-28 14:36:20.793000 traducteur-0.4.3/traducteur/tasks/task/redis.py
--rw-r--r--   0        0        0      103 2023-01-28 14:36:20.797000 traducteur-0.4.3/traducteur/tasks/worker/base.py
--rw-r--r--   0        0        0     1138 2023-01-28 14:36:20.797000 traducteur-0.4.3/traducteur/tasks/worker/redis.py
--rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 traducteur-0.4.3/setup.py
--rw-r--r--   0        0        0     4634 1970-01-01 00:00:00.000000 traducteur-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-11 19:25:11.123111 traducteur-0.4.4/LICENSE
+-rw-r--r--   0        0        0     3588 2023-04-11 19:25:11.123111 traducteur-0.4.4/README.md
+-rw-r--r--   0        0        0      756 2023-04-11 19:25:11.123111 traducteur-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-04-11 19:25:11.123111 traducteur-0.4.4/traducteur/context/__init__.py
+-rw-r--r--   0        0        0      253 2023-04-11 19:25:11.123111 traducteur-0.4.4/traducteur/context/base.py
+-rw-r--r--   0        0        0      606 2023-04-11 19:25:11.123111 traducteur-0.4.4/traducteur/context/mongo.py
+-rw-r--r--   0        0        0      523 2023-04-11 19:25:11.123111 traducteur-0.4.4/traducteur/context/sqlite.py
+-rw-r--r--   0        0        0       71 2023-04-11 19:25:11.123111 traducteur-0.4.4/traducteur/exceptions/tasks/__init__.py
+-rw-r--r--   0        0        0       40 2023-04-11 19:25:11.123111 traducteur-0.4.4/traducteur/exceptions/tasks/base.py
+-rw-r--r--   0        0        0       46 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/exceptions/tasks/worker.py
+-rw-r--r--   0        0        0       34 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/__init__.py
+-rw-r--r--   0        0        0      189 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/base.py
+-rw-r--r--   0        0        0      264 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/base.py
+-rw-r--r--   0        0        0      164 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/types/__init__.py
+-rw-r--r--   0        0        0       73 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/types/base.py
+-rw-r--r--   0        0        0      204 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/types/datetime_filter.py
+-rw-r--r--   0        0        0      133 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/types/exists_filter.py
+-rw-r--r--   0        0        0      189 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/types/number_filter.py
+-rw-r--r--   0        0        0      229 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/filters/types/string_filter.py
+-rw-r--r--   0        0        0     3041 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/mongo.py
+-rw-r--r--   0        0        0       33 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/query/__init__.py
+-rw-r--r--   0        0        0     3798 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/query/sql.py
+-rw-r--r--   0        0        0     2134 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/managers/sql.py
+-rw-r--r--   0        0        0       68 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/base/__init__.py
+-rw-r--r--   0        0        0      805 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/base/base.py
+-rw-r--r--   0        0        0      731 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/base/database.py
+-rw-r--r--   0        0        0       68 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/document/__init__.py
+-rw-r--r--   0        0        0     2828 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/document/mongo.py
+-rw-r--r--   0        0        0      676 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/document/redis.py
+-rw-r--r--   0        0        0     2301 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/models/relational/sql.py
+-rw-r--r--   0        0        0       27 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/base/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/base/base.py
+-rw-r--r--   0        0        0      548 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/base/lifetime.py
+-rw-r--r--   0        0        0      130 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/base/status.py
+-rw-r--r--   0        0        0       28 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/task/__init__.py
+-rw-r--r--   0        0        0     1991 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/task/redis.py
+-rw-r--r--   0        0        0      103 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/worker/base.py
+-rw-r--r--   0        0        0     1138 2023-04-11 19:25:11.127111 traducteur-0.4.4/traducteur/tasks/worker/redis.py
+-rw-r--r--   0        0        0     4634 1970-01-01 00:00:00.000000 traducteur-0.4.4/PKG-INFO
```

### Comparing `traducteur-0.4.3/LICENSE` & `traducteur-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/README.md` & `traducteur-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/pyproject.toml` & `traducteur-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "traducteur"
-version = "0.4.3"
+version = "0.4.4"
 description = "Traducteur is the middle man to handle your basic data needs."
 authors = ["Seppe De Langhe <seppedelanghe@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.10.4"
```

### Comparing `traducteur-0.4.3/traducteur/context/mongo.py` & `traducteur-0.4.4/traducteur/context/mongo.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/traducteur/context/sqlite.py` & `traducteur-0.4.4/traducteur/context/sqlite.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/traducteur/managers/mongo.py` & `traducteur-0.4.4/traducteur/managers/mongo.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/traducteur/managers/query/sql.py` & `traducteur-0.4.4/traducteur/managers/query/sql.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/traducteur/managers/sql.py` & `traducteur-0.4.4/traducteur/managers/sql.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/traducteur/models/base/base.py` & `traducteur-0.4.4/traducteur/models/base/base.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/traducteur/models/base/database.py` & `traducteur-0.4.4/traducteur/models/base/database.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/traducteur/models/document/mongo.py` & `traducteur-0.4.4/traducteur/models/document/mongo.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/traducteur/models/document/redis.py` & `traducteur-0.4.4/traducteur/models/document/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import redis
 import os
+import redis
 
 from ..base import BaseDatabaseModel
 
 
 class BaseRedisModel(BaseDatabaseModel):
     @classmethod
     def get(cls, uuid: str):
         r = cls.redis_instance()
         out = r.get(uuid)
         return cls.from_json(out) if isinstance(out, bytes) else None
 
     def save(self):
         r = self.redis_instance()
-        r.set(self.id, self.json(), ex=float(os.environ.get('REDIS_TTL', None)))
+        r.set(self.id, self.json(), ex=float(os.environ.get('REDIS_TTL', '86400')))
         return self
 
     def delete(self):
         r = self.redis_instance()
         r.delete(self.id)
 
     @staticmethod
     def redis_instance():
-        return redis.Redis(host=os.environ.get('REDIS_HOST'), port=int(os.environ.get('REDIS_PORT', '6379')))
+        return redis.Redis(host=os.environ.get('REDIS_HOST'), port=int(os.environ.get('REDIS_PORT', '6379')))
```

### Comparing `traducteur-0.4.3/traducteur/models/relational/sql.py` & `traducteur-0.4.4/traducteur/models/relational/sql.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/traducteur/tasks/base/base.py` & `traducteur-0.4.4/traducteur/tasks/base/base.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/traducteur/tasks/base/lifetime.py` & `traducteur-0.4.4/traducteur/tasks/base/lifetime.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/traducteur/tasks/task/redis.py` & `traducteur-0.4.4/traducteur/tasks/task/redis.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/traducteur/tasks/worker/redis.py` & `traducteur-0.4.4/traducteur/tasks/worker/redis.py`

 * *Files identical despite different names*

### Comparing `traducteur-0.4.3/setup.py` & `traducteur-0.4.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,227 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['traducteur',
- 'traducteur.context',
- 'traducteur.exceptions.tasks',
- 'traducteur.managers',
- 'traducteur.managers.filters',
- 'traducteur.managers.filters.types',
- 'traducteur.managers.query',
- 'traducteur.models.base',
- 'traducteur.models.document',
- 'traducteur.models.relational',
- 'traducteur.tasks.base',
- 'traducteur.tasks.task',
- 'traducteur.tasks.worker']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pydantic>=1.10.4,<2.0.0']
-
-extras_require = \
-{'all': ['redis>=4.2.2,<5.0.0',
-         'pymongo>=4.3.3,<5.0.0',
-         'sqlalchemy>=1.4.46,<2.0.0',
-         'dill>=0.3.6,<0.4.0'],
- 'caching': ['redis>=4.2.2,<5.0.0'],
- 'mongo': ['pymongo>=4.3.3,<5.0.0'],
- 'nosql': ['redis>=4.2.2,<5.0.0', 'pymongo>=4.3.3,<5.0.0'],
- 'sql': ['sqlalchemy>=1.4.46,<2.0.0'],
- 'tasks': ['redis>=4.2.2,<5.0.0', 'dill>=0.3.6,<0.4.0']}
-
-setup_kwargs = {
-    'name': 'traducteur',
-    'version': '0.4.3',
-    'description': 'Traducteur is the middle man to handle your basic data needs.',
-    'long_description': '# Traducteur\nTraducteur is a database model manager and task sheduler which aims to make developing basic app with database models and tasks faster and easier.\n\n\n<div align="center">\n    <img src="https://img.shields.io/pypi/v/traducteur"/>\n    <img src="https://img.shields.io/pypi/dm/traducteur"/>\n    <img src="https://img.shields.io/github/actions/workflow/status/seppedelanghe/traducteur/tests.yaml?label=tests" />\n    <br/>\n    <img src="https://img.shields.io/pypi/pyversions/traducteur"/>\n    <img src="https://img.shields.io/github/languages/code-size/seppedelanghe/traducteur"/>\n</div>\n\n## Requirements\n- `python ^3.8`\n- `pydantic ^1.10.4`\n\n### Optional\n__For mongo db:__\n- `pymongo ^4.3.3`\n\n__For task queueing or redis model management:__\n- `redis-py ^4.4.2`\n\n## Installation\n__Base install:__\n```\npip install traducteur\n```\n\n__Install with extras:__\n```\npip install "traducteur[tasks]"\n```\nThis example will install traducteur and all the packages you need to use traducteur tasks.\n\n__optional extras:__\n- sql\n- nosql\n- caching\n- mongo\n- tasks\n- all\n\n\n## The idea\n\n### Context managers\n```python\nwith BaseContext(connection_string) as db:\n    return db.get()\n```\n\n### Model managers\nModel managers use context managers\n```python\nmanager = BaseModelManager(connection_string)\nresult = manager.get(example_id)\nresult = manager.delete(example_id)\n```\n\n### Models\nModels use model managers\n```python\nclass User(BaseDatabaseModel):\n    username: str\n    fname: str\n    lname: str\n    email: str\n    \nuser = User(\n    username=\'johndoe\',\n    fname=\'John\',\n    lname=\'Doe\',\n    email=\'john.doe@mail.com\'\n)\n\n\'\'\'\n    Easy create, save, update and delete\n\'\'\'\nuser = User(\n    username=\'johndoe\',\n    fname=\'John\',\n    lname=\'Doe\',\n    email=\'john.doe@mail.com\'\n)\n\n# saving the model\nuser = user.save()\n\n# saving also updates the model\nuser.lname = \'Joe\'\nuser = user.save()\n\n# getting a model by its ID from the database\nuser = User.get(user_id)\n\n# deleting a model from the database\ndeleted_user = user.delete()\n```\n\n### Tasks\nTasks use models\n```python\n# in a program\ndef my_func(a: int, b: int) -> int:\n  return a + b\n\ntask = BaseTask(action=my_func)\ntask.queue(a=8, b=3)\n\n###############\n# in a worker #\ntask.digest() #\n###############\n\n# some time later\nresult = task.result()\n```\n\n### Chain tasks\nTasks can be chained together for larger workloads\n```python\ndef double(number: int):\n    return {\n        \'number\': number * 2\n    }\n\n# make tasks\none = BaseTask(action=double)\ntwo = BaseTask(action=double)\nthree = BaseTask(action=double)\n\n# chain tasks\ntwo.set_parent(one)\nthree.set_parent(two)\n\n# queue parent task\none.queue(number=2)\n\n###############\n# in a worker #\none.digest()  #\n###############\n\n# some time later\nresult = one.result()\nassert result == 8, "Should be 8 as 2*2*2 == 8"\n```\n\n## Available functionality\n\n### Context managers\n- MongoContext\n- SQLite3Context\n\n\n### Model managers\n- MongoModelManager\n- SQLModelManager\n  - SQLQueryBuilder\n\n### Query filters\n- Datetime filter\n- Number filter\n- String filter\n\n### Models\n- BaseMongoModel\n- BaseRedisModel\n- BaseSQLModel\n\n### Tasks\n- RedisTask\n\n# Todo / in progress\n\n### Tasks\n- [ ] Chain tasks\n    - [x] Redis\n    - [ ] Mongo\n    - [ ] SQL\n- [ ] Task worker\n  \t- [ ] Single Process\n    - [ ] Multi Process\n- [ ] RabbitMQ task\n\n# Tests\n\nTests can be found in the `test` folder. They use pythons `unittest` and can be run with:\n```\npython3 -m unittest path/to/test.py\n```\n\nTests get automatically run after each push.\n\n### Available tests\n- Mongo model\n- Mongo sorting\n- Redis task\n    - Basic functions\n    - Chaining',
-    'author': 'Seppe De Langhe',
-    'author_email': 'seppedelanghe@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: traducteur
+Version: 0.4.4
+Summary: Traducteur is the middle man to handle your basic data needs.
+Author: Seppe De Langhe
+Author-email: seppedelanghe@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: caching
+Provides-Extra: mongo
+Provides-Extra: nosql
+Provides-Extra: sql
+Provides-Extra: tasks
+Requires-Dist: dill (>=0.3.6,<0.4.0) ; extra == "tasks" or extra == "all"
+Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: pymongo (>=4.3.3,<5.0.0) ; extra == "mongo" or extra == "nosql" or extra == "all"
+Requires-Dist: redis (>=4.2.2,<5.0.0) ; extra == "tasks" or extra == "caching" or extra == "nosql" or extra == "all"
+Requires-Dist: sqlalchemy (>=1.4.46,<2.0.0) ; extra == "sql" or extra == "all"
+Description-Content-Type: text/markdown
+
+# Traducteur
+Traducteur is a database model manager and task sheduler which aims to make developing basic app with database models and tasks faster and easier.
+
+
+<div align="center">
+    <img src="https://img.shields.io/pypi/v/traducteur"/>
+    <img src="https://img.shields.io/pypi/dm/traducteur"/>
+    <img src="https://img.shields.io/github/actions/workflow/status/seppedelanghe/traducteur/tests.yaml?label=tests" />
+    <br/>
+    <img src="https://img.shields.io/pypi/pyversions/traducteur"/>
+    <img src="https://img.shields.io/github/languages/code-size/seppedelanghe/traducteur"/>
+</div>
+
+## Requirements
+- `python ^3.8`
+- `pydantic ^1.10.4`
+
+### Optional
+__For mongo db:__
+- `pymongo ^4.3.3`
+
+__For task queueing or redis model management:__
+- `redis-py ^4.4.2`
+
+## Installation
+__Base install:__
+```
+pip install traducteur
+```
+
+__Install with extras:__
+```
+pip install "traducteur[tasks]"
+```
+This example will install traducteur and all the packages you need to use traducteur tasks.
+
+__optional extras:__
+- sql
+- nosql
+- caching
+- mongo
+- tasks
+- all
+
+
+## The idea
+
+### Context managers
+```python
+with BaseContext(connection_string) as db:
+    return db.get()
+```
+
+### Model managers
+Model managers use context managers
+```python
+manager = BaseModelManager(connection_string)
+result = manager.get(example_id)
+result = manager.delete(example_id)
+```
+
+### Models
+Models use model managers
+```python
+class User(BaseDatabaseModel):
+    username: str
+    fname: str
+    lname: str
+    email: str
+    
+user = User(
+    username='johndoe',
+    fname='John',
+    lname='Doe',
+    email='john.doe@mail.com'
+)
+
+'''
+    Easy create, save, update and delete
+'''
+user = User(
+    username='johndoe',
+    fname='John',
+    lname='Doe',
+    email='john.doe@mail.com'
+)
+
+# saving the model
+user = user.save()
+
+# saving also updates the model
+user.lname = 'Joe'
+user = user.save()
+
+# getting a model by its ID from the database
+user = User.get(user_id)
+
+# deleting a model from the database
+deleted_user = user.delete()
+```
+
+### Tasks
+Tasks use models
+```python
+# in a program
+def my_func(a: int, b: int) -> int:
+  return a + b
+
+task = BaseTask(action=my_func)
+task.queue(a=8, b=3)
+
+###############
+# in a worker #
+task.digest() #
+###############
+
+# some time later
+result = task.result()
+```
+
+### Chain tasks
+Tasks can be chained together for larger workloads
+```python
+def double(number: int):
+    return {
+        'number': number * 2
+    }
+
+# make tasks
+one = BaseTask(action=double)
+two = BaseTask(action=double)
+three = BaseTask(action=double)
+
+# chain tasks
+two.set_parent(one)
+three.set_parent(two)
+
+# queue parent task
+one.queue(number=2)
+
+###############
+# in a worker #
+one.digest()  #
+###############
+
+# some time later
+result = one.result()
+assert result == 8, "Should be 8 as 2*2*2 == 8"
+```
+
+## Available functionality
+
+### Context managers
+- MongoContext
+- SQLite3Context
+
+
+### Model managers
+- MongoModelManager
+- SQLModelManager
+  - SQLQueryBuilder
+
+### Query filters
+- Datetime filter
+- Number filter
+- String filter
+
+### Models
+- BaseMongoModel
+- BaseRedisModel
+- BaseSQLModel
+
+### Tasks
+- RedisTask
+
+# Todo / in progress
+
+### Tasks
+- [ ] Chain tasks
+    - [x] Redis
+    - [ ] Mongo
+    - [ ] SQL
+- [ ] Task worker
+  	- [ ] Single Process
+    - [ ] Multi Process
+- [ ] RabbitMQ task
+
+# Tests
+
+Tests can be found in the `test` folder. They use pythons `unittest` and can be run with:
+```
+python3 -m unittest path/to/test.py
+```
+
+Tests get automatically run after each push.
+
+### Available tests
+- Mongo model
+- Mongo sorting
+- Redis task
+    - Basic functions
+    - Chaining
```

