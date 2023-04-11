# Comparing `tmp/codestructure-1.0.0.tar.gz` & `tmp/codestructure-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codestructure-1.0.0.tar", last modified: Mon Apr 10 19:46:09 2023, max compression
+gzip compressed data, was "codestructure-1.1.0.tar", last modified: Tue Apr 11 00:29:43 2023, max compression
```

## Comparing `codestructure-1.0.0.tar` & `codestructure-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-04-10 19:46:09.794740 codestructure-1.0.0/
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-04-10 19:46:09.753960 codestructure-1.0.0/.github/
--rw-r--r--   0 basnijholt   (501) staff       (20)     3677 2023-04-10 07:01:54.000000 codestructure-1.0.0/.github/release.py
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-04-10 19:46:09.762181 codestructure-1.0.0/.github/workflows/
--rw-r--r--   0 basnijholt   (501) staff       (20)      547 2023-04-10 19:09:29.000000 codestructure-1.0.0/.github/workflows/pytest.yml
--rw-r--r--   0 basnijholt   (501) staff       (20)     1421 2023-04-10 08:41:56.000000 codestructure-1.0.0/.github/workflows/release.yml
--rw-r--r--   0 basnijholt   (501) staff       (20)      196 2023-04-10 06:59:02.000000 codestructure-1.0.0/.github/workflows/toc.yaml
--rw-r--r--   0 basnijholt   (501) staff       (20)     1468 2023-04-10 06:59:02.000000 codestructure-1.0.0/.github/workflows/update-readme.yml
--rw-r--r--   0 basnijholt   (501) staff       (20)     3103 2023-04-10 06:59:02.000000 codestructure-1.0.0/.gitignore
--rw-r--r--   0 basnijholt   (501) staff       (20)      666 2023-04-10 06:59:00.000000 codestructure-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 basnijholt   (501) staff       (20)    11357 2023-04-10 06:59:00.000000 codestructure-1.0.0/LICENSE
--rw-r--r--   0 basnijholt   (501) staff       (20)     3878 2023-04-10 19:46:09.778200 codestructure-1.0.0/PKG-INFO
--rw-r--r--   0 basnijholt   (501) staff       (20)     3408 2023-04-10 19:42:28.000000 codestructure-1.0.0/README.md
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-04-10 19:46:09.771337 codestructure-1.0.0/codestructure.egg-info/
--rw-r--r--   0 basnijholt   (501) staff       (20)     3878 2023-04-10 19:46:09.000000 codestructure-1.0.0/codestructure.egg-info/PKG-INFO
--rw-r--r--   0 basnijholt   (501) staff       (20)      496 2023-04-10 19:46:09.000000 codestructure-1.0.0/codestructure.egg-info/SOURCES.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)        1 2023-04-10 19:46:09.000000 codestructure-1.0.0/codestructure.egg-info/dependency_links.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       53 2023-04-10 19:46:09.000000 codestructure-1.0.0/codestructure.egg-info/entry_points.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       90 2023-04-10 19:46:09.000000 codestructure-1.0.0/codestructure.egg-info/requires.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)       14 2023-04-10 19:46:09.000000 codestructure-1.0.0/codestructure.egg-info/top_level.txt
--rw-r--r--   0 basnijholt   (501) staff       (20)    10372 2023-04-10 19:06:29.000000 codestructure-1.0.0/codestructure.py
--rw-r--r--   0 basnijholt   (501) staff       (20)     2200 2023-04-10 18:27:12.000000 codestructure-1.0.0/pyproject.toml
--rw-r--r--   0 basnijholt   (501) staff       (20)       38 2023-04-10 19:46:09.794920 codestructure-1.0.0/setup.cfg
-drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-04-10 19:46:09.777517 codestructure-1.0.0/tests/
--rw-r--r--   0 basnijholt   (501) staff       (20)       54 2023-04-10 06:59:00.000000 codestructure-1.0.0/tests/__init__.py
--rw-r--r--   0 basnijholt   (501) staff       (20)    10480 2023-04-10 19:12:43.000000 codestructure-1.0.0/tests/test_code_structure.py
+drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-04-11 00:29:43.698689 codestructure-1.1.0/
+drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-04-11 00:29:43.628852 codestructure-1.1.0/.github/
+-rw-r--r--   0 basnijholt   (501) staff       (20)     3677 2023-04-10 07:01:54.000000 codestructure-1.1.0/.github/release.py
+drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-04-11 00:29:43.637653 codestructure-1.1.0/.github/workflows/
+-rw-r--r--   0 basnijholt   (501) staff       (20)      547 2023-04-10 19:09:29.000000 codestructure-1.1.0/.github/workflows/pytest.yml
+-rw-r--r--   0 basnijholt   (501) staff       (20)     1421 2023-04-10 08:41:56.000000 codestructure-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0 basnijholt   (501) staff       (20)      196 2023-04-10 06:59:02.000000 codestructure-1.1.0/.github/workflows/toc.yaml
+-rw-r--r--   0 basnijholt   (501) staff       (20)     1468 2023-04-10 06:59:02.000000 codestructure-1.1.0/.github/workflows/update-readme.yml
+-rw-r--r--   0 basnijholt   (501) staff       (20)     3103 2023-04-10 06:59:02.000000 codestructure-1.1.0/.gitignore
+-rw-r--r--   0 basnijholt   (501) staff       (20)      666 2023-04-10 06:59:00.000000 codestructure-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 basnijholt   (501) staff       (20)    11357 2023-04-10 06:59:00.000000 codestructure-1.1.0/LICENSE
+-rw-r--r--   0 basnijholt   (501) staff       (20)    18562 2023-04-11 00:29:43.697655 codestructure-1.1.0/PKG-INFO
+-rw-r--r--   0 basnijholt   (501) staff       (20)     5117 2023-04-11 00:20:34.000000 codestructure-1.1.0/README.md
+drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-04-11 00:29:43.663389 codestructure-1.1.0/codestructure.egg-info/
+-rw-r--r--   0 basnijholt   (501) staff       (20)    18562 2023-04-11 00:29:43.000000 codestructure-1.1.0/codestructure.egg-info/PKG-INFO
+-rw-r--r--   0 basnijholt   (501) staff       (20)      513 2023-04-11 00:29:43.000000 codestructure-1.1.0/codestructure.egg-info/SOURCES.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)        1 2023-04-11 00:29:43.000000 codestructure-1.1.0/codestructure.egg-info/dependency_links.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)       53 2023-04-11 00:29:43.000000 codestructure-1.1.0/codestructure.egg-info/entry_points.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)       90 2023-04-11 00:29:43.000000 codestructure-1.1.0/codestructure.egg-info/requires.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)       14 2023-04-11 00:29:43.000000 codestructure-1.1.0/codestructure.egg-info/top_level.txt
+-rw-r--r--   0 basnijholt   (501) staff       (20)    11282 2023-04-10 21:00:42.000000 codestructure-1.1.0/codestructure.py
+-rw-r--r--   0 basnijholt   (501) staff       (20)     2229 2023-04-11 00:27:55.000000 codestructure-1.1.0/pyproject.toml
+-rw-r--r--   0 basnijholt   (501) staff       (20)       38 2023-04-11 00:29:43.698766 codestructure-1.1.0/setup.cfg
+drwxr-xr-x   0 basnijholt   (501) staff       (20)        0 2023-04-11 00:29:43.695676 codestructure-1.1.0/tests/
+-rw-r--r--   0 basnijholt   (501) staff       (20)       54 2023-04-10 06:59:00.000000 codestructure-1.1.0/tests/__init__.py
+-rw-r--r--   0 basnijholt   (501) staff       (20)      354 2023-04-10 23:53:54.000000 codestructure-1.1.0/tests/example.py
+-rw-r--r--   0 basnijholt   (501) staff       (20)    13855 2023-04-10 23:48:23.000000 codestructure-1.1.0/tests/test_code_structure.py
```

### Comparing `codestructure-1.0.0/.github/release.py` & `codestructure-1.1.0/.github/release.py`

 * *Files identical despite different names*

### Comparing `codestructure-1.0.0/.github/workflows/pytest.yml` & `codestructure-1.1.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `codestructure-1.0.0/.github/workflows/release.yml` & `codestructure-1.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `codestructure-1.0.0/.github/workflows/update-readme.yml` & `codestructure-1.1.0/.github/workflows/update-readme.yml`

 * *Files identical despite different names*

### Comparing `codestructure-1.0.0/.gitignore` & `codestructure-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `codestructure-1.0.0/.pre-commit-config.yaml` & `codestructure-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `codestructure-1.0.0/LICENSE` & `codestructure-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codestructure-1.0.0/codestructure.py` & `codestructure-1.1.0/codestructure.py`

 * *Files 11% similar despite different names*

```diff
@@ -67,14 +67,16 @@
 @dataclass
 class Class:
     """A class."""
 
     class_name: str
     attributes: list[tuple[str, str | None]]
     functions: dict[str, Function] = field(default_factory=dict)
+    docstring: str | None = None
+    decorator: str | None = None
 
 
 @dataclass
 class ExtractedFunctions:
     """The information about classes and functions in a Python module."""
 
     classes: list[tuple[str, Class]] = field(default_factory=list)
@@ -108,15 +110,15 @@
                 isinstance(parent, ast.ClassDef) and parent.name == cls
                 for parent in node.parent_list  # type: ignore[attr-defined, union-attr]
             ):
                 return cls
         return None
 
     def get_decorator_name(
-        node: ast.FunctionDef | ast.AsyncFunctionDef,
+        node: ast.FunctionDef | ast.AsyncFunctionDef | ast.ClassDef,
     ) -> str | None:
         for decorator in node.decorator_list:
             if isinstance(decorator, ast.Name | ast.Attribute):
                 return ast.unparse(decorator)
         return None
 
     def get_parameters(
@@ -152,16 +154,26 @@
                 (
                     stmt.target.id,
                     ast.unparse(stmt.annotation) if stmt.annotation else None,
                 )
                 for stmt in node.body
                 if isinstance(stmt, ast.AnnAssign) and isinstance(stmt.target, ast.Name)
             ]
+            decorator_name = get_decorator_name(node)
+            class_docstring = ast.get_docstring(node)
             result.classes.append(
-                (node.name, Class(class_name=node.name, attributes=class_attributes)),
+                (
+                    node.name,
+                    Class(
+                        class_name=node.name,
+                        docstring=class_docstring,
+                        attributes=class_attributes,
+                        decorator=decorator_name,
+                    ),
+                ),
             )
 
         if isinstance(node, ast.FunctionDef | ast.AsyncFunctionDef):
             if any(
                 isinstance(parent, ast.FunctionDef | ast.AsyncFunctionDef)
                 for parent in node.parent_list  # type: ignore[union-attr]
             ):
@@ -237,22 +249,38 @@
             f'"""{function.docstring}"""' if function.docstring else "...",
             indent_docs,
         )
 
         return f"{decorator}{signature}\n{docstring}\n"
 
     for class_name, class_info in function_info.classes:
+        if class_info.decorator:
+            print(f"@{class_info.decorator}")
         print(f"class {class_name}:")
-        for attr_name, attr_type in class_info.attributes:
-            print(f"    {attr_name}: {attr_type}" if attr_type else f"    {attr_name}")
 
-        for method_name, method in class_info.functions.items():
-            if not with_private and _is_private(method_name):
-                continue
+        attrs = [
+            (attr_name, attr_type)
+            for attr_name, attr_type in class_info.attributes
+            if with_private or not _is_private(attr_name)
+        ]
+        methods = [
+            (method_name, method)
+            for method_name, method in class_info.functions.items()
+            if with_private or not _is_private(method_name)
+        ]
+
+        if class_info.docstring:
+            print(f'    """{class_info.docstring}"""')
+        elif not attrs and not methods:
+            print("    ...")
+
+        for attr_name, attr_type in attrs:
+            print(f"    {attr_name}: {attr_type}" if attr_type else f"    {attr_name}")
 
+        for _method_name, method in methods:
             print(format_function(method, 4))
         print()
 
     for function_name, function in function_info.functions:
         if not with_private and _is_private(function_name):
             continue
         print(format_function(function, 0))
```

### Comparing `codestructure-1.0.0/pyproject.toml` & `codestructure-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 name = "codestructure"
 description = "CodeStructure is a Python package that analyzes the structure of a Python file and extracts information about its classes, functions, and their associated attributes."
 dynamic = ["version"]
 authors = [{ name = "Bas Nijholt", email = "bas@nijho.lt" }]
 dependencies = ["pyperclip", "rich"]
 requires-python = ">=3.10"
 
+[project.license]
+file = "LICENSE"
+
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://github.com/basnijholt/codestructure"
 
@@ -60,15 +63,15 @@
     "PLW0603", # Using the global statement to update `X` is discouraged
     "D401",    # First line of docstring should be in imperative mood
     "SLF001",  # Private member accessed
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["SLF001"]
-"tests/test_examples.py" = ["E501"]
+"tests/example.py" = ["ALL"]
 ".github/*" = ["INP001"]
 
 [tool.ruff.mccabe]
 max-complexity = 18
 
 [tool.mypy]
 python_version = "3.10"
```

### Comparing `codestructure-1.0.0/tests/test_code_structure.py` & `codestructure-1.1.0/tests/test_code_structure.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """Test codestructure."""
 import ast
 import contextlib
 import textwrap
 from io import StringIO
+from pathlib import Path
 from unittest import mock
 
 from codestructure import (
     Class,
     ExtractedFunctions,
     Function,
     Parameter,
     add_parent_list,
     extract_function_info,
     main,
     parse_module,
     print_function_info,
 )
 
+REPO_ROOT = Path(__file__).parent.parent
+
 
 def test_parse_module() -> None:
     """Test parse_module."""
     source_code = textwrap.dedent(
         """
         def example_function():
             pass
@@ -350,7 +353,129 @@
         ],
     )
 
     tree = parse_module(source_code=source_code)
     function_info = extract_function_info(tree)
 
     assert function_info == expected_functions
+
+
+def test_print_function_info_with_class_docstring() -> None:
+    """Test print_function_info with a class that has a docstring."""
+    extracted_functions = ExtractedFunctions(
+        classes=[
+            (
+                "Foo",
+                Class(
+                    class_name="Foo",
+                    docstring="Some exception.",
+                    attributes=[],
+                    functions={},
+                ),
+            ),
+        ],
+        functions=[],
+    )
+
+    expected_output = textwrap.dedent(
+        """\
+        class Foo:
+            \"\"\"Some exception.\"\"\"
+        """,
+    )
+
+    with StringIO() as string, contextlib.redirect_stdout(string):
+        print_function_info(extracted_functions, with_private=True)
+        output = string.getvalue()
+
+    assert output.strip() == expected_output.strip()
+
+
+def test_print_function_info_with_class_attribute() -> None:
+    """Test print_function_info with a class that has an attribute."""
+    extracted_functions = ExtractedFunctions(
+        classes=[
+            (
+                "A",
+                Class(
+                    class_name="A",
+                    docstring=None,
+                    attributes=[("x", "int")],
+                    functions={},
+                    decorator="dataclass",
+                ),
+            ),
+        ],
+        functions=[],
+    )
+
+    expected_output = textwrap.dedent(
+        """
+        @dataclass
+        class A:
+            x: int
+        """,
+    )
+
+    with StringIO() as string, contextlib.redirect_stdout(string):
+        print_function_info(extracted_functions, with_private=True)
+        output = string.getvalue()
+
+    assert output.strip() == expected_output.strip()
+
+
+def test_print_function_info_with_private_class_attribute() -> None:
+    """Test print_function_info with a class that has a private attribute."""
+    extracted_functions = ExtractedFunctions(
+        classes=[
+            (
+                "A",
+                Class(
+                    class_name="A",
+                    docstring=None,
+                    attributes=[("_priv", "bool")],
+                    functions={},
+                ),
+            ),
+        ],
+        functions=[],
+    )
+
+    expected_output = textwrap.dedent(
+        """\
+        class A:
+            ...
+        """,
+    )
+
+    with StringIO() as string, contextlib.redirect_stdout(string):
+        print_function_info(extracted_functions, with_private=False)
+        output = string.getvalue()
+
+    assert output.strip() == expected_output.strip()
+
+
+def test_example_file() -> None:
+    """Test example file."""
+    test_file = REPO_ROOT / "tests" / "example.py"
+    with test_file.open() as f:
+        source_code = f.read()
+
+    tree = parse_module(source_code=source_code)
+    function_info = extract_function_info(tree)
+
+    with StringIO() as string, contextlib.redirect_stdout(string):
+        print_function_info(function_info, with_private=False)
+        output = string.getvalue()
+    expected = textwrap.dedent(
+        """
+        class MyClass:
+            my_attr: str
+            def my_method(self, arg1: int) -> bool:
+                \"\"\"My docstring.\"\"\"
+
+
+        def my_function(arg2: float) -> None:
+            ...
+        """,
+    )
+    assert output.strip() == expected.strip()
```

