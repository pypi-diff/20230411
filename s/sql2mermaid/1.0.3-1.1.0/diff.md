# Comparing `tmp/sql2mermaid-1.0.3.tar.gz` & `tmp/sql2mermaid-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql2mermaid-1.0.3.tar", max compression
+gzip compressed data, was "sql2mermaid-1.1.0.tar", max compression
```

## Comparing `sql2mermaid-1.0.3.tar` & `sql2mermaid-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1060 2023-04-04 11:16:22.644988 sql2mermaid-1.0.3/LICENSE.md
--rw-r--r--   0        0        0     1537 2023-04-07 18:27:39.373474 sql2mermaid-1.0.3/README.md
--rw-r--r--   0        0        0     1184 2023-04-07 18:27:39.383777 sql2mermaid-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       71 2023-04-07 18:27:39.384497 sql2mermaid-1.0.3/sql2mermaid/__init__.py
--rw-r--r--   0        0        0      496 2023-04-06 13:15:37.128373 sql2mermaid-1.0.3/sql2mermaid/dependencies.py
--rw-r--r--   0        0        0     3256 2023-04-07 16:38:18.111127 sql2mermaid-1.0.3/sql2mermaid/main.py
--rw-r--r--   0        0        0      597 2023-04-06 13:37:41.942630 sql2mermaid-1.0.3/sql2mermaid/tables.py
--rw-r--r--   0        0        0      313 2023-04-06 13:34:47.882454 sql2mermaid-1.0.3/sql2mermaid/utils.py
--rw-r--r--   0        0        0     2184 1970-01-01 00:00:00.000000 sql2mermaid-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-04 11:16:22.644988 sql2mermaid-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     1537 2023-04-07 18:27:39.373474 sql2mermaid-1.1.0/README.md
+-rw-r--r--   0        0        0     1184 2023-04-11 08:40:45.495251 sql2mermaid-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       71 2023-04-11 08:40:45.495766 sql2mermaid-1.1.0/sql2mermaid/__init__.py
+-rw-r--r--   0        0        0      496 2023-04-06 13:15:37.128373 sql2mermaid-1.1.0/sql2mermaid/dependencies.py
+-rw-r--r--   0        0        0     3277 2023-04-11 08:36:09.297910 sql2mermaid-1.1.0/sql2mermaid/main.py
+-rw-r--r--   0        0        0      597 2023-04-06 13:37:41.942630 sql2mermaid-1.1.0/sql2mermaid/tables.py
+-rw-r--r--   0        0        0      352 2023-04-11 08:36:09.298385 sql2mermaid-1.1.0/sql2mermaid/utils.py
+-rw-r--r--   0        0        0     2184 1970-01-01 00:00:00.000000 sql2mermaid-1.1.0/PKG-INFO
```

### Comparing `sql2mermaid-1.0.3/LICENSE.md` & `sql2mermaid-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sql2mermaid-1.0.3/README.md` & `sql2mermaid-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sql2mermaid-1.0.3/pyproject.toml` & `sql2mermaid-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql2mermaid"
-version = "1.0.3"
+version = "1.1.0"
 description = "Convert SQL table dependencies to mermaid.js"
 authors = ["nkato <naokato.aq@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/nkato/sql2mermaid"
 
 [tool.poetry.dependencies]
```

### Comparing `sql2mermaid-1.0.3/sql2mermaid/main.py` & `sql2mermaid-1.1.0/sql2mermaid/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             current_indent_level += 1
         elif token.value == ")":
             current_indent_level -= 1
         elif token.ttype is sqlparse.tokens.Name and current_indent_level == 0 and is_in_with:  # Sub table
             table_name = remove_quotes(token.value)
             tables.add(table_name)
             current_table = table_name
-        elif token.ttype is sqlparse.tokens.Keyword and is_pre_tables_mark(token.value):  # FROM or JOIN
+        elif token.ttype is sqlparse.tokens.Keyword and is_pre_tables_mark(token.value, parsed[i - 3].value):  # FROM or JOIN
             table_name = remove_quotes(parsed[i + 1].value)
             if not table_name == "(":
                 tables.add(table_name)
                 dep = Dependency(current_table, token.value, table_name)
                 if dep not in dependencies:
                     dependencies.add(dep)
         elif token.ttype is sqlparse.tokens.Keyword.DML and token.value.upper() == "SELECT" and current_indent_level == 0:
```

### Comparing `sql2mermaid-1.0.3/sql2mermaid/tables.py` & `sql2mermaid-1.1.0/sql2mermaid/tables.py`

 * *Files identical despite different names*

### Comparing `sql2mermaid-1.0.3/PKG-INFO` & `sql2mermaid-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql2mermaid
-Version: 1.0.3
+Version: 1.1.0
 Summary: Convert SQL table dependencies to mermaid.js
 Home-page: https://github.com/nkato/sql2mermaid
 License: MIT
 Author: nkato
 Author-email: naokato.aq@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

