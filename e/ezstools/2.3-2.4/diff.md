# Comparing `tmp/ezstools-2.3.tar.gz` & `tmp/ezstools-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezstools-2.3.tar", last modified: Wed Apr  5 23:06:39 2023, max compression
+gzip compressed data, was "ezstools-2.4.tar", last modified: Tue Apr 11 21:30:04 2023, max compression
```

## Comparing `ezstools-2.3.tar` & `ezstools-2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 23:06:39.777058 ezstools-2.3/
--rw-rw-rw-   0        0        0     2512 2023-04-05 23:06:39.775060 ezstools-2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2255 2023-04-05 23:05:59.000000 ezstools-2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 23:06:39.623468 ezstools-2.3/ezstools/
--rw-rw-rw-   0        0        0      185 2023-04-05 22:53:31.000000 ezstools-2.3/ezstools/__init__.py
--rw-rw-rw-   0        0        0      714 2023-04-05 22:52:24.000000 ezstools-2.3/ezstools/console_utils.py
--rw-rw-rw-   0        0        0     6036 2023-04-05 22:43:57.000000 ezstools-2.3/ezstools/custom_iterables.py
--rw-rw-rw-   0        0        0     1524 2021-11-16 00:24:08.000000 ezstools-2.3/ezstools/errorshelp.py
--rw-rw-rw-   0        0        0     1919 2023-04-05 22:51:37.000000 ezstools-2.3/ezstools/funcs.py
--rw-rw-rw-   0        0        0    11247 2022-07-25 16:30:19.000000 ezstools-2.3/ezstools/html_slice.py
--rw-rw-rw-   0        0        0     9064 2022-05-30 12:31:38.000000 ezstools-2.3/ezstools/json_tools.py
--rw-rw-rw-   0        0        0      330 2022-11-12 14:50:00.000000 ezstools-2.3/ezstools/module_tools.py
--rw-rw-rw-   0        0        0     1964 2022-05-30 12:28:59.000000 ezstools-2.3/ezstools/random_generator.py
--rw-rw-rw-   0        0        0     2027 2022-11-10 21:58:33.000000 ezstools-2.3/ezstools/simple_kv.py
--rw-rw-rw-   0        0        0     2927 2023-04-05 22:49:13.000000 ezstools-2.3/ezstools/string_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-05 23:06:39.772069 ezstools-2.3/ezstools.egg-info/
--rw-rw-rw-   0        0        0     2512 2023-04-05 23:06:38.000000 ezstools-2.3/ezstools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2023-04-05 23:06:38.000000 ezstools-2.3/ezstools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 23:06:38.000000 ezstools-2.3/ezstools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-05 23:06:38.000000 ezstools-2.3/ezstools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-05 23:06:38.000000 ezstools-2.3/ezstools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 23:06:39.778054 ezstools-2.3/setup.cfg
--rw-rw-rw-   0        0        0     1334 2023-04-05 22:52:42.000000 ezstools-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:30:04.968792 ezstools-2.4/
+-rw-rw-rw-   0        0        0     2546 2023-04-11 21:30:04.966797 ezstools-2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2255 2023-04-05 23:05:59.000000 ezstools-2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:30:04.913975 ezstools-2.4/ezstools/
+-rw-rw-rw-   0        0        0      177 2023-04-11 20:47:41.000000 ezstools-2.4/ezstools/__init__.py
+-rw-rw-rw-   0        0        0      714 2023-04-05 22:52:24.000000 ezstools-2.4/ezstools/console_utils.py
+-rw-rw-rw-   0        0        0     1524 2021-11-16 00:24:08.000000 ezstools-2.4/ezstools/errorshelp.py
+-rw-rw-rw-   0        0        0     1919 2023-04-05 22:51:37.000000 ezstools-2.4/ezstools/funcs.py
+-rw-rw-rw-   0        0        0    11247 2022-07-25 16:30:19.000000 ezstools-2.4/ezstools/html_slice.py
+-rw-rw-rw-   0        0        0     6230 2023-04-11 21:28:35.000000 ezstools-2.4/ezstools/iterator.py
+-rw-rw-rw-   0        0        0     9064 2022-05-30 12:31:38.000000 ezstools-2.4/ezstools/json_tools.py
+-rw-rw-rw-   0        0        0      330 2022-11-12 14:50:00.000000 ezstools-2.4/ezstools/module_tools.py
+-rw-rw-rw-   0        0        0     1964 2022-05-30 12:28:59.000000 ezstools-2.4/ezstools/random_generator.py
+-rw-rw-rw-   0        0        0     2027 2022-11-10 21:58:33.000000 ezstools-2.4/ezstools/simple_kv.py
+-rw-rw-rw-   0        0        0     3565 2023-04-11 21:10:19.000000 ezstools-2.4/ezstools/string_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:30:04.952834 ezstools-2.4/ezstools.egg-info/
+-rw-rw-rw-   0        0        0     2546 2023-04-11 21:30:04.000000 ezstools-2.4/ezstools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-04-11 21:30:04.000000 ezstools-2.4/ezstools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:30:04.000000 ezstools-2.4/ezstools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-11 21:30:04.000000 ezstools-2.4/ezstools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-11 21:30:04.000000 ezstools-2.4/ezstools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:30:04.969791 ezstools-2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1363 2023-04-11 21:25:52.000000 ezstools-2.4/setup.py
```

### Comparing `ezstools-2.3/PKG-INFO` & `ezstools-2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ezstools
-Version: 2.3
-Summary: Libreria Multi proposito, con modulos variados
+Version: 2.4
+Summary: Libreria Multi proposito, con modulos variados para ayudar con ciertos problemas
 Home-page: 
 Author: Hendrick Y. "NoVa
 Author-email: hendrickrodriguez.nova@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # ezstools
```

### Comparing `ezstools-2.3/README.md` & `ezstools-2.4/README.md`

 * *Files identical despite different names*

### Comparing `ezstools-2.3/ezstools/console_utils.py` & `ezstools-2.4/ezstools/console_utils.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.3/ezstools/errorshelp.py` & `ezstools-2.4/ezstools/errorshelp.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.3/ezstools/funcs.py` & `ezstools-2.4/ezstools/funcs.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.3/ezstools/html_slice.py` & `ezstools-2.4/ezstools/html_slice.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.3/ezstools/json_tools.py` & `ezstools-2.4/ezstools/json_tools.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.3/ezstools/random_generator.py` & `ezstools-2.4/ezstools/random_generator.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.3/ezstools/simple_kv.py` & `ezstools-2.4/ezstools/simple_kv.py`

 * *Files identical despite different names*

### Comparing `ezstools-2.3/ezstools.egg-info/PKG-INFO` & `ezstools-2.4/ezstools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ezstools
-Version: 2.3
-Summary: Libreria Multi proposito, con modulos variados
+Version: 2.4
+Summary: Libreria Multi proposito, con modulos variados para ayudar con ciertos problemas
 Home-page: 
 Author: Hendrick Y. "NoVa
 Author-email: hendrickrodriguez.nova@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # ezstools
```

### Comparing `ezstools-2.3/setup.py` & `ezstools-2.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import pathlib
 from setuptools import find_packages, setup
+from ezstools.json_tools import open_json
+
+with open_json("./data.json", mode="r") as data:
+    VERSION = data["version"]
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '2.3' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'ezstools' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Hendrick Y. "NoVa' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'hendrickrodriguez.nova@gmail.com' #Modificar con vuestros datos
 URL = '' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
-DESCRIPTION = 'Libreria Multi proposito, con modulos variados' #Descripción corta
+DESCRIPTION = 'Libreria Multi proposito, con modulos variados para ayudar con ciertos problemas' #Descripción corta
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8') #Referencia al documento README con una descripción más elaborada
 LONG_DESC_TYPE = "text/markdown"
 
 
 #Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
     "datetime", "pyenchant", "importlib", "pick"
```

