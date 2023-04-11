# Comparing `tmp/olstecnologia-0.1.0.tar.gz` & `tmp/olstecnologia-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olstecnologia-0.1.0.tar", max compression
+gzip compressed data, was "olstecnologia-0.1.1.tar", max compression
```

## Comparing `olstecnologia-0.1.0.tar` & `olstecnologia-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-0.1.0/olstecnologia/__init__.py
--rw-r--r--   0        0        0      150 2023-04-11 13:11:04.581410 olstecnologia-0.1.0/olstecnologia/app.py
--rw-r--r--   0        0        0       26 2023-04-06 11:58:53.547641 olstecnologia-0.1.0/olstecnologia/config/__init__.py
--rw-r--r--   0        0        0     1799 2023-04-11 13:21:10.411176 olstecnologia-0.1.0/olstecnologia/config/database.py
--rw-r--r--   0        0        0      179 2023-04-10 17:58:30.917062 olstecnologia-0.1.0/olstecnologia/entities/__init__.py
--rw-r--r--   0        0        0      287 2023-04-10 17:56:32.173814 olstecnologia-0.1.0/olstecnologia/entities/bairro_entity.py
--rw-r--r--   0        0        0      132 2023-04-06 11:46:50.189344 olstecnologia-0.1.0/olstecnologia/entities/base_declative_entity.py
--rw-r--r--   0        0        0      323 2023-04-10 17:55:35.872698 olstecnologia-0.1.0/olstecnologia/entities/cidade_entity.py
--rw-r--r--   0        0        0      306 2023-04-10 17:56:13.452742 olstecnologia-0.1.0/olstecnologia/entities/logradouro_entity.py
--rw-r--r--   0        0        0     3254 2023-04-11 12:47:33.145374 olstecnologia-0.1.0/olstecnologia/entities/paciente_entity.py
--rw-r--r--   0        0        0      315 2023-04-10 17:59:00.227941 olstecnologia-0.1.0/olstecnologia/entities/rua_entity.py
--rw-r--r--   0        0        0       47 2023-04-11 11:19:34.706909 olstecnologia-0.1.0/olstecnologia/features/__int__.py
--rw-r--r--   0        0        0       48 2023-04-11 11:20:24.926916 olstecnologia-0.1.0/olstecnologia/features/atualiza_endereco/__init__.py
--rw-r--r--   0        0        0     2466 2023-04-11 14:16:37.240314 olstecnologia-0.1.0/olstecnologia/features/atualiza_endereco/atualiza_endereco.py
--rw-r--r--   0        0        0        0 2023-04-10 13:16:23.454502 olstecnologia-0.1.0/olstecnologia/services/__init__.py
--rw-r--r--   0        0        0      829 2023-04-11 13:34:43.232245 olstecnologia-0.1.0/olstecnologia/services/utils.py
--rw-r--r--   0        0        0      535 2023-04-11 14:16:19.258867 olstecnologia-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-0.1.0/README.md
--rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 olstecnologia-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-0.1.1/olstecnologia/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-11 14:42:19.577223 olstecnologia-0.1.1/olstecnologia/app.py
+-rw-r--r--   0        0        0       26 2023-04-06 11:58:53.547641 olstecnologia-0.1.1/olstecnologia/config/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-11 18:31:22.350517 olstecnologia-0.1.1/olstecnologia/config/database.py
+-rw-r--r--   0        0        0      179 2023-04-10 17:58:30.917062 olstecnologia-0.1.1/olstecnologia/entities/__init__.py
+-rw-r--r--   0        0        0      287 2023-04-10 17:56:32.173814 olstecnologia-0.1.1/olstecnologia/entities/bairro_entity.py
+-rw-r--r--   0        0        0      132 2023-04-06 11:46:50.189344 olstecnologia-0.1.1/olstecnologia/entities/base_declative_entity.py
+-rw-r--r--   0        0        0      323 2023-04-10 17:55:35.872698 olstecnologia-0.1.1/olstecnologia/entities/cidade_entity.py
+-rw-r--r--   0        0        0      306 2023-04-10 17:56:13.452742 olstecnologia-0.1.1/olstecnologia/entities/logradouro_entity.py
+-rw-r--r--   0        0        0     3254 2023-04-11 12:47:33.145374 olstecnologia-0.1.1/olstecnologia/entities/paciente_entity.py
+-rw-r--r--   0        0        0      315 2023-04-10 17:59:00.227941 olstecnologia-0.1.1/olstecnologia/entities/rua_entity.py
+-rw-r--r--   0        0        0       47 2023-04-11 11:19:34.706909 olstecnologia-0.1.1/olstecnologia/features/__int__.py
+-rw-r--r--   0        0        0       48 2023-04-11 18:19:03.436972 olstecnologia-0.1.1/olstecnologia/features/atualiza_endereco/__init__.py
+-rw-r--r--   0        0        0     3864 2023-04-11 18:30:45.661813 olstecnologia-0.1.1/olstecnologia/features/atualiza_endereco/atualiza_endereco.py
+-rw-r--r--   0        0        0        0 2023-04-10 13:16:23.454502 olstecnologia-0.1.1/olstecnologia/services/__init__.py
+-rw-r--r--   0        0        0      829 2023-04-11 13:34:43.232245 olstecnologia-0.1.1/olstecnologia/services/utils.py
+-rw-r--r--   0        0        0      535 2023-04-11 18:32:17.216819 olstecnologia-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 11:36:07.593080 olstecnologia-0.1.1/README.md
+-rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 olstecnologia-0.1.1/PKG-INFO
```

### Comparing `olstecnologia-0.1.0/olstecnologia/config/database.py` & `olstecnologia-0.1.1/olstecnologia/config/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from sqlalchemy import create_engine
-from sqlalchemy.engine.url import URL
 from sqlalchemy.orm import sessionmaker, Session
 from sqlalchemy import MetaData
-import urllib.parse
 from sqlalchemy import inspect
 from sqlalchemy import text
 
                       
 class Conn():
     def __init__(self, connect_string, **kwargs):
         self.connect_string = connect_string
```

### Comparing `olstecnologia-0.1.0/olstecnologia/entities/paciente_entity.py` & `olstecnologia-0.1.1/olstecnologia/entities/paciente_entity.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-0.1.0/olstecnologia/services/utils.py` & `olstecnologia-0.1.1/olstecnologia/services/utils.py`

 * *Files identical despite different names*

### Comparing `olstecnologia-0.1.0/pyproject.toml` & `olstecnologia-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olstecnologia"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Julio Pereira <juliopereira.dev@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 sqlalchemy = "^2.0.9"
```

