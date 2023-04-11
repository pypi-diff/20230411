# Comparing `tmp/lupin-danquin-0.0.1.dev2.tar.gz` & `tmp/lupin-danquin-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-danquin-0.0.1.dev2.tar", last modified: Sun Apr  9 21:53:09 2023, max compression
+gzip compressed data, was "lupin-danquin-0.0.1.dev3.tar", last modified: Tue Apr 11 08:33:32 2023, max compression
```

## Comparing `lupin-danquin-0.0.1.dev2.tar` & `lupin-danquin-0.0.1.dev3.tar`

### file list

```diff
@@ -1,34 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 21:53:09.715095 lupin-danquin-0.0.1.dev2/
--rw-rw-rw-   0        0        0     1093 2023-04-09 16:27:22.000000 lupin-danquin-0.0.1.dev2/LICENCE
--rw-rw-rw-   0        0        0      573 2023-04-09 21:53:09.715095 lupin-danquin-0.0.1.dev2/PKG-INFO
--rw-rw-rw-   0        0        0     1010 2023-04-09 16:27:22.000000 lupin-danquin-0.0.1.dev2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 21:53:09.690273 lupin-danquin-0.0.1.dev2/lupin_danquin/
--rw-rw-rw-   0        0        0       28 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/__init__.py
--rw-rw-rw-   0        0        0       78 2023-04-09 16:33:06.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/__main__.py
--rw-rw-rw-   0        0        0      825 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/check_coding_rules.py
-drwxrwxrwx   0        0        0        0 2023-04-09 21:53:09.712093 lupin-danquin-0.0.1.dev2/lupin_danquin/core/
--rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/__init__.py
--rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/application.py
--rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/global_variable.py
--rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/line_ended.py
--rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/local_variable.py
--rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/parameter.py
--rw-rw-rw-   0        0        0     4619 2023-04-09 15:14:46.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/program.py
--rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/rules.py
-drwxrwxrwx   0        0        0        0 2023-04-09 21:53:09.713095 lupin-danquin-0.0.1.dev2/lupin_danquin/core/tools/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/tools/__init__.py
--rw-rw-rw-   0        0        0     1917 2023-04-09 21:52:28.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 21:53:09.714095 lupin-danquin-0.0.1.dev2/lupin_danquin/core/val3_doc_generator/
--rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/val3_doc_generator/__init__.py
--rw-rw-rw-   0        0        0     3264 2023-04-09 17:28:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
--rw-rw-rw-   0        0        0     1441 2023-04-09 21:52:55.000000 lupin-danquin-0.0.1.dev2/lupin_danquin/run.py
-drwxrwxrwx   0        0        0        0 2023-04-09 21:53:09.704784 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/
--rw-rw-rw-   0        0        0      573 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-09 16:34:59.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-09 21:53:09.000000 lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      906 2023-04-09 21:53:09.716094 lupin-danquin-0.0.1.dev2/setup.cfg
--rw-rw-rw-   0        0        0      172 2023-04-09 16:27:22.000000 lupin-danquin-0.0.1.dev2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.927216 lupin-danquin-0.0.1.dev3/
+-rw-rw-rw-   0        0        0     1093 2023-04-09 16:27:22.000000 lupin-danquin-0.0.1.dev3/LICENCE
+-rw-rw-rw-   0        0        0       67 2023-04-11 08:12:17.000000 lupin-danquin-0.0.1.dev3/MANIFEST.in
+-rw-rw-rw-   0        0        0      573 2023-04-11 08:33:32.927216 lupin-danquin-0.0.1.dev3/PKG-INFO
+-rw-rw-rw-   0        0        0     1010 2023-04-09 16:27:22.000000 lupin-danquin-0.0.1.dev3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.895696 lupin-danquin-0.0.1.dev3/lupin_danquin/
+-rw-rw-rw-   0        0        0       28 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/__init__.py
+-rw-rw-rw-   0        0        0       78 2023-04-09 16:33:06.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.914700 lupin-danquin-0.0.1.dev3/lupin_danquin/assets/
+-rw-rw-rw-   0        0        0     6730 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/assets/BeginingOfFile.md
+-rw-rw-rw-   0        0        0      379 2023-04-03 12:43:51.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/assets/EndOfFile.md
+-rw-rw-rw-   0        0        0      825 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/check_coding_rules.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.923216 lupin-danquin-0.0.1.dev3/lupin_danquin/core/
+-rw-rw-rw-   0        0        0        0 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/__init__.py
+-rw-rw-rw-   0        0        0     4561 2023-04-07 13:23:10.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/application.py
+-rw-rw-rw-   0        0        0     1797 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/global_variable.py
+-rw-rw-rw-   0        0        0       23 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/line_ended.py
+-rw-rw-rw-   0        0        0     1173 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/local_variable.py
+-rw-rw-rw-   0        0        0     1448 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/parameter.py
+-rw-rw-rw-   0        0        0     4619 2023-04-09 15:14:46.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/program.py
+-rw-rw-rw-   0        0        0      356 2023-04-05 07:25:51.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/rules.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.924219 lupin-danquin-0.0.1.dev3/lupin_danquin/core/tools/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/tools/__init__.py
+-rw-rw-rw-   0        0        0     1917 2023-04-09 21:52:28.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.926214 lupin-danquin-0.0.1.dev3/lupin_danquin/core/val3_doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/val3_doc_generator/__init__.py
+-rw-rw-rw-   0        0        0     3261 2023-04-11 08:28:18.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
+-rw-rw-rw-   0        0        0     1438 2023-04-11 08:14:47.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/run.py
+drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.927216 lupin-danquin-0.0.1.dev3/lupin_danquin/templates/
+-rw-rw-rw-   0        0        0     2728 2023-04-07 07:13:26.000000 lupin-danquin-0.0.1.dev3/lupin_danquin/templates/val3_documentation_md.j2
+drwxrwxrwx   0        0        0        0 2023-04-11 08:33:32.912699 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/
+-rw-rw-rw-   0        0        0      573 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-09 16:34:59.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       90 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 08:33:32.000000 lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      906 2023-04-11 08:33:32.928214 lupin-danquin-0.0.1.dev3/setup.cfg
+-rw-rw-rw-   0        0        0      172 2023-04-09 16:27:22.000000 lupin-danquin-0.0.1.dev3/setup.py
```

### Comparing `lupin-danquin-0.0.1.dev2/LICENCE` & `lupin-danquin-0.0.1.dev3/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev2/PKG-INFO` & `lupin-danquin-0.0.1.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-0.0.1.dev2/README.md` & `lupin-danquin-0.0.1.dev3/README.md`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev2/lupin_danquin/check_coding_rules.py` & `lupin-danquin-0.0.1.dev3/lupin_danquin/check_coding_rules.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev2/lupin_danquin/core/application.py` & `lupin-danquin-0.0.1.dev3/lupin_danquin/core/application.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev2/lupin_danquin/core/global_variable.py` & `lupin-danquin-0.0.1.dev3/lupin_danquin/core/global_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev2/lupin_danquin/core/local_variable.py` & `lupin-danquin-0.0.1.dev3/lupin_danquin/core/local_variable.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev2/lupin_danquin/core/parameter.py` & `lupin-danquin-0.0.1.dev3/lupin_danquin/core/parameter.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev2/lupin_danquin/core/program.py` & `lupin-danquin-0.0.1.dev3/lupin_danquin/core/program.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev2/lupin_danquin/core/tools/utils.py` & `lupin-danquin-0.0.1.dev3/lupin_danquin/core/tools/utils.py`

 * *Files identical despite different names*

### Comparing `lupin-danquin-0.0.1.dev2/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py` & `lupin-danquin-0.0.1.dev3/lupin_danquin/core/val3_doc_generator/val3_doc_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List
 import codecs
 import os
 
 from jinja2 import (
     Environment,
-    FileSystemLoader,
+    PackageLoader,
     select_autoescape,
     Template,
     TemplateNotFound,
     TemplateError,
     TemplateRuntimeError,
 )
 
@@ -55,15 +55,15 @@
             result = f.read()
         return result
 
     def _get_local_template(self) -> Template:
         try:
             # Create jinja2 environment
             env = Environment(
-                loader=FileSystemLoader("lupin_danquin/templates"),
+                loader=PackageLoader("lupin_danquin", "templates"),
                 autoescape=select_autoescape(),
                 trim_blocks=True,
                 lstrip_blocks=True,
             )
             # Charge template
             template = env.get_template("val3_documentation_md.j2")
             return template
```

### Comparing `lupin-danquin-0.0.1.dev2/lupin_danquin/run.py` & `lupin-danquin-0.0.1.dev3/lupin_danquin/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 @cli.command(help="Print version")
 def version():
     print(f"Version: {__version__}")
 
 
 @cli.command()
-def val_docs(
+def valdocs(
     application_names: Optional[str] = typer.Argument(
         ...,
         help="Name of applications to be documented. Ex: 'app1,app2,app3'",
         envvar="VAL3_APPLICATIONS",
     )
 ):
     """
     Generate documentation from VAL3 applications in usrapp directory.
-    You can specify the applications to be documented in the 'danq val-docs' command
+    You can specify the applications to be documented in the 'danq valdocs' command
     or by setting the VAL3_APPLICATIONS environment variable.
     :param application_names: Name of applications to be documented. Ex: app1,app2,app3
     :type application_names: str
 
-    :example: danq val_docs "App1,App2"
+    :example: danq valdocs "App1,App2"
     """
     if not application_names:
         application_names = must_get_string_value_from_env_var("VAL3_APPLICATIONS")
 
     configure_logging()
     applications_list = convert_application_name_to_list(application_names)
     Val3Documentation().generate_markdown(applications_list=applications_list)
```

### Comparing `lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/PKG-INFO` & `lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lupin-danquin
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: Testing - Documentation
 License: MIT License
 Keywords: documentation,testing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Documentation
```

### Comparing `lupin-danquin-0.0.1.dev2/lupin_danquin.egg-info/SOURCES.txt` & `lupin-danquin-0.0.1.dev3/lupin_danquin.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 LICENCE
+MANIFEST.in
 README.md
 setup.cfg
 setup.py
 lupin_danquin/__init__.py
 lupin_danquin/__main__.py
 lupin_danquin/check_coding_rules.py
 lupin_danquin/run.py
 lupin_danquin.egg-info/PKG-INFO
 lupin_danquin.egg-info/SOURCES.txt
 lupin_danquin.egg-info/dependency_links.txt
 lupin_danquin.egg-info/entry_points.txt
 lupin_danquin.egg-info/not-zip-safe
 lupin_danquin.egg-info/requires.txt
 lupin_danquin.egg-info/top_level.txt
+lupin_danquin/assets/BeginingOfFile.md
+lupin_danquin/assets/EndOfFile.md
 lupin_danquin/core/__init__.py
 lupin_danquin/core/application.py
 lupin_danquin/core/global_variable.py
 lupin_danquin/core/line_ended.py
 lupin_danquin/core/local_variable.py
 lupin_danquin/core/parameter.py
 lupin_danquin/core/program.py
 lupin_danquin/core/rules.py
 lupin_danquin/core/tools/__init__.py
 lupin_danquin/core/tools/utils.py
 lupin_danquin/core/val3_doc_generator/__init__.py
-lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
+lupin_danquin/core/val3_doc_generator/val3_doc_generator.py
+lupin_danquin/templates/val3_documentation_md.j2
```

### Comparing `lupin-danquin-0.0.1.dev2/setup.cfg` & `lupin-danquin-0.0.1.dev3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d64 616e 7175 696e   = lupin-danquin
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
-00000030: 312e 6465 7632 0d0a 6465 7363 7269 7074  1.dev2..descript
+00000030: 312e 6465 7633 0d0a 6465 7363 7269 7074  1.dev3..descript
 00000040: 696f 6e20 3d20 5465 7374 696e 6720 2d20  ion = Testing - 
 00000050: 446f 6375 6d65 6e74 6174 696f 6e0d 0a6c  Documentation..l
 00000060: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000070: 3d20 5465 7374 2056 414c 3320 636f 6465  = Test VAL3 code
 00000080: 2061 6e64 2067 656e 6572 6174 6520 646f   and generate do
 00000090: 6375 6d65 6e74 6174 696f 6e20 6672 6f6d  cumentation from
 000000a0: 2069 740d 0a6b 6579 776f 7264 7320 3d20   it..keywords =
```

