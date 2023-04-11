# Comparing `tmp/jsoninja-1.0.0.tar.gz` & `tmp/jsoninja-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/jsoninja/jsoninja/dist/.tmp-hm_2xvck/jsoninja-1.0.0.tar", last modified: Sun Apr  9 19:46:06 2023, max compression
+gzip compressed data, was "/home/runner/work/jsoninja/jsoninja/dist/.tmp-z0hxh62k/jsoninja-1.0.1.tar", last modified: Tue Apr 11 10:15:02 2023, max compression
```

## Comparing `jsoninja-1.0.0.tar` & `jsoninja-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:46:06.000000 jsoninja-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-09 19:45:57.000000 jsoninja-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-04-09 19:46:06.000000 jsoninja-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-09 19:45:57.000000 jsoninja-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:46:06.000000 jsoninja-1.0.0/jsoninja/
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-09 19:45:57.000000 jsoninja-1.0.0/jsoninja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:46:06.000000 jsoninja-1.0.0/jsoninja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-04-09 19:46:06.000000 jsoninja-1.0.0/jsoninja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-09 19:46:06.000000 jsoninja-1.0.0/jsoninja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:46:06.000000 jsoninja-1.0.0/jsoninja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-09 19:46:06.000000 jsoninja-1.0.0/jsoninja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-09 19:46:06.000000 jsoninja-1.0.0/jsoninja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-09 19:45:57.000000 jsoninja-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:46:06.000000 jsoninja-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:46:06.000000 jsoninja-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-09 19:45:57.000000 jsoninja-1.0.0/tests/test_jsoninja.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:02.000000 jsoninja-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-11 10:14:50.000000 jsoninja-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-11 10:15:02.000000 jsoninja-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-11 10:14:50.000000 jsoninja-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:02.000000 jsoninja-1.0.1/jsoninja/
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-11 10:14:50.000000 jsoninja-1.0.1/jsoninja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:02.000000 jsoninja-1.0.1/jsoninja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-11 10:15:02.000000 jsoninja-1.0.1/jsoninja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-11 10:15:02.000000 jsoninja-1.0.1/jsoninja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:15:02.000000 jsoninja-1.0.1/jsoninja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 10:15:02.000000 jsoninja-1.0.1/jsoninja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 10:15:02.000000 jsoninja-1.0.1/jsoninja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-11 10:14:50.000000 jsoninja-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:15:02.000000 jsoninja-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:02.000000 jsoninja-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-04-11 10:14:50.000000 jsoninja-1.0.1/tests/test_jsoninja.py
```

### Comparing `jsoninja-1.0.0/LICENSE` & `jsoninja-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsoninja-1.0.0/PKG-INFO` & `jsoninja-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsoninja
-Version: 1.0.0
+Version: 1.0.1
 Summary: Jsoninja is a library that allows you to generate JSON's from templates written with Python dicts.
 Author-email: Víctor Lázaro <vlazaro@outlook.es>
 License: MIT License
         
         Copyright (c) 2023 Víctor Lázaro
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,31 +47,31 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 	<p>
-        <a href="https://pypi.org/project/jsoninja" target="_blank">
+        <a href="https://pypi.org/project/jsoninja">
             <img src="https://em-content.zobj.net/thumbs/240/apple/354/ninja_1f977.png" width="100px">
         </a>
     </p>
 	<h1>Jsoninja</h1>
     <p>
         <em>
             A library that allows you to generate JSON's from
             <br/>
             templates written with Python dicts.
         </em>
     </p>
     <p>
-        <a href="https://pypi.org/project/jsoninja" target="_blank">
+        <a href="https://pypi.org/project/jsoninja">
             <img src="https://img.shields.io/pypi/v/jsoninja?label=Version" alt="Library version">
         </a>
-        <a href="https://pypi.org/project/jsoninja" target="_blank">
+        <a href="https://pypi.org/project/jsoninja">
             <img src="https://img.shields.io/pypi/pyversions/jsoninja.svg?label=Python" alt="Supported Python versions">
         </a>
     </p>
 </div>
 
 ## Instalation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jsoninja Version: 1.0.0 Summary: Jsoninja is a
+Metadata-Version: 2.1 Name: jsoninja Version: 1.0.1 Summary: Jsoninja is a
 library that allows you to generate JSON's from templates written with Python
 dicts. Author-email: VÃ­ctor LÃ¡zaro
 outlook.es> License: MIT License Copyright (c) 2023 VÃ­ctor LÃ¡zaro Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

### Comparing `jsoninja-1.0.0/README.md` & `jsoninja-1.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <div align="center">
 	<p>
-        <a href="https://pypi.org/project/jsoninja" target="_blank">
+        <a href="https://pypi.org/project/jsoninja">
             <img src="https://em-content.zobj.net/thumbs/240/apple/354/ninja_1f977.png" width="100px">
         </a>
     </p>
 	<h1>Jsoninja</h1>
     <p>
         <em>
             A library that allows you to generate JSON's from
             <br/>
             templates written with Python dicts.
         </em>
     </p>
     <p>
-        <a href="https://pypi.org/project/jsoninja" target="_blank">
+        <a href="https://pypi.org/project/jsoninja">
             <img src="https://img.shields.io/pypi/v/jsoninja?label=Version" alt="Library version">
         </a>
-        <a href="https://pypi.org/project/jsoninja" target="_blank">
+        <a href="https://pypi.org/project/jsoninja">
             <img src="https://img.shields.io/pypi/pyversions/jsoninja.svg?label=Python" alt="Supported Python versions">
         </a>
     </p>
 </div>
 
 ## Instalation
```

### Comparing `jsoninja-1.0.0/jsoninja/__init__.py` & `jsoninja-1.0.1/jsoninja/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             A dict containing the template with the replaced values.
 
         Raises:
             ValueError: A template has not been loaded.
         """
         if not template:
             raise ValueError("A template has not been loaded.")
-        return self.__scan_template(template, replacements)
+        return self.__scan_template(template.copy(), replacements)
 
     def __scan_template(
         self, template: Dict[str, Any], replacements: Dict[str, Any]
     ) -> Dict[str, Any]:
         """
         Iterate the template and replace the variables with the values.
 
@@ -67,15 +67,15 @@
 
         Returns:
             The value associated with the template variable.
 
         Raises:
             KeyError: Unable to find a replacement for "...".
         """
-        variable_regex = re.compile(r"\{\{[a-zA-Z0-9_]+\}\}")
+        variable_regex = re.compile(r"\{\{\ ?[a-zA-Z0-9_]+\ ?\}\}")
         if variable_regex.fullmatch(str(value)):
             value_key = self.__clean_value(value)
             if value_key in replacements:
                 return replacements[value_key]
             raise KeyError(f'Unable to find a replacement for "{value_key}".')
         return None
 
@@ -85,8 +85,8 @@
 
         Args:
             value (str): The value of the item.
 
         Returns:
             The value of the item without the brackets that declare the variable.
         """
-        return value[2:-2]
+        return value[2:-2].strip()
```

### Comparing `jsoninja-1.0.0/jsoninja.egg-info/PKG-INFO` & `jsoninja-1.0.1/jsoninja.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsoninja
-Version: 1.0.0
+Version: 1.0.1
 Summary: Jsoninja is a library that allows you to generate JSON's from templates written with Python dicts.
 Author-email: Víctor Lázaro <vlazaro@outlook.es>
 License: MIT License
         
         Copyright (c) 2023 Víctor Lázaro
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,31 +47,31 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 	<p>
-        <a href="https://pypi.org/project/jsoninja" target="_blank">
+        <a href="https://pypi.org/project/jsoninja">
             <img src="https://em-content.zobj.net/thumbs/240/apple/354/ninja_1f977.png" width="100px">
         </a>
     </p>
 	<h1>Jsoninja</h1>
     <p>
         <em>
             A library that allows you to generate JSON's from
             <br/>
             templates written with Python dicts.
         </em>
     </p>
     <p>
-        <a href="https://pypi.org/project/jsoninja" target="_blank">
+        <a href="https://pypi.org/project/jsoninja">
             <img src="https://img.shields.io/pypi/v/jsoninja?label=Version" alt="Library version">
         </a>
-        <a href="https://pypi.org/project/jsoninja" target="_blank">
+        <a href="https://pypi.org/project/jsoninja">
             <img src="https://img.shields.io/pypi/pyversions/jsoninja.svg?label=Python" alt="Supported Python versions">
         </a>
     </p>
 </div>
 
 ## Instalation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jsoninja Version: 1.0.0 Summary: Jsoninja is a
+Metadata-Version: 2.1 Name: jsoninja Version: 1.0.1 Summary: Jsoninja is a
 library that allows you to generate JSON's from templates written with Python
 dicts. Author-email: VÃ­ctor LÃ¡zaro
 outlook.es> License: MIT License Copyright (c) 2023 VÃ­ctor LÃ¡zaro Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

### Comparing `jsoninja-1.0.0/pyproject.toml` & `jsoninja-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsoninja"
-version = "1.0.0"
+version = "1.0.1"
 description = "Jsoninja is a library that allows you to generate JSON's from templates written with Python dicts."
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 authors = [
     { name = "Víctor Lázaro", email = "vlazaro@outlook.es" },
 ]
```

### Comparing `jsoninja-1.0.0/tests/test_jsoninja.py` & `jsoninja-1.0.1/tests/test_jsoninja.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,27 @@
         """
         Tests that an exception is raised when the template is not received.
         """
         jsoninja = Jsoninja()
         with pytest.raises(ValueError, match="A template has not been loaded."):
             jsoninja.replace({}, {})
 
+    def test_returns_new_object(self) -> None:
+        """
+        Tests that the template is not replaced and returns a new object.
+        """
+        jsoninja = Jsoninja()
+        template = {
+            "foo": "{{foo}}",
+        }
+        replacements = {
+            "foo": "bar",
+        }
+        assert jsoninja.replace(template, replacements) != template
+
     def test_missing_replacement(self) -> None:
         """
         Tests that an exception is raised when the replacement value of a variable
         declared in the template is not received.
         """
         jsoninja = Jsoninja()
         template = {
@@ -35,14 +48,33 @@
             "firstname": "John",
         }
         with pytest.raises(
             KeyError, match='Unable to find a replacement for "lastname".'
         ):
             jsoninja.replace(template, replacements)
 
+    def test_variable_declarations(self) -> None:
+        """
+        Tests that the variable declarations work correctly.
+        """
+        jsoninja = Jsoninja()
+        template = {
+            "declaration1": "{{declaration1}}",
+            "declaration2": "{{ declaration2 }}",
+        }
+        replacements = {
+            "declaration1": "foo",
+            "declaration2": "bar",
+        }
+        expected = {
+            "declaration1": "foo",
+            "declaration2": "bar",
+        }
+        assert jsoninja.replace(template, replacements) == expected
+
     def test_str_replacement(self) -> None:
         """
         Tests that the replacement of str variables works correctly.
         """
         jsoninja = Jsoninja()
         template = {
             "str": "{{str}}",
```

