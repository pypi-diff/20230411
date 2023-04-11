# Comparing `tmp/pyloobins-0.1.0.tar.gz` & `tmp/pyloobins-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloobins-0.1.0.tar", max compression
+gzip compressed data, was "pyloobins-0.1.1.tar", max compression
```

## Comparing `pyloobins-0.1.0.tar` & `pyloobins-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0        0 2023-04-07 02:06:55.451802 pyloobins-0.1.0/LOOBins/.gitkeep
--rw-r--r--   0        0        0      332 2023-04-10 01:14:55.271338 pyloobins-0.1.0/README.md
--rw-r--r--   0        0        0      693 2023-04-10 01:39:32.686975 pyloobins-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.0/src/pyloobins/__init__.py
--rw-r--r--   0        0        0     1515 2023-04-10 01:37:23.987664 pyloobins-0.1.0/src/pyloobins/cli.py
--rw-r--r--   0        0        0     3618 2023-04-10 01:14:36.244757 pyloobins-0.1.0/src/pyloobins/models.py
--rw-r--r--   0        0        0     1055 2023-04-10 01:14:36.245041 pyloobins-0.1.0/src/pyloobins/templates/loobin.md.j2
--rw-r--r--   0        0        0     1981 2023-04-10 01:14:36.245196 pyloobins-0.1.0/src/pyloobins/util.py
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 pyloobins-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 00:56:15.923700 pyloobins-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-07 02:06:55.451802 pyloobins-0.1.1/LOOBins/.gitkeep
+-rw-r--r--   0        0        0      331 2023-04-11 00:56:15.923980 pyloobins-0.1.1/README.md
+-rw-r--r--   0        0        0      844 2023-04-11 00:56:33.886265 pyloobins-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.1/src/pyloobins/__init__.py
+-rw-r--r--   0        0        0     1498 2023-04-11 00:56:15.925235 pyloobins-0.1.1/src/pyloobins/cli.py
+-rw-r--r--   0        0        0     3582 2023-04-11 00:56:15.925856 pyloobins-0.1.1/src/pyloobins/models.py
+-rw-r--r--   0        0        0     1056 2023-04-11 00:56:15.926235 pyloobins-0.1.1/src/pyloobins/templates/loobin.md.j2
+-rw-r--r--   0        0        0     1965 2023-04-11 00:56:15.926520 pyloobins-0.1.1/src/pyloobins/util.py
+-rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 pyloobins-0.1.1/PKG-INFO
```

### Comparing `pyloobins-0.1.0/pyproject.toml` & `pyloobins-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 [tool.poetry]
 name = "PyLOOBins"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python package for managing the LOOBins model and schema."
 authors = ["infosecB <brendan@infosecb.com>"]
 readme = "README.md"
 packages = [{include = "pyloobins", from = "src"}]
-include = ["LOOBins"]
+include = ["LOOBins/*"]
+homepage = "https://loobins.io/"
+repository = "https://github.com/infosecB/LOOBins"
+keywords = ["cybersecurity", "cli", "lol"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.10.5"
 pyyaml = "^6.0"
 click = "^8.1.3"
 jinja2 = "^3.1.2"
 
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.0"
 black = "^23.1.0"
+pre-commit = "^3.2.2"
 
 [tool.poetry.scripts]
 pyloobins = 'pyloobins.cli:cli'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyloobins-0.1.0/src/pyloobins/cli.py` & `pyloobins-0.1.1/src/pyloobins/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Model for CLI functions"""
-import sys
 import os
+import sys
+
 import click
-from .util import validate_loobin, make_template, normalize_file_name
+
+from .util import make_template, normalize_file_name, validate_loobin
 
 
 @click.group()
 def cli():
     """Create, manage, and validate LOOBin objects."""
 
 
@@ -22,20 +24,15 @@
     if validate_loobin(yml_path=file):
         print(f"LOOBin at {file} is valid.")
     else:
         print(f"LOOBin at {file} is NOT valid.")
 
 
 @cli.command()
-@click.option(
-    "--name", 
-    type=str,
-    required=False,
-    help="Enter the name of the binary"
-)
+@click.option("--name", type=str, required=False, help="Enter the name of the binary")
 @click.option(
     "--path",
     type=str,
     required=False,
     help="Enter the path where you would like to create the template YAML file.",
 )
 def create_template(name: str, path: str) -> None:
```

### Comparing `pyloobins-0.1.0/src/pyloobins/models.py` & `pyloobins-0.1.1/src/pyloobins/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Model that represents a LOOBin and its various components"""
-from typing import List, Optional, Literal
 from datetime import date
-from pydantic import BaseModel, Field
+from typing import List, Literal, Optional
+
 import yaml
 from jinja2 import Environment, PackageLoader, select_autoescape
-
+from pydantic import BaseModel, Field
 
 AttackTactics = Literal[
     "Reconnaissance",
     "Resource Development",
     "Initial Access",
     "Execution",
     "Persistence",
@@ -59,34 +59,29 @@
         "This will display in the LOOBin card list and the LOOBins website search results.",
     )
     full_description: str = Field(
         title="Full Description",
         description="A full description of the LOOBin."
         "This will display on the LOOBin's single page.",
     )
-    created: date = Field(
-        title="Created", description="Date the LOOBin was created"
-    )
+    created: date = Field(title="Created", description="Date the LOOBin was created")
     example_use_cases: List[ExampleUseCase] = Field(
         title="Example Use Cases",
         description="A list of example use cases for the LOOBin",
     )
-    paths: List[str] = Field(
-        title="Paths", description="A list of paths to the LOOBin"
-    )
+    paths: List[str] = Field(title="Paths", description="A list of paths to the LOOBin")
     detections: List[Detection] = Field(
         title="Detections", description="A list of detections for the LOOBin"
     )
     resources: Optional[List[Resource]] = Field(
         title="Resource",
         description="A list of useful resources for the LOOBin",
     )
     acknowledgements: Optional[List[str]] = Field(
-        title="Acknowledgements",
-        description="Acknowledgements for the LOOBin"
+        title="Acknowledgements", description="Acknowledgements for the LOOBin"
     )
 
     def combine_tactics(self) -> List[str]:
         """Returns a list of all tactics across all LOOBin example use cases"""
         return [t for euc in self.example_use_cases for t in euc.tactics]  # type: ignore
 
     def combine_tags(self) -> List[str]:
```

### Comparing `pyloobins-0.1.0/src/pyloobins/templates/loobin.md.j2` & `pyloobins-0.1.1/src/pyloobins/templates/loobin.md.j2`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 {% for resource in loobin.resources %}
 - [{{ resource.name }}]({{ resource.url }})
 {% endfor %}
 
 # Acknowledgements
 {% for acknowledgement in loobin.acknowledgements %}
 - {{ acknowledgement }}
-{% endfor %}
+{% endfor %}
```

### Comparing `pyloobins-0.1.0/src/pyloobins/util.py` & `pyloobins-0.1.1/src/pyloobins/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """Utility functions that support the CLI and library"""
 from datetime import date
+
 import yaml
-from .models import (
-    LOOBin,
-    ExampleUseCase,
-    Detection,
-    Resource
-)
+
+from .models import Detection, ExampleUseCase, LOOBin, Resource
 
 
 def validate_loobin(yml_path: str) -> bool:
     """Validates LOOBin YAML file"""
     with open(yml_path, "r", encoding="utf-8") as stream:
         try:
             yml_content = yaml.safe_load(stream)
@@ -51,15 +48,15 @@
         ],
         resources=[
             Resource(
                 name="Name of resources.",
                 url="https://urlofexternalreference.here",
             )
         ],
-        acknowledgements=["Enter any acknowledgements here."]
+        acknowledgements=["Enter any acknowledgements here."],
     )
     return loobin_template
 
 
 def normalize_file_name(title: str) -> str:
     """Accepts a binary title and normalizes it for the file name"""
-    return title.lower().replace(" ", "_")
+    return title.lower().replace(" ", "_")
```

