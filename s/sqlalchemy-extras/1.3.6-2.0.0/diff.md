# Comparing `tmp/sqlalchemy_extras-1.3.6.tar.gz` & `tmp/sqlalchemy_extras-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_extras-1.3.6.tar", max compression
+gzip compressed data, was "sqlalchemy_extras-2.0.0.tar", max compression
```

## Comparing `sqlalchemy_extras-1.3.6.tar` & `sqlalchemy_extras-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-1.3.6/README.md
--rw-r--r--   0        0        0      829 2023-03-20 20:10:48.863206 sqlalchemy_extras-1.3.6/pyproject.toml
--rw-r--r--   0        0        0      183 2023-03-09 19:01:38.717890 sqlalchemy_extras-1.3.6/sqlalchemy_extras/__init__.py
--rw-r--r--   0        0        0     4518 2023-03-20 20:10:25.160405 sqlalchemy_extras-1.3.6/sqlalchemy_extras/fastapi.py
--rw-r--r--   0        0        0     3803 2023-03-09 18:34:58.457012 sqlalchemy_extras-1.3.6/sqlalchemy_extras/models.py
--rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-1.3.6/sqlalchemy_extras/py.typed
--rw-r--r--   0        0        0     2092 2023-03-09 18:34:58.457012 sqlalchemy_extras-1.3.6/sqlalchemy_extras/utils.py
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 sqlalchemy_extras-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.0/README.md
+-rw-r--r--   0        0        0      790 2023-04-11 17:49:09.114293 sqlalchemy_extras-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-03-09 19:01:38.717890 sqlalchemy_extras-2.0.0/sqlalchemy_extras/__init__.py
+-rw-r--r--   0        0        0     6662 2023-04-11 17:48:37.793160 sqlalchemy_extras-2.0.0/sqlalchemy_extras/fastapi.py
+-rw-r--r--   0        0        0     5349 2023-04-11 17:48:37.793160 sqlalchemy_extras-2.0.0/sqlalchemy_extras/models.py
+-rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.0/sqlalchemy_extras/py.typed
+-rw-r--r--   0        0        0     2092 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.0/sqlalchemy_extras/utils.py
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 sqlalchemy_extras-2.0.0/PKG-INFO
```

### Comparing `sqlalchemy_extras-1.3.6/pyproject.toml` & `sqlalchemy_extras-2.0.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [tool.poetry]
 authors = ["Francisco Del Roio <francipvb@hotmail.com>"]
 description = ""
 name = "sqlalchemy-extras"
 readme = "README.md"
-version = "1.3.6"
+version = "2.0.0"
 
 [tool.poetry.dependencies]
-SQLAlchemy = "^1.4.0"
-fastapi = {version = ">=0.60.0,<1.0.0", optional = true}
-python = "^3.8"
+sqlalchemy = "^2.0.9"
+fastapi = { version = ">=0.60.0,<1.0.0", optional = true }
+python = ">=3.10.0, <4"
 
 [tool.poetry.extras]
 fastapi = ["fastapi"]
 
-[tool.poetry.dev-dependencies]
-SQLAlchemy = {version = "^1.4.0", extras = ["mypy"]}
-autoflake = "^1.4"
+
+[tool.poetry.group.dev.dependencies]
+isort = "^5.12.0"
+autoflake = "^2.0.2"
 bandit = "^1.7.4"
-black = "^22.3.0"
-flake8 = "^4.0.1"
-mypy = "^0.950"
+black = "^23.1.0"
+flake8 = "^6.0.0"
 pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.0.0"
 pytest-sugar = "^0.9.4"
-fastapi = "^0.78.0"
-aiosqlite = "^0.17.0"
+fastapi = ">=0.80.0, <1.0.0"
+aiosqlite = "^0.18.0"
 requests = "^2.28.1"
-pytest-asyncio = "^0.18.3"
-
-[tool.poetry.group.dev.dependencies]
-isort = "^5.12.0"
+pytest-asyncio = "^0.21.0"
+httpx = "^0.23.3"
+ipykernel = "^6.22.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.isort]
 profile = "black"
```

### Comparing `sqlalchemy_extras-1.3.6/sqlalchemy_extras/utils.py` & `sqlalchemy_extras-2.0.0/sqlalchemy_extras/utils.py`

 * *Files identical despite different names*

