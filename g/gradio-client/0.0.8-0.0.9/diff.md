# Comparing `tmp/gradio_client-0.0.8.tar.gz` & `tmp/gradio_client-0.0.9.tar.gz`

## Comparing `gradio_client-0.0.8.tar` & `gradio_client-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 gradio_client-0.0.8/README.md
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 gradio_client-0.0.8/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.0.8/gradio_client/__init__.py
--rw-r--r--   0        0        0    33173 2020-02-02 00:00:00.000000 gradio_client-0.0.8/gradio_client/client.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 gradio_client-0.0.8/gradio_client/documentation.py
--rw-r--r--   0        0        0    11484 2020-02-02 00:00:00.000000 gradio_client-0.0.8/gradio_client/serializing.py
--rw-r--r--   0        0        0    10534 2020-02-02 00:00:00.000000 gradio_client-0.0.8/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.0.8/gradio_client/version.txt
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 gradio_client-0.0.8/.gitignore
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 gradio_client-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 gradio_client-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     7462 2020-02-02 00:00:00.000000 gradio_client-0.0.9/README.md
+-rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 gradio_client-0.0.9/requirements.txt
+-rwxr-xr-x   0        0        0      139 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/__init__.py
+-rwxr-xr-x   0        0        0    39444 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/client.py
+-rwxr-xr-x   0        0        0      443 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/data_classes.py
+-rwxr-xr-x   0        0        0    10765 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/documentation.py
+-rwxr-xr-x   0        0        0    14859 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/serializing.py
+-rwxr-xr-x   0        0        0    12276 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/utils.py
+-rwxr-xr-x   0        0        0        7 2020-02-02 00:00:00.000000 gradio_client-0.0.9/gradio_client/version.txt
+-rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 gradio_client-0.0.9/.gitignore
+-rwxr-xr-x   0        0        0     1418 2020-02-02 00:00:00.000000 gradio_client-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 gradio_client-0.0.9/PKG-INFO
```

### Comparing `gradio_client-0.0.8/README.md` & `gradio_client-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: gradio_client
+Version: 0.0.9
+Summary: Python library for easily interacting with trained machine learning models
+Project-URL: Homepage, https://github.com/gradio-app/gradio
+Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
+License-Expression: Apache-2.0
+Keywords: API,client,machine learning
+Requires-Python: >=3.7
+Requires-Dist: fsspec
+Requires-Dist: httpx
+Requires-Dist: huggingface-hub>=0.13.0
+Requires-Dist: packaging
+Requires-Dist: requests
+Requires-Dist: typing-extensions
+Requires-Dist: websockets
+Description-Content-Type: text/markdown
+
 # `gradio_client`: Use a Gradio app as an API -- in 3 lines of Python
 
 This directory contains the source code for `gradio_client`, a lightweight Python library that makes it very easy to use any Gradio app as an API. 
 
 As an example, consider this [Hugging Face Space that transcribes audio files](https://huggingface.co/spaces/abidlabs/whisper) that are recorded from the microphone.
 
 ![](https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/gradio-guides/whisper-screenshot.jpg)
```

### Comparing `gradio_client-0.0.8/gradio_client/documentation.py` & `gradio_client-0.0.9/gradio_client/documentation.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,266 +1,266 @@
-"""Contains methods that generate documentation for Gradio functions and classes."""
-
-from __future__ import annotations
-
-import inspect
-from typing import Callable, Dict, List, Tuple
-
-classes_to_document = {}
-classes_inherit_documentation = {}
-documentation_group = None
-
-
-def set_documentation_group(m):
-    global documentation_group
-    documentation_group = m
-    if m not in classes_to_document:
-        classes_to_document[m] = []
-
-
-def extract_instance_attr_doc(cls, attr):
-    code = inspect.getsource(cls.__init__)
-    lines = [line.strip() for line in code.split("\n")]
-    i = None
-    for i, line in enumerate(lines):
-        if line.startswith("self." + attr + ":") or line.startswith(
-            "self." + attr + " ="
-        ):
-            break
-    assert i is not None, f"Could not find {attr} in {cls.__name__}"
-    start_line = lines.index('"""', i)
-    end_line = lines.index('"""', start_line + 1)
-    for j in range(i + 1, start_line):
-        assert not lines[j].startswith("self."), (
-            f"Found another attribute before docstring for {attr} in {cls.__name__}: "
-            + lines[j]
-            + "\n start:"
-            + lines[i]
-        )
-    doc_string = " ".join(lines[start_line + 1 : end_line])
-    return doc_string
-
-
-def document(*fns, inherit=False):
-    """
-    Defines the @document decorator which adds classes or functions to the Gradio
-    documentation at www.gradio.app/docs.
-
-    Usage examples:
-    - Put @document() above a class to document the class and its constructor.
-    - Put @document("fn1", "fn2") above a class to also document methods fn1 and fn2.
-    - Put @document("*fn3") with an asterisk above a class to document the instance attribute methods f3.
-    """
-
-    def inner_doc(cls):
-        global documentation_group
-        if inherit:
-            classes_inherit_documentation[cls] = None
-        classes_to_document[documentation_group].append((cls, fns))
-        return cls
-
-    return inner_doc
-
-
-def document_fn(fn: Callable, cls) -> Tuple[str, List[Dict], Dict, str | None]:
-    """
-    Generates documentation for any function.
-    Parameters:
-        fn: Function to document
-    Returns:
-        description: General description of fn
-        parameters: A list of dicts for each parameter, storing data for the parameter name, annotation and doc
-        return: A dict storing data for the returned annotation and doc
-        example: Code for an example use of the fn
-    """
-    doc_str = inspect.getdoc(fn) or ""
-    doc_lines = doc_str.split("\n")
-    signature = inspect.signature(fn)
-    description, parameters, returns, examples = [], {}, [], []
-    mode = "description"
-    for line in doc_lines:
-        line = line.rstrip()
-        if line == "Parameters:":
-            mode = "parameter"
-        elif line.startswith("Example:"):
-            mode = "example"
-            if "(" in line and ")" in line:
-                c = line.split("(")[1].split(")")[0]
-                if c != cls.__name__:
-                    mode = "ignore"
-        elif line == "Returns:":
-            mode = "return"
-        else:
-            if mode == "description":
-                description.append(line if line.strip() else "<br>")
-                continue
-            if not (line.startswith("    ") or line.strip() == ""):
-                print(line)
-            assert (
-                line.startswith("    ") or line.strip() == ""
-            ), f"Documentation format for {fn.__name__} has format error in line: {line}"
-            line = line[4:]
-            if mode == "parameter":
-                colon_index = line.index(": ")
-                assert (
-                    colon_index > -1
-                ), f"Documentation format for {fn.__name__} has format error in line: {line}"
-                parameter = line[:colon_index]
-                parameter_doc = line[colon_index + 2 :]
-                parameters[parameter] = parameter_doc
-            elif mode == "return":
-                returns.append(line)
-            elif mode == "example":
-                examples.append(line)
-    description_doc = " ".join(description)
-    parameter_docs = []
-    for param_name, param in signature.parameters.items():
-        if param_name.startswith("_"):
-            continue
-        if param_name in ["kwargs", "args"] and param_name not in parameters:
-            continue
-        parameter_doc = {
-            "name": param_name,
-            "annotation": param.annotation,
-            "doc": parameters.get(param_name),
-        }
-        if param_name in parameters:
-            del parameters[param_name]
-        if param.default != inspect.Parameter.empty:
-            default = param.default
-            if type(default) == str:
-                default = '"' + default + '"'
-            if default.__class__.__module__ != "builtins":
-                default = f"{default.__class__.__name__}()"
-            parameter_doc["default"] = default
-        elif parameter_doc["doc"] is not None:
-            if "kwargs" in parameter_doc["doc"]:
-                parameter_doc["kwargs"] = True
-            if "args" in parameter_doc["doc"]:
-                parameter_doc["args"] = True
-        parameter_docs.append(parameter_doc)
-    assert (
-        len(parameters) == 0
-    ), f"Documentation format for {fn.__name__} documents nonexistent parameters: {''.join(parameters.keys())}"
-    if len(returns) == 0:
-        return_docs = {}
-    elif len(returns) == 1:
-        return_docs = {"annotation": signature.return_annotation, "doc": returns[0]}
-    else:
-        return_docs = {}
-        # raise ValueError("Does not support multiple returns yet.")
-    examples_doc = "\n".join(examples) if len(examples) > 0 else None
-    return description_doc, parameter_docs, return_docs, examples_doc
-
-
-def document_cls(cls):
-    doc_str = inspect.getdoc(cls)
-    if doc_str is None:
-        return "", {}, ""
-    tags = {}
-    description_lines = []
-    mode = "description"
-    for line in doc_str.split("\n"):
-        line = line.rstrip()
-        if line.endswith(":") and " " not in line:
-            mode = line[:-1].lower()
-            tags[mode] = []
-        elif line.split(" ")[0].endswith(":") and not line.startswith("    "):
-            tag = line[: line.index(":")].lower()
-            value = line[line.index(":") + 2 :]
-            tags[tag] = value
-        else:
-            if mode == "description":
-                description_lines.append(line if line.strip() else "<br>")
-            else:
-                assert (
-                    line.startswith("    ") or not line.strip()
-                ), f"Documentation format for {cls.__name__} has format error in line: {line}"
-                tags[mode].append(line[4:])
-    if "example" in tags:
-        example = "\n".join(tags["example"])
-        del tags["example"]
-    else:
-        example = None
-    for key, val in tags.items():
-        if isinstance(val, list):
-            tags[key] = "<br>".join(val)
-    description = " ".join(description_lines).replace("\n", "<br>")
-    return description, tags, example
-
-
-def generate_documentation():
-    documentation = {}
-    for mode, class_list in classes_to_document.items():
-        documentation[mode] = []
-        for cls, fns in class_list:
-            fn_to_document = cls if inspect.isfunction(cls) else cls.__init__
-            _, parameter_doc, return_doc, _ = document_fn(fn_to_document, cls)
-            cls_description, cls_tags, cls_example = document_cls(cls)
-            cls_documentation = {
-                "class": cls,
-                "name": cls.__name__,
-                "description": cls_description,
-                "tags": cls_tags,
-                "parameters": parameter_doc,
-                "returns": return_doc,
-                "example": cls_example,
-                "fns": [],
-            }
-            for fn_name in fns:
-                instance_attribute_fn = fn_name.startswith("*")
-                if instance_attribute_fn:
-                    fn_name = fn_name[1:]
-                    # Instance attribute fns are classes
-                    # whose __call__ method determines their behavior
-                    fn = getattr(cls(), fn_name).__call__
-                else:
-                    fn = getattr(cls, fn_name)
-                if not callable(fn):
-                    description_doc = str(fn)
-                    parameter_docs = {}
-                    return_docs = {}
-                    examples_doc = ""
-                    override_signature = f"gr.{cls.__name__}.{fn_name}"
-                else:
-                    (
-                        description_doc,
-                        parameter_docs,
-                        return_docs,
-                        examples_doc,
-                    ) = document_fn(fn, cls)
-                    override_signature = None
-                if instance_attribute_fn:
-                    description_doc = extract_instance_attr_doc(cls, fn_name)
-                cls_documentation["fns"].append(
-                    {
-                        "fn": fn,
-                        "name": fn_name,
-                        "description": description_doc,
-                        "tags": {},
-                        "parameters": parameter_docs,
-                        "returns": return_docs,
-                        "example": examples_doc,
-                        "override_signature": override_signature,
-                    }
-                )
-            documentation[mode].append(cls_documentation)
-            if cls in classes_inherit_documentation:
-                classes_inherit_documentation[cls] = cls_documentation["fns"]
-    for mode, class_list in classes_to_document.items():
-        for i, (cls, _) in enumerate(class_list):
-            for super_class in classes_inherit_documentation:
-                if (
-                    inspect.isclass(cls)
-                    and issubclass(cls, super_class)
-                    and cls != super_class
-                ):
-                    for inherited_fn in classes_inherit_documentation[super_class]:
-                        inherited_fn = dict(inherited_fn)
-                        try:
-                            inherited_fn["description"] = extract_instance_attr_doc(
-                                cls, inherited_fn["name"]
-                            )
-                        except (ValueError, AssertionError):
-                            pass
-                        documentation[mode][i]["fns"].append(inherited_fn)
-    return documentation
+"""Contains methods that generate documentation for Gradio functions and classes."""
+
+from __future__ import annotations
+
+import inspect
+from typing import Callable, Dict, List, Tuple
+
+classes_to_document = {}
+classes_inherit_documentation = {}
+documentation_group = None
+
+
+def set_documentation_group(m):
+    global documentation_group
+    documentation_group = m
+    if m not in classes_to_document:
+        classes_to_document[m] = []
+
+
+def extract_instance_attr_doc(cls, attr):
+    code = inspect.getsource(cls.__init__)
+    lines = [line.strip() for line in code.split("\n")]
+    i = None
+    for i, line in enumerate(lines):
+        if line.startswith("self." + attr + ":") or line.startswith(
+            "self." + attr + " ="
+        ):
+            break
+    assert i is not None, f"Could not find {attr} in {cls.__name__}"
+    start_line = lines.index('"""', i)
+    end_line = lines.index('"""', start_line + 1)
+    for j in range(i + 1, start_line):
+        assert not lines[j].startswith("self."), (
+            f"Found another attribute before docstring for {attr} in {cls.__name__}: "
+            + lines[j]
+            + "\n start:"
+            + lines[i]
+        )
+    doc_string = " ".join(lines[start_line + 1 : end_line])
+    return doc_string
+
+
+def document(*fns, inherit=False):
+    """
+    Defines the @document decorator which adds classes or functions to the Gradio
+    documentation at www.gradio.app/docs.
+
+    Usage examples:
+    - Put @document() above a class to document the class and its constructor.
+    - Put @document("fn1", "fn2") above a class to also document methods fn1 and fn2.
+    - Put @document("*fn3") with an asterisk above a class to document the instance attribute methods f3.
+    """
+
+    def inner_doc(cls):
+        global documentation_group
+        if inherit:
+            classes_inherit_documentation[cls] = None
+        classes_to_document[documentation_group].append((cls, fns))
+        return cls
+
+    return inner_doc
+
+
+def document_fn(fn: Callable, cls) -> Tuple[str, List[Dict], Dict, str | None]:
+    """
+    Generates documentation for any function.
+    Parameters:
+        fn: Function to document
+    Returns:
+        description: General description of fn
+        parameters: A list of dicts for each parameter, storing data for the parameter name, annotation and doc
+        return: A dict storing data for the returned annotation and doc
+        example: Code for an example use of the fn
+    """
+    doc_str = inspect.getdoc(fn) or ""
+    doc_lines = doc_str.split("\n")
+    signature = inspect.signature(fn)
+    description, parameters, returns, examples = [], {}, [], []
+    mode = "description"
+    for line in doc_lines:
+        line = line.rstrip()
+        if line == "Parameters:":
+            mode = "parameter"
+        elif line.startswith("Example:"):
+            mode = "example"
+            if "(" in line and ")" in line:
+                c = line.split("(")[1].split(")")[0]
+                if c != cls.__name__:
+                    mode = "ignore"
+        elif line == "Returns:":
+            mode = "return"
+        else:
+            if mode == "description":
+                description.append(line if line.strip() else "<br>")
+                continue
+            if not (line.startswith("    ") or line.strip() == ""):
+                print(line)
+            assert (
+                line.startswith("    ") or line.strip() == ""
+            ), f"Documentation format for {fn.__name__} has format error in line: {line}"
+            line = line[4:]
+            if mode == "parameter":
+                colon_index = line.index(": ")
+                assert (
+                    colon_index > -1
+                ), f"Documentation format for {fn.__name__} has format error in line: {line}"
+                parameter = line[:colon_index]
+                parameter_doc = line[colon_index + 2 :]
+                parameters[parameter] = parameter_doc
+            elif mode == "return":
+                returns.append(line)
+            elif mode == "example":
+                examples.append(line)
+    description_doc = " ".join(description)
+    parameter_docs = []
+    for param_name, param in signature.parameters.items():
+        if param_name.startswith("_"):
+            continue
+        if param_name in ["kwargs", "args"] and param_name not in parameters:
+            continue
+        parameter_doc = {
+            "name": param_name,
+            "annotation": param.annotation,
+            "doc": parameters.get(param_name),
+        }
+        if param_name in parameters:
+            del parameters[param_name]
+        if param.default != inspect.Parameter.empty:
+            default = param.default
+            if type(default) == str:
+                default = '"' + default + '"'
+            if default.__class__.__module__ != "builtins":
+                default = f"{default.__class__.__name__}()"
+            parameter_doc["default"] = default
+        elif parameter_doc["doc"] is not None:
+            if "kwargs" in parameter_doc["doc"]:
+                parameter_doc["kwargs"] = True
+            if "args" in parameter_doc["doc"]:
+                parameter_doc["args"] = True
+        parameter_docs.append(parameter_doc)
+    assert (
+        len(parameters) == 0
+    ), f"Documentation format for {fn.__name__} documents nonexistent parameters: {''.join(parameters.keys())}"
+    if len(returns) == 0:
+        return_docs = {}
+    elif len(returns) == 1:
+        return_docs = {"annotation": signature.return_annotation, "doc": returns[0]}
+    else:
+        return_docs = {}
+        # raise ValueError("Does not support multiple returns yet.")
+    examples_doc = "\n".join(examples) if len(examples) > 0 else None
+    return description_doc, parameter_docs, return_docs, examples_doc
+
+
+def document_cls(cls):
+    doc_str = inspect.getdoc(cls)
+    if doc_str is None:
+        return "", {}, ""
+    tags = {}
+    description_lines = []
+    mode = "description"
+    for line in doc_str.split("\n"):
+        line = line.rstrip()
+        if line.endswith(":") and " " not in line:
+            mode = line[:-1].lower()
+            tags[mode] = []
+        elif line.split(" ")[0].endswith(":") and not line.startswith("    "):
+            tag = line[: line.index(":")].lower()
+            value = line[line.index(":") + 2 :]
+            tags[tag] = value
+        else:
+            if mode == "description":
+                description_lines.append(line if line.strip() else "<br>")
+            else:
+                assert (
+                    line.startswith("    ") or not line.strip()
+                ), f"Documentation format for {cls.__name__} has format error in line: {line}"
+                tags[mode].append(line[4:])
+    if "example" in tags:
+        example = "\n".join(tags["example"])
+        del tags["example"]
+    else:
+        example = None
+    for key, val in tags.items():
+        if isinstance(val, list):
+            tags[key] = "<br>".join(val)
+    description = " ".join(description_lines).replace("\n", "<br>")
+    return description, tags, example
+
+
+def generate_documentation():
+    documentation = {}
+    for mode, class_list in classes_to_document.items():
+        documentation[mode] = []
+        for cls, fns in class_list:
+            fn_to_document = cls if inspect.isfunction(cls) else cls.__init__
+            _, parameter_doc, return_doc, _ = document_fn(fn_to_document, cls)
+            cls_description, cls_tags, cls_example = document_cls(cls)
+            cls_documentation = {
+                "class": cls,
+                "name": cls.__name__,
+                "description": cls_description,
+                "tags": cls_tags,
+                "parameters": parameter_doc,
+                "returns": return_doc,
+                "example": cls_example,
+                "fns": [],
+            }
+            for fn_name in fns:
+                instance_attribute_fn = fn_name.startswith("*")
+                if instance_attribute_fn:
+                    fn_name = fn_name[1:]
+                    # Instance attribute fns are classes
+                    # whose __call__ method determines their behavior
+                    fn = getattr(cls(), fn_name).__call__
+                else:
+                    fn = getattr(cls, fn_name)
+                if not callable(fn):
+                    description_doc = str(fn)
+                    parameter_docs = {}
+                    return_docs = {}
+                    examples_doc = ""
+                    override_signature = f"gr.{cls.__name__}.{fn_name}"
+                else:
+                    (
+                        description_doc,
+                        parameter_docs,
+                        return_docs,
+                        examples_doc,
+                    ) = document_fn(fn, cls)
+                    override_signature = None
+                if instance_attribute_fn:
+                    description_doc = extract_instance_attr_doc(cls, fn_name)
+                cls_documentation["fns"].append(
+                    {
+                        "fn": fn,
+                        "name": fn_name,
+                        "description": description_doc,
+                        "tags": {},
+                        "parameters": parameter_docs,
+                        "returns": return_docs,
+                        "example": examples_doc,
+                        "override_signature": override_signature,
+                    }
+                )
+            documentation[mode].append(cls_documentation)
+            if cls in classes_inherit_documentation:
+                classes_inherit_documentation[cls] = cls_documentation["fns"]
+    for mode, class_list in classes_to_document.items():
+        for i, (cls, _) in enumerate(class_list):
+            for super_class in classes_inherit_documentation:
+                if (
+                    inspect.isclass(cls)
+                    and issubclass(cls, super_class)
+                    and cls != super_class
+                ):
+                    for inherited_fn in classes_inherit_documentation[super_class]:
+                        inherited_fn = dict(inherited_fn)
+                        try:
+                            inherited_fn["description"] = extract_instance_attr_doc(
+                                cls, inherited_fn["name"]
+                            )
+                        except (ValueError, AssertionError):
+                            pass
+                        documentation[mode][i]["fns"].append(inherited_fn)
+    return documentation
```

### Comparing `gradio_client-0.0.8/gradio_client/utils.py` & `gradio_client-0.0.9/gradio_client/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,367 +1,397 @@
-from __future__ import annotations
-
-import base64
-import json
-import mimetypes
-import os
-import pkgutil
-import shutil
-import tempfile
-from dataclasses import dataclass, field
-from datetime import datetime
-from enum import Enum
-from pathlib import Path
-from threading import Lock
-from typing import Any, Callable, Dict, List, Tuple
-
-import fsspec.asyn
-import requests
-from websockets.legacy.protocol import WebSocketCommonProtocol
-
-API_URL = "{}/api/predict/"
-WS_URL = "{}/queue/join"
-STATE_COMPONENT = "state"
-
-__version__ = (pkgutil.get_data(__name__, "version.txt") or b"").decode("ascii").strip()
-
-
-class TooManyRequestsError(Exception):
-    """Raised when the API returns a 429 status code."""
-
-    pass
-
-
-class QueueError(Exception):
-    """Raised when the queue is full or there is an issue adding a job to the queue."""
-
-    pass
-
-
-class InvalidAPIEndpointError(Exception):
-    """Raised when the API endpoint is invalid."""
-
-    pass
-
-
-class Status(Enum):
-    """Status codes presented to client users."""
-
-    STARTING = "STARTING"
-    JOINING_QUEUE = "JOINING_QUEUE"
-    QUEUE_FULL = "QUEUE_FULL"
-    IN_QUEUE = "IN_QUEUE"
-    SENDING_DATA = "SENDING_DATA"
-    PROCESSING = "PROCESSSING"
-    ITERATING = "ITERATING"
-    FINISHED = "FINISHED"
-
-    @staticmethod
-    def ordering(status: "Status") -> int:
-        """Order of messages. Helpful for testing."""
-        order = [
-            Status.STARTING,
-            Status.JOINING_QUEUE,
-            Status.QUEUE_FULL,
-            Status.IN_QUEUE,
-            Status.SENDING_DATA,
-            Status.PROCESSING,
-            Status.ITERATING,
-            Status.FINISHED,
-        ]
-        return order.index(status)
-
-    def __lt__(self, other: "Status"):
-        return self.ordering(self) < self.ordering(other)
-
-    @staticmethod
-    def msg_to_status(msg: str) -> "Status":
-        """Map the raw message from the backend to the status code presented to users."""
-        return {
-            "send_hash": Status.JOINING_QUEUE,
-            "queue_full": Status.QUEUE_FULL,
-            "estimation": Status.IN_QUEUE,
-            "send_data": Status.SENDING_DATA,
-            "process_starts": Status.PROCESSING,
-            "process_generating": Status.ITERATING,
-            "process_completed": Status.FINISHED,
-        }[msg]
-
-
-@dataclass
-class StatusUpdate:
-    """Update message sent from the worker thread to the Job on the main thread."""
-
-    code: Status
-    rank: int | None
-    queue_size: int | None
-    eta: float | None
-    success: bool | None
-    time: datetime | None
-
-
-def create_initial_status_update():
-    return StatusUpdate(
-        code=Status.STARTING,
-        rank=None,
-        queue_size=None,
-        eta=None,
-        success=None,
-        time=datetime.now(),
-    )
-
-
-@dataclass
-class JobStatus:
-    """The job status.
-
-    Keeps strack of the latest status update and intermediate outputs (not yet implements).
-    """
-
-    latest_status: StatusUpdate = field(default_factory=create_initial_status_update)
-    outputs: List[Any] = field(default_factory=list)
-
-
-@dataclass
-class Communicator:
-    """Helper class to help communicate between the worker thread and main thread."""
-
-    lock: Lock
-    job: JobStatus
-    deserialize: Callable[..., Tuple]
-
-
-########################
-# Network utils
-########################
-
-
-def is_valid_url(possible_url: str) -> bool:
-    headers = {"User-Agent": "gradio (https://gradio.app/; team@gradio.app)"}
-    try:
-        head_request = requests.head(possible_url, headers=headers)
-        if head_request.status_code == 405:
-            return requests.get(possible_url, headers=headers).ok
-        return head_request.ok
-    except Exception:
-        return False
-
-
-async def get_pred_from_ws(
-    websocket: WebSocketCommonProtocol,
-    data: str,
-    hash_data: str,
-    helper: Communicator | None = None,
-) -> Dict[str, Any]:
-    completed = False
-    resp = {}
-    while not completed:
-        msg = await websocket.recv()
-        resp = json.loads(msg)
-        if helper:
-            with helper.lock:
-                status_update = StatusUpdate(
-                    code=Status.msg_to_status(resp["msg"]),
-                    queue_size=resp.get("queue_size"),
-                    rank=resp.get("rank", None),
-                    success=resp.get("success"),
-                    time=datetime.now(),
-                    eta=resp.get("rank_eta"),
-                )
-                output = resp.get("output", {}).get("data", [])
-                if output and status_update.code != Status.FINISHED:
-                    try:
-                        result = helper.deserialize(*output)
-                    except Exception as e:
-                        result = [e]
-                    helper.job.outputs.append(result)
-                helper.job.latest_status = status_update
-        if resp["msg"] == "queue_full":
-            raise QueueError("Queue is full! Please try again.")
-        if resp["msg"] == "send_hash":
-            await websocket.send(hash_data)
-        elif resp["msg"] == "send_data":
-            await websocket.send(data)
-        completed = resp["msg"] == "process_completed"
-    return resp["output"]
-
-
-########################
-# Data processing utils
-########################
-
-
-def download_tmp_copy_of_file(
-    url_path: str, hf_token: str | None = None, dir: str | None = None
-) -> tempfile._TemporaryFileWrapper:
-    if dir is not None:
-        os.makedirs(dir, exist_ok=True)
-    headers = {"Authorization": "Bearer " + hf_token} if hf_token else {}
-    prefix = Path(url_path).stem
-    suffix = Path(url_path).suffix
-    file_obj = tempfile.NamedTemporaryFile(
-        delete=False,
-        prefix=prefix,
-        suffix=suffix,
-        dir=dir,
-    )
-    with requests.get(url_path, headers=headers, stream=True) as r:
-        with open(file_obj.name, "wb") as f:
-            shutil.copyfileobj(r.raw, f)
-    return file_obj
-
-
-def create_tmp_copy_of_file(
-    file_path: str, dir: str | None = None
-) -> tempfile._TemporaryFileWrapper:
-    if dir is not None:
-        os.makedirs(dir, exist_ok=True)
-    prefix = Path(file_path).stem
-    suffix = Path(file_path).suffix
-    file_obj = tempfile.NamedTemporaryFile(
-        delete=False,
-        prefix=prefix,
-        suffix=suffix,
-        dir=dir,
-    )
-    shutil.copy2(file_path, file_obj.name)
-    return file_obj
-
-
-def get_mimetype(filename: str) -> str | None:
-    mimetype = mimetypes.guess_type(filename)[0]
-    if mimetype is not None:
-        mimetype = mimetype.replace("x-wav", "wav").replace("x-flac", "flac")
-    return mimetype
-
-
-def get_extension(encoding: str) -> str | None:
-    encoding = encoding.replace("audio/wav", "audio/x-wav")
-    type = mimetypes.guess_type(encoding)[0]
-    if type == "audio/flac":  # flac is not supported by mimetypes
-        return "flac"
-    elif type is None:
-        return None
-    extension = mimetypes.guess_extension(type)
-    if extension is not None and extension.startswith("."):
-        extension = extension[1:]
-    return extension
-
-
-def encode_file_to_base64(f):
-    with open(f, "rb") as file:
-        encoded_string = base64.b64encode(file.read())
-        base64_str = str(encoded_string, "utf-8")
-        mimetype = get_mimetype(f)
-        return (
-            "data:"
-            + (mimetype if mimetype is not None else "")
-            + ";base64,"
-            + base64_str
-        )
-
-
-def encode_url_to_base64(url):
-    encoded_string = base64.b64encode(requests.get(url).content)
-    base64_str = str(encoded_string, "utf-8")
-    mimetype = get_mimetype(url)
-    return (
-        "data:" + (mimetype if mimetype is not None else "") + ";base64," + base64_str
-    )
-
-
-def encode_url_or_file_to_base64(path: str | Path):
-    path = str(path)
-    if is_valid_url(path):
-        return encode_url_to_base64(path)
-    else:
-        return encode_file_to_base64(path)
-
-
-def decode_base64_to_binary(encoding) -> Tuple[bytes, str | None]:
-    extension = get_extension(encoding)
-    try:
-        data = encoding.split(",")[1]
-    except IndexError:
-        data = ""
-    return base64.b64decode(data), extension
-
-
-def strip_invalid_filename_characters(filename: str, max_bytes: int = 200) -> str:
-    """Strips invalid characters from a filename and ensures that the file_length is less than `max_bytes` bytes."""
-    filename = "".join([char for char in filename if char.isalnum() or char in "._- "])
-    filename_len = len(filename.encode())
-    if filename_len > max_bytes:
-        while filename_len > max_bytes:
-            if len(filename) == 0:
-                break
-            filename = filename[:-1]
-            filename_len = len(filename.encode())
-    return filename
-
-
-def decode_base64_to_file(encoding, file_path=None, dir=None, prefix=None):
-    if dir is not None:
-        os.makedirs(dir, exist_ok=True)
-    data, extension = decode_base64_to_binary(encoding)
-    if file_path is not None and prefix is None:
-        filename = Path(file_path).name
-        prefix = filename
-        if "." in filename:
-            prefix = filename[0 : filename.index(".")]
-            extension = filename[filename.index(".") + 1 :]
-
-    if prefix is not None:
-        prefix = strip_invalid_filename_characters(prefix)
-
-    if extension is None:
-        file_obj = tempfile.NamedTemporaryFile(delete=False, prefix=prefix, dir=dir)
-    else:
-        file_obj = tempfile.NamedTemporaryFile(
-            delete=False,
-            prefix=prefix,
-            suffix="." + extension,
-            dir=dir,
-        )
-    file_obj.write(data)
-    file_obj.flush()
-    return file_obj
-
-
-def dict_or_str_to_json_file(jsn, dir=None):
-    if dir is not None:
-        os.makedirs(dir, exist_ok=True)
-
-    file_obj = tempfile.NamedTemporaryFile(
-        delete=False, suffix=".json", dir=dir, mode="w+"
-    )
-    if isinstance(jsn, str):
-        jsn = json.loads(jsn)
-    json.dump(jsn, file_obj)
-    file_obj.flush()
-    return file_obj
-
-
-def file_to_json(file_path: str | Path) -> Dict:
-    with open(file_path) as f:
-        return json.load(f)
-
-
-########################
-# Misc utils
-########################
-
-
-def synchronize_async(func: Callable, *args, **kwargs) -> Any:
-    """
-    Runs async functions in sync scopes. Can be used in any scope.
-
-    Example:
-        if inspect.iscoroutinefunction(block_fn.fn):
-            predictions = utils.synchronize_async(block_fn.fn, *processed_input)
-
-    Args:
-        func:
-        *args:
-        **kwargs:
-    """
-    return fsspec.asyn.sync(fsspec.asyn.get_loop(), func, *args, **kwargs)  # type: ignore
+from __future__ import annotations
+
+import asyncio
+import base64
+import json
+import mimetypes
+import os
+import pkgutil
+import shutil
+import tempfile
+from concurrent.futures import CancelledError
+from dataclasses import dataclass, field
+from datetime import datetime
+from enum import Enum
+from pathlib import Path
+from threading import Lock
+from typing import Any, Callable, Dict, List, Tuple
+
+import fsspec.asyn
+import httpx
+import requests
+from websockets.legacy.protocol import WebSocketCommonProtocol
+
+API_URL = "/api/predict/"
+WS_URL = "/queue/join"
+UPLOAD_URL = "/upload"
+RESET_URL = "/reset"
+DUPLICATE_URL = "https://huggingface.co/spaces/{}?duplicate=true"
+STATE_COMPONENT = "state"
+
+__version__ = (pkgutil.get_data(__name__, "version.txt") or b"").decode("ascii").strip()
+
+
+class TooManyRequestsError(Exception):
+    """Raised when the API returns a 429 status code."""
+
+    pass
+
+
+class QueueError(Exception):
+    """Raised when the queue is full or there is an issue adding a job to the queue."""
+
+    pass
+
+
+class InvalidAPIEndpointError(Exception):
+    """Raised when the API endpoint is invalid."""
+
+    pass
+
+
+class Status(Enum):
+    """Status codes presented to client users."""
+
+    STARTING = "STARTING"
+    JOINING_QUEUE = "JOINING_QUEUE"
+    QUEUE_FULL = "QUEUE_FULL"
+    IN_QUEUE = "IN_QUEUE"
+    SENDING_DATA = "SENDING_DATA"
+    PROCESSING = "PROCESSSING"
+    ITERATING = "ITERATING"
+    FINISHED = "FINISHED"
+    CANCELLED = "CANCELLED"
+
+    @staticmethod
+    def ordering(status: "Status") -> int:
+        """Order of messages. Helpful for testing."""
+        order = [
+            Status.STARTING,
+            Status.JOINING_QUEUE,
+            Status.QUEUE_FULL,
+            Status.IN_QUEUE,
+            Status.SENDING_DATA,
+            Status.PROCESSING,
+            Status.ITERATING,
+            Status.FINISHED,
+            Status.CANCELLED,
+        ]
+        return order.index(status)
+
+    def __lt__(self, other: "Status"):
+        return self.ordering(self) < self.ordering(other)
+
+    @staticmethod
+    def msg_to_status(msg: str) -> "Status":
+        """Map the raw message from the backend to the status code presented to users."""
+        return {
+            "send_hash": Status.JOINING_QUEUE,
+            "queue_full": Status.QUEUE_FULL,
+            "estimation": Status.IN_QUEUE,
+            "send_data": Status.SENDING_DATA,
+            "process_starts": Status.PROCESSING,
+            "process_generating": Status.ITERATING,
+            "process_completed": Status.FINISHED,
+        }[msg]
+
+
+@dataclass
+class StatusUpdate:
+    """Update message sent from the worker thread to the Job on the main thread."""
+
+    code: Status
+    rank: int | None
+    queue_size: int | None
+    eta: float | None
+    success: bool | None
+    time: datetime | None
+
+
+def create_initial_status_update():
+    return StatusUpdate(
+        code=Status.STARTING,
+        rank=None,
+        queue_size=None,
+        eta=None,
+        success=None,
+        time=datetime.now(),
+    )
+
+
+@dataclass
+class JobStatus:
+    """The job status.
+
+    Keeps strack of the latest status update and intermediate outputs (not yet implements).
+    """
+
+    latest_status: StatusUpdate = field(default_factory=create_initial_status_update)
+    outputs: List[Any] = field(default_factory=list)
+
+
+@dataclass
+class Communicator:
+    """Helper class to help communicate between the worker thread and main thread."""
+
+    lock: Lock
+    job: JobStatus
+    deserialize: Callable[..., Tuple]
+    reset_url: str
+    should_cancel: bool = False
+
+
+########################
+# Network utils
+########################
+
+
+def is_valid_url(possible_url: str) -> bool:
+    headers = {"User-Agent": "gradio (https://gradio.app/; team@gradio.app)"}
+    try:
+        head_request = requests.head(possible_url, headers=headers)
+        if head_request.status_code == 405:
+            return requests.get(possible_url, headers=headers).ok
+        return head_request.ok
+    except Exception:
+        return False
+
+
+async def get_pred_from_ws(
+    websocket: WebSocketCommonProtocol,
+    data: str,
+    hash_data: str,
+    helper: Communicator | None = None,
+) -> Dict[str, Any]:
+    completed = False
+    resp = {}
+    while not completed:
+        # Receive message in the background so that we can
+        # cancel even while running a long pred
+        task = asyncio.create_task(websocket.recv())
+        while not task.done():
+            if helper:
+                with helper.lock:
+                    if helper.should_cancel:
+                        # Need to reset the iterator state since the client
+                        # will not reset the session
+                        async with httpx.AsyncClient() as http:
+                            reset = http.post(
+                                helper.reset_url, json=json.loads(hash_data)
+                            )
+                            # Retrieve cancel exception from task
+                            # otherwise will get nasty warning in console
+                            task.cancel()
+                            await asyncio.gather(task, reset, return_exceptions=True)
+                        raise CancelledError()
+            # Need to suspend this coroutine so that task actually runs
+            await asyncio.sleep(0.01)
+        msg = task.result()
+        resp = json.loads(msg)
+        if helper:
+            with helper.lock:
+                status_update = StatusUpdate(
+                    code=Status.msg_to_status(resp["msg"]),
+                    queue_size=resp.get("queue_size"),
+                    rank=resp.get("rank", None),
+                    success=resp.get("success"),
+                    time=datetime.now(),
+                    eta=resp.get("rank_eta"),
+                )
+                output = resp.get("output", {}).get("data", [])
+                if output and status_update.code != Status.FINISHED:
+                    try:
+                        result = helper.deserialize(*output)
+                    except Exception as e:
+                        result = [e]
+                    helper.job.outputs.append(result)
+                helper.job.latest_status = status_update
+        if resp["msg"] == "queue_full":
+            raise QueueError("Queue is full! Please try again.")
+        if resp["msg"] == "send_hash":
+            await websocket.send(hash_data)
+        elif resp["msg"] == "send_data":
+            await websocket.send(data)
+        completed = resp["msg"] == "process_completed"
+    return resp["output"]
+
+
+########################
+# Data processing utils
+########################
+
+
+def download_tmp_copy_of_file(
+    url_path: str, hf_token: str | None = None, dir: str | None = None
+) -> tempfile._TemporaryFileWrapper:
+    if dir is not None:
+        os.makedirs(dir, exist_ok=True)
+    headers = {"Authorization": "Bearer " + hf_token} if hf_token else {}
+    prefix = Path(url_path).stem
+    suffix = Path(url_path).suffix
+    file_obj = tempfile.NamedTemporaryFile(
+        delete=False,
+        prefix=prefix,
+        suffix=suffix,
+        dir=dir,
+    )
+    with requests.get(url_path, headers=headers, stream=True) as r:
+        with open(file_obj.name, "wb") as f:
+            shutil.copyfileobj(r.raw, f)
+    return file_obj
+
+
+def create_tmp_copy_of_file(
+    file_path: str, dir: str | None = None
+) -> tempfile._TemporaryFileWrapper:
+    if dir is not None:
+        os.makedirs(dir, exist_ok=True)
+    prefix = Path(file_path).stem
+    suffix = Path(file_path).suffix
+    file_obj = tempfile.NamedTemporaryFile(
+        delete=False,
+        prefix=prefix,
+        suffix=suffix,
+        dir=dir,
+    )
+    shutil.copy2(file_path, file_obj.name)
+    return file_obj
+
+
+def get_mimetype(filename: str) -> str | None:
+    mimetype = mimetypes.guess_type(filename)[0]
+    if mimetype is not None:
+        mimetype = mimetype.replace("x-wav", "wav").replace("x-flac", "flac")
+    return mimetype
+
+
+def get_extension(encoding: str) -> str | None:
+    encoding = encoding.replace("audio/wav", "audio/x-wav")
+    type = mimetypes.guess_type(encoding)[0]
+    if type == "audio/flac":  # flac is not supported by mimetypes
+        return "flac"
+    elif type is None:
+        return None
+    extension = mimetypes.guess_extension(type)
+    if extension is not None and extension.startswith("."):
+        extension = extension[1:]
+    return extension
+
+
+def encode_file_to_base64(f):
+    with open(f, "rb") as file:
+        encoded_string = base64.b64encode(file.read())
+        base64_str = str(encoded_string, "utf-8")
+        mimetype = get_mimetype(f)
+        return (
+            "data:"
+            + (mimetype if mimetype is not None else "")
+            + ";base64,"
+            + base64_str
+        )
+
+
+def encode_url_to_base64(url):
+    encoded_string = base64.b64encode(requests.get(url).content)
+    base64_str = str(encoded_string, "utf-8")
+    mimetype = get_mimetype(url)
+    return (
+        "data:" + (mimetype if mimetype is not None else "") + ";base64," + base64_str
+    )
+
+
+def encode_url_or_file_to_base64(path: str | Path):
+    path = str(path)
+    if is_valid_url(path):
+        return encode_url_to_base64(path)
+    else:
+        return encode_file_to_base64(path)
+
+
+def decode_base64_to_binary(encoding) -> Tuple[bytes, str | None]:
+    extension = get_extension(encoding)
+    try:
+        data = encoding.split(",")[1]
+    except IndexError:
+        data = ""
+    return base64.b64decode(data), extension
+
+
+def strip_invalid_filename_characters(filename: str, max_bytes: int = 200) -> str:
+    """Strips invalid characters from a filename and ensures that the file_length is less than `max_bytes` bytes."""
+    filename = "".join([char for char in filename if char.isalnum() or char in "._- "])
+    filename_len = len(filename.encode())
+    if filename_len > max_bytes:
+        while filename_len > max_bytes:
+            if len(filename) == 0:
+                break
+            filename = filename[:-1]
+            filename_len = len(filename.encode())
+    return filename
+
+
+def decode_base64_to_file(encoding, file_path=None, dir=None, prefix=None):
+    if dir is not None:
+        os.makedirs(dir, exist_ok=True)
+    data, extension = decode_base64_to_binary(encoding)
+    if file_path is not None and prefix is None:
+        filename = Path(file_path).name
+        prefix = filename
+        if "." in filename:
+            prefix = filename[0 : filename.index(".")]
+            extension = filename[filename.index(".") + 1 :]
+
+    if prefix is not None:
+        prefix = strip_invalid_filename_characters(prefix)
+
+    if extension is None:
+        file_obj = tempfile.NamedTemporaryFile(delete=False, prefix=prefix, dir=dir)
+    else:
+        file_obj = tempfile.NamedTemporaryFile(
+            delete=False,
+            prefix=prefix,
+            suffix="." + extension,
+            dir=dir,
+        )
+    file_obj.write(data)
+    file_obj.flush()
+    return file_obj
+
+
+def dict_or_str_to_json_file(jsn, dir=None):
+    if dir is not None:
+        os.makedirs(dir, exist_ok=True)
+
+    file_obj = tempfile.NamedTemporaryFile(
+        delete=False, suffix=".json", dir=dir, mode="w+"
+    )
+    if isinstance(jsn, str):
+        jsn = json.loads(jsn)
+    json.dump(jsn, file_obj)
+    file_obj.flush()
+    return file_obj
+
+
+def file_to_json(file_path: str | Path) -> Dict:
+    with open(file_path) as f:
+        return json.load(f)
+
+
+########################
+# Misc utils
+########################
+
+
+def synchronize_async(func: Callable, *args, **kwargs) -> Any:
+    """
+    Runs async functions in sync scopes. Can be used in any scope.
+
+    Example:
+        if inspect.iscoroutinefunction(block_fn.fn):
+            predictions = utils.synchronize_async(block_fn.fn, *processed_input)
+
+    Args:
+        func:
+        *args:
+        **kwargs:
+    """
+    return fsspec.asyn.sync(fsspec.asyn.get_loop(), func, *args, **kwargs)  # type: ignore
```

### Comparing `gradio_client-0.0.8/pyproject.toml` & `gradio_client-0.0.9/pyproject.toml`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-[build-system]
-requires = ["hatchling", "hatch-requirements-txt", "hatch-fancy-pypi-readme>=22.5.0"]
-build-backend = "hatchling.build"
-
-[project]
-name = "gradio_client"
-dynamic = ["version", "dependencies", "readme"]
-description = "Python library for easily interacting with trained machine learning models"
-license = "Apache-2.0"
-requires-python = ">=3.7"
-authors = [
-  { name = "Abubakar Abid", email = "team@gradio.app" },
-  { name = "Ali Abid", email = "team@gradio.app" },
-  { name = "Ali Abdalla", email = "team@gradio.app" },
-  { name = "Dawood Khan", email = "team@gradio.app" },
-  { name = "Ahsen Khaliq", email = "team@gradio.app" },
-  { name = "Pete Allen", email = "team@gradio.app" },
-  { name = "Freddy Boulton", email = "team@gradio.app" },
-]
-keywords = ["machine learning", "client", "API"]
-
-[project.urls]
-Homepage = "https://github.com/gradio-app/gradio"
-
-[tool.hatch.version]
-path = "gradio_client/version.txt"
-pattern = "(?P<version>.+)"
-
-[tool.hatch.metadata.hooks.requirements_txt]
-filename = "requirements.txt"
-
-[tool.hatch.metadata.hooks.fancy-pypi-readme]
-content-type = "text/markdown"
-fragments = [
-  { path = "README.md" },
-]
-
-[tool.hatch.build.targets.sdist]
-include = [
-  "/gradio_client",
-  "/README.md",
-  "/requirements.txt",
-]
-
-[tool.ruff]
-extend = "../../pyproject.toml"
-
-[tool.ruff.isort]
-known-first-party = [
-  "gradio_client"
-]
+[build-system]
+requires = ["hatchling", "hatch-requirements-txt", "hatch-fancy-pypi-readme>=22.5.0"]
+build-backend = "hatchling.build"
+
+[project]
+name = "gradio_client"
+dynamic = ["version", "dependencies", "readme"]
+description = "Python library for easily interacting with trained machine learning models"
+license = "Apache-2.0"
+requires-python = ">=3.7"
+authors = [
+  { name = "Abubakar Abid", email = "team@gradio.app" },
+  { name = "Ali Abid", email = "team@gradio.app" },
+  { name = "Ali Abdalla", email = "team@gradio.app" },
+  { name = "Dawood Khan", email = "team@gradio.app" },
+  { name = "Ahsen Khaliq", email = "team@gradio.app" },
+  { name = "Pete Allen", email = "team@gradio.app" },
+  { name = "Freddy Boulton", email = "team@gradio.app" },
+]
+keywords = ["machine learning", "client", "API"]
+
+[project.urls]
+Homepage = "https://github.com/gradio-app/gradio"
+
+[tool.hatch.version]
+path = "gradio_client/version.txt"
+pattern = "(?P<version>.+)"
+
+[tool.hatch.metadata.hooks.requirements_txt]
+filename = "requirements.txt"
+
+[tool.hatch.metadata.hooks.fancy-pypi-readme]
+content-type = "text/markdown"
+fragments = [
+  { path = "README.md" },
+]
+
+[tool.hatch.build.targets.sdist]
+include = [
+  "/gradio_client",
+  "/README.md",
+  "/requirements.txt",
+]
+
+[tool.ruff]
+extend = "../../pyproject.toml"
+
+[tool.ruff.isort]
+known-first-party = [
+  "gradio_client"
+]
```

### Comparing `gradio_client-0.0.8/PKG-INFO` & `gradio_client-0.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,229 +1,212 @@
-Metadata-Version: 2.1
-Name: gradio_client
-Version: 0.0.8
-Summary: Python library for easily interacting with trained machine learning models
-Project-URL: Homepage, https://github.com/gradio-app/gradio
-Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
-License-Expression: Apache-2.0
-Keywords: API,client,machine learning
-Requires-Python: >=3.7
-Requires-Dist: fsspec
-Requires-Dist: huggingface-hub>=0.13.0
-Requires-Dist: packaging
-Requires-Dist: requests
-Requires-Dist: typing-extensions
-Requires-Dist: websockets
-Description-Content-Type: text/markdown
-
-# `gradio_client`: Use a Gradio app as an API -- in 3 lines of Python
-
-This directory contains the source code for `gradio_client`, a lightweight Python library that makes it very easy to use any Gradio app as an API. 
-
-As an example, consider this [Hugging Face Space that transcribes audio files](https://huggingface.co/spaces/abidlabs/whisper) that are recorded from the microphone.
-
-![](https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/gradio-guides/whisper-screenshot.jpg)
-
-Using the `gradio_client` library, we can easily use the Gradio as an API to transcribe audio files programmatically.
-
-Here's the entire code to do it:
-
-```python
-from gradio_client import Client
-
-client = Client("abidlabs/whisper") 
-client.predict("audio_sample.wav")  
-
->> "This is a test of the whisper speech recognition model."
-```
-
-The Gradio client works with any Gradio Space, whether it be an image generator, a stateful chatbot, or a tax calculator.
-
-## Installation
-
-If you already have a recent version of `gradio`, then the `gradio_client` is included as a dependency. 
-
-Otherwise, the lightweight `gradio_client` package can be installed from pip (or pip3) and works with Python versions 3.9 or higher:
-
-```bash
-$ pip install gradio_client
-```
-
-## Usage
-
-### Connecting to a Space or a Gradio app
-
-Start by connecting instantiating a `Client` object and connecting it to a Gradio app that is running on Spaces (or anywhere else)!
-
-**Connecting to a Space**
-
-```python
-from gradio_client import Client
-
-client = Client("abidlabs/en2fr")  # a Space that translates from English to French
-```
-
-You can also connect to private Spaces by passing in your HF token with the `hf_token` parameter. You can get your HF token here: https://huggingface.co/settings/tokens
-
-```python
-from gradio_client import Client
-
-client = Client("abidlabs/my-private-space", hf_token="...") 
-```
-
-
-**Connecting a general Gradio app**
-
-If your app is running somewhere else, just provide the full URL instead, including the "http://" or "https://". Here's an example of making predictions to a Gradio app that is running on a share URL:
-
-```python
-from gradio_client import Client
-
-client = Client("https://bec81a83-5b5c-471e.gradio.live")
-```
-
-### Inspecting the API endpoints
-
-Once you have connected to a Gradio app, you can view the APIs that are available to you by calling the `Client.view_api()` method. For the Whisper Space, we see the following:
-
-```
-Client.predict() Usage Info
----------------------------
-Named API endpoints: 1
-
- - predict(input_audio, api_name="/predict") -> value_0
-    Parameters:
-     - [Audio] input_audio: str (filepath or URL)
-    Returns:
-     - [Textbox] value_0: str (value)
-```
-
-This shows us that we have 1 API endpoint in this space, and shows us how to use the API endpoint to make a prediction: we should call the `.predict()` method, providing a parameter `input_audio` of type `str`, which is a `filepath or URL`. 
-
-We should also provide the `api_name='/predict'` argument. Although this isn't necessary if a Gradio app has a single named endpoint, it does allow us to call different endpoints in a single app if they are available. If an app has unnamed API endpoints, these can also be displayed by running `.view_api(all_endpoints=True)`.
-
-
-### Making a prediction
-
-The simplest way to make a prediction is simply to call the `.predict()` function with the appropriate arguments:
-
-```python
-from gradio_client import Client
-
-client = Client("abidlabs/en2fr")
-client.predict("Hello")
-
->> Bonjour
-```
-
-If there are multiple parameters, then you should pass them as separate arguments to `.predict()`, like this:
-
-
-```python
-from gradio_client import Client
-
-client = Client("gradio/calculator")
-client.predict(4, "add", 5)
-
->> 9.0
-```
-
-For certain inputs, such as images, you should pass in the filepath or URL to the file. Likewise, for the corresponding output types, you will get a filepath or URL returned. 
-
-```python
-from gradio_client import Client
-
-client = Client("abidlabs/whisper")
-client.predict("https://audio-samples.github.io/samples/mp3/blizzard_unconditional/sample-0.mp3")
-
->> "My thought I have nobody by a beauty and will as you poured. Mr. Rochester is serve in that so don't find simpus, and devoted abode, to at might in a r—"
-```
-
-
-**Running jobs asyncronously**
-
-Oe should note that `.predict()` is a *blocking* operation as it waits for the operation to complete before returning the prediction. 
-
-In many cases, you may be better off letting the job run in the background until you need the results of the prediction. You can do this by creating a `Job` instance using the `.submit()` method, and then later calling `.result()` on the job to get the result. For example:
-
-```python
-from gradio_client import Client
-
-client = Client(space="abidlabs/en2fr")
-job = client.submit("Hello", api_name="/predict")  # This is not blocking
-
-# Do something else
-
-job.result()  # This is blocking
-
->> Bonjour
-```
-
-**Adding callbacks**
-
-Alternatively, one can add one or more callbacks to perform actions after the job has completed running, like this:
-
-```python
-from gradio_client import Client
-
-def print_result(x):
-    print("The translated result is: {x}")
-
-client = Client(space="abidlabs/en2fr")
-
-job = client.submit("Hello", api_name="/predict", result_callbacks=[print_result])
-
-# Do something else
-
->> The translated result is: Bonjour
-
-```
-
-**Status**
-
-The `Job` object also allows you to get the status of the running job by calling the `.status()` method. This returns a `StatusUpdate` object with the following attributes: `code` (the status code, one of a set of defined strings representing the status. See the `utils.Status` class), `rank` (the current position of this job in the queue), `queue_size` (the total queue size),  `eta` (estimated time this job will complete), `success` (a boolean representing whether the job completed successfully), and `time` (the time that the status was generated). 
-
-```py
-from gradio_client import Client
-
-client = Client(src="gradio/calculator")
-job = client.submit(5, "add", 4, api_name="/predict")
-job.status()
-
->> <Status.STARTING: 'STARTING'>
-```
-
-The `Job` object also has a `done()` instance method which returns a boolean indicating whether the job has completed.
-
-### Generator Endpoints
-
-Some Gradio API endpoints do not return a single value, rather they return a series of values. You can get the series of values that have been returned at any time from such a generator endpoint by running `job.outputs()`:
-
-```py
-from gradio_client import Client
-
-client = Client(src="gradio/count_generator")
-job = client.submit(3, api_name="/count")
-while not job.done():
-    time.sleep(0.1)
-job.outputs()
-
->> ['0', '1', '2']
-```
-
-Note that running `job.result()` on a generator endpoint only gives you the *first* value returned by the endpoint. 
-
-The `Job` object is also iterable, which means you can use it to display the results of a generator function as they are returned from the endpoint. Here's the equivalent example using the `Job` as a generator:
-
-```py
-from gradio_client import Client
-
-client = Client(src="gradio/count_generator")
-job = client.submit(3, api_name="/count")
-
-for o in job:
-    print(o)
-
->> 0
->> 1
->> 2
+# `gradio_client`: Use a Gradio app as an API -- in 3 lines of Python
+
+This directory contains the source code for `gradio_client`, a lightweight Python library that makes it very easy to use any Gradio app as an API. 
+
+As an example, consider this [Hugging Face Space that transcribes audio files](https://huggingface.co/spaces/abidlabs/whisper) that are recorded from the microphone.
+
+![](https://huggingface.co/datasets/huggingface/documentation-images/resolve/main/gradio-guides/whisper-screenshot.jpg)
+
+Using the `gradio_client` library, we can easily use the Gradio as an API to transcribe audio files programmatically.
+
+Here's the entire code to do it:
+
+```python
+from gradio_client import Client
+
+client = Client("abidlabs/whisper") 
+client.predict("audio_sample.wav")  
+
+>> "This is a test of the whisper speech recognition model."
+```
+
+The Gradio client works with any Gradio Space, whether it be an image generator, a stateful chatbot, or a tax calculator.
+
+## Installation
+
+If you already have a recent version of `gradio`, then the `gradio_client` is included as a dependency. 
+
+Otherwise, the lightweight `gradio_client` package can be installed from pip (or pip3) and works with Python versions 3.9 or higher:
+
+```bash
+$ pip install gradio_client
+```
+
+## Usage
+
+### Connecting to a Space or a Gradio app
+
+Start by connecting instantiating a `Client` object and connecting it to a Gradio app that is running on Spaces (or anywhere else)!
+
+**Connecting to a Space**
+
+```python
+from gradio_client import Client
+
+client = Client("abidlabs/en2fr")  # a Space that translates from English to French
+```
+
+You can also connect to private Spaces by passing in your HF token with the `hf_token` parameter. You can get your HF token here: https://huggingface.co/settings/tokens
+
+```python
+from gradio_client import Client
+
+client = Client("abidlabs/my-private-space", hf_token="...") 
+```
+
+
+**Connecting a general Gradio app**
+
+If your app is running somewhere else, just provide the full URL instead, including the "http://" or "https://". Here's an example of making predictions to a Gradio app that is running on a share URL:
+
+```python
+from gradio_client import Client
+
+client = Client("https://bec81a83-5b5c-471e.gradio.live")
+```
+
+### Inspecting the API endpoints
+
+Once you have connected to a Gradio app, you can view the APIs that are available to you by calling the `Client.view_api()` method. For the Whisper Space, we see the following:
+
+```
+Client.predict() Usage Info
+---------------------------
+Named API endpoints: 1
+
+ - predict(input_audio, api_name="/predict") -> value_0
+    Parameters:
+     - [Audio] input_audio: str (filepath or URL)
+    Returns:
+     - [Textbox] value_0: str (value)
+```
+
+This shows us that we have 1 API endpoint in this space, and shows us how to use the API endpoint to make a prediction: we should call the `.predict()` method, providing a parameter `input_audio` of type `str`, which is a `filepath or URL`. 
+
+We should also provide the `api_name='/predict'` argument. Although this isn't necessary if a Gradio app has a single named endpoint, it does allow us to call different endpoints in a single app if they are available. If an app has unnamed API endpoints, these can also be displayed by running `.view_api(all_endpoints=True)`.
+
+
+### Making a prediction
+
+The simplest way to make a prediction is simply to call the `.predict()` function with the appropriate arguments:
+
+```python
+from gradio_client import Client
+
+client = Client("abidlabs/en2fr")
+client.predict("Hello")
+
+>> Bonjour
+```
+
+If there are multiple parameters, then you should pass them as separate arguments to `.predict()`, like this:
+
+
+```python
+from gradio_client import Client
+
+client = Client("gradio/calculator")
+client.predict(4, "add", 5)
+
+>> 9.0
+```
+
+For certain inputs, such as images, you should pass in the filepath or URL to the file. Likewise, for the corresponding output types, you will get a filepath or URL returned. 
+
+```python
+from gradio_client import Client
+
+client = Client("abidlabs/whisper")
+client.predict("https://audio-samples.github.io/samples/mp3/blizzard_unconditional/sample-0.mp3")
+
+>> "My thought I have nobody by a beauty and will as you poured. Mr. Rochester is serve in that so don't find simpus, and devoted abode, to at might in a r—"
+```
+
+
+**Running jobs asyncronously**
+
+Oe should note that `.predict()` is a *blocking* operation as it waits for the operation to complete before returning the prediction. 
+
+In many cases, you may be better off letting the job run in the background until you need the results of the prediction. You can do this by creating a `Job` instance using the `.submit()` method, and then later calling `.result()` on the job to get the result. For example:
+
+```python
+from gradio_client import Client
+
+client = Client(space="abidlabs/en2fr")
+job = client.submit("Hello", api_name="/predict")  # This is not blocking
+
+# Do something else
+
+job.result()  # This is blocking
+
+>> Bonjour
+```
+
+**Adding callbacks**
+
+Alternatively, one can add one or more callbacks to perform actions after the job has completed running, like this:
+
+```python
+from gradio_client import Client
+
+def print_result(x):
+    print("The translated result is: {x}")
+
+client = Client(space="abidlabs/en2fr")
+
+job = client.submit("Hello", api_name="/predict", result_callbacks=[print_result])
+
+# Do something else
+
+>> The translated result is: Bonjour
+
+```
+
+**Status**
+
+The `Job` object also allows you to get the status of the running job by calling the `.status()` method. This returns a `StatusUpdate` object with the following attributes: `code` (the status code, one of a set of defined strings representing the status. See the `utils.Status` class), `rank` (the current position of this job in the queue), `queue_size` (the total queue size),  `eta` (estimated time this job will complete), `success` (a boolean representing whether the job completed successfully), and `time` (the time that the status was generated). 
+
+```py
+from gradio_client import Client
+
+client = Client(src="gradio/calculator")
+job = client.submit(5, "add", 4, api_name="/predict")
+job.status()
+
+>> <Status.STARTING: 'STARTING'>
+```
+
+The `Job` object also has a `done()` instance method which returns a boolean indicating whether the job has completed.
+
+### Generator Endpoints
+
+Some Gradio API endpoints do not return a single value, rather they return a series of values. You can get the series of values that have been returned at any time from such a generator endpoint by running `job.outputs()`:
+
+```py
+from gradio_client import Client
+
+client = Client(src="gradio/count_generator")
+job = client.submit(3, api_name="/count")
+while not job.done():
+    time.sleep(0.1)
+job.outputs()
+
+>> ['0', '1', '2']
+```
+
+Note that running `job.result()` on a generator endpoint only gives you the *first* value returned by the endpoint. 
+
+The `Job` object is also iterable, which means you can use it to display the results of a generator function as they are returned from the endpoint. Here's the equivalent example using the `Job` as a generator:
+
+```py
+from gradio_client import Client
+
+client = Client(src="gradio/count_generator")
+job = client.submit(3, api_name="/count")
+
+for o in job:
+    print(o)
+
+>> 0
+>> 1
+>> 2
 ```
```

