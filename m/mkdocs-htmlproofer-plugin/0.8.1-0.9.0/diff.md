# Comparing `tmp/mkdocs-htmlproofer-plugin-0.8.1.tar.gz` & `tmp/mkdocs-htmlproofer-plugin-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mkdocs-htmlproofer-plugin-0.8.1.tar", last modified: Fri Oct  7 12:25:08 2022, max compression
+gzip compressed data, was "dist/mkdocs-htmlproofer-plugin-0.9.0.tar", last modified: Fri Oct  7 12:31:39 2022, max compression
```

## Comparing `mkdocs-htmlproofer-plugin-0.8.1.tar` & `mkdocs-htmlproofer-plugin-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tianlzhang (110523479) 110523479        0 2022-10-07 12:25:08.000000 mkdocs-htmlproofer-plugin-0.8.1/
--rw-r--r--   0 tianlzhang (110523479) 110523479     4998 2022-10-07 12:25:08.000000 mkdocs-htmlproofer-plugin-0.8.1/PKG-INFO
--rw-r--r--   0 tianlzhang (110523479) 110523479     3148 2021-09-18 01:12:34.000000 mkdocs-htmlproofer-plugin-0.8.1/README.md
-drwxr-xr-x   0 tianlzhang (110523479) 110523479        0 2022-10-07 12:25:08.000000 mkdocs-htmlproofer-plugin-0.8.1/htmlproofer/
--rw-r--r--   0 tianlzhang (110523479) 110523479        0 2021-09-18 01:12:34.000000 mkdocs-htmlproofer-plugin-0.8.1/htmlproofer/__init__.py
--rw-r--r--   0 tianlzhang (110523479) 110523479     7466 2022-10-07 12:19:06.000000 mkdocs-htmlproofer-plugin-0.8.1/htmlproofer/plugin.py
-drwxr-xr-x   0 tianlzhang (110523479) 110523479        0 2022-10-07 12:25:08.000000 mkdocs-htmlproofer-plugin-0.8.1/mkdocs_htmlproofer_plugin.egg-info/
--rw-r--r--   0 tianlzhang (110523479) 110523479     4998 2022-10-07 12:25:08.000000 mkdocs-htmlproofer-plugin-0.8.1/mkdocs_htmlproofer_plugin.egg-info/PKG-INFO
--rw-r--r--   0 tianlzhang (110523479) 110523479      360 2022-10-07 12:25:08.000000 mkdocs-htmlproofer-plugin-0.8.1/mkdocs_htmlproofer_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 tianlzhang (110523479) 110523479        1 2022-10-07 12:25:08.000000 mkdocs-htmlproofer-plugin-0.8.1/mkdocs_htmlproofer_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 tianlzhang (110523479) 110523479       69 2022-10-07 12:25:08.000000 mkdocs-htmlproofer-plugin-0.8.1/mkdocs_htmlproofer_plugin.egg-info/entry_points.txt
--rw-r--r--   0 tianlzhang (110523479) 110523479       51 2022-10-07 12:25:08.000000 mkdocs-htmlproofer-plugin-0.8.1/mkdocs_htmlproofer_plugin.egg-info/requires.txt
--rw-r--r--   0 tianlzhang (110523479) 110523479       12 2022-10-07 12:25:08.000000 mkdocs-htmlproofer-plugin-0.8.1/mkdocs_htmlproofer_plugin.egg-info/top_level.txt
--rw-r--r--   0 tianlzhang (110523479) 110523479       38 2022-10-07 12:25:08.000000 mkdocs-htmlproofer-plugin-0.8.1/setup.cfg
--rw-r--r--   0 tianlzhang (110523479) 110523479     1444 2022-10-07 12:21:58.000000 mkdocs-htmlproofer-plugin-0.8.1/setup.py
+drwxr-xr-x   0 tianlzhang (110523479) 110523479        0 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/
+-rw-r--r--   0 tianlzhang (110523479) 110523479     4998 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/PKG-INFO
+-rw-r--r--   0 tianlzhang (110523479) 110523479     3148 2021-09-18 01:12:34.000000 mkdocs-htmlproofer-plugin-0.9.0/README.md
+drwxr-xr-x   0 tianlzhang (110523479) 110523479        0 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/htmlproofer/
+-rw-r--r--   0 tianlzhang (110523479) 110523479        0 2021-09-18 01:12:34.000000 mkdocs-htmlproofer-plugin-0.9.0/htmlproofer/__init__.py
+-rw-r--r--   0 tianlzhang (110523479) 110523479     7480 2022-10-07 12:29:09.000000 mkdocs-htmlproofer-plugin-0.9.0/htmlproofer/plugin.py
+drwxr-xr-x   0 tianlzhang (110523479) 110523479        0 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/
+-rw-r--r--   0 tianlzhang (110523479) 110523479     4998 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 tianlzhang (110523479) 110523479      360 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 tianlzhang (110523479) 110523479        1 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 tianlzhang (110523479) 110523479       69 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 tianlzhang (110523479) 110523479       51 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/requires.txt
+-rw-r--r--   0 tianlzhang (110523479) 110523479       12 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/top_level.txt
+-rw-r--r--   0 tianlzhang (110523479) 110523479       38 2022-10-07 12:31:39.000000 mkdocs-htmlproofer-plugin-0.9.0/setup.cfg
+-rw-r--r--   0 tianlzhang (110523479) 110523479     1444 2022-10-07 12:30:55.000000 mkdocs-htmlproofer-plugin-0.9.0/setup.py
```

### Comparing `mkdocs-htmlproofer-plugin-0.8.1/PKG-INFO` & `mkdocs-htmlproofer-plugin-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-htmlproofer-plugin
-Version: 0.8.1
+Version: 0.9.0
 Summary: A MkDocs plugin that validates URL in rendered HTML files
 Home-page: https://github.com/manuzhang/mkdocs-htmlproofer-plugin
 Author: Manu Zhang
 Author-email: owenzhang1990@gmail.com
 License: MIT
 Description: # mkdocs-htmlproofer-plugin [![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-htmlproofer-plugin.svg)](https://pypi.org/project/mkdocs-htmlproofer-plugin)
```

### Comparing `mkdocs-htmlproofer-plugin-0.8.1/README.md` & `mkdocs-htmlproofer-plugin-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-htmlproofer-plugin-0.8.1/htmlproofer/plugin.py` & `mkdocs-htmlproofer-plugin-0.9.0/htmlproofer/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     for local in ('localhost', '127.0.0.1', 'app_server')
 ]
 
 urllib3.disable_warnings()
 
 
 class HtmlProoferPlugin(BasePlugin):
-    files: Files = None
+    files: Files
 
     config_scheme = (
         ("enabled", config_options.Type(bool, default=True)),
         ('raise_error', config_options.Type(bool, default=False)),
         ('raise_error_excludes', config_options.Type(dict, default={})),
         ('validate_external_urls', config_options.Type(bool, default=True)),
         ('validate_rendered_template', config_options.Type(bool, default=False)),
@@ -59,15 +59,15 @@
         if not self.config['enabled']:
             return
 
         use_directory_urls = config.data["use_directory_urls"]
 
         # Optimization: only parse links and headings
         # li, sup are used for footnotes
-        strainer = SoupStrainer(('a', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'li', 'sup'))
+        strainer = SoupStrainer(('a', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'li', 'sup', 'img'))
 
         content = output_content if self.config['validate_rendered_template'] else page.content
         soup = BeautifulSoup(content, 'lxml', parse_only=strainer)
 
         all_element_ids = set(tag['id'] for tag in soup.select('[id]'))
         all_element_ids.add('')  # Empty anchor is commonly used, but not real
         for a in soup.find_all('a', href=True):
@@ -127,15 +127,15 @@
     @staticmethod
     def find_target_markdown(url: str, src_path: str, files: Files) -> Optional[str]:
         """From a built URL, find the original Markdown source from the project that built it."""
 
         # Handle relative links by concatenating the source dir with the destination path
         search = os.path.normpath(str(pathlib.Path(src_path).parent / pathlib.Path(url)))
         for file in files.src_paths.values():  # type: File
-            if file.url == search:
+            if file.url == search and file.page:
                 return file.page.markdown
 
         print(f"Warning: Unable to locate Markdown source file for: {url}", file=sys.stderr)
         return None
 
     @staticmethod
     def contains_anchor(markdown: str, anchor: str) -> bool:
```

### Comparing `mkdocs-htmlproofer-plugin-0.8.1/mkdocs_htmlproofer_plugin.egg-info/PKG-INFO` & `mkdocs-htmlproofer-plugin-0.9.0/mkdocs_htmlproofer_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-htmlproofer-plugin
-Version: 0.8.1
+Version: 0.9.0
 Summary: A MkDocs plugin that validates URL in rendered HTML files
 Home-page: https://github.com/manuzhang/mkdocs-htmlproofer-plugin
 Author: Manu Zhang
 Author-email: owenzhang1990@gmail.com
 License: MIT
 Description: # mkdocs-htmlproofer-plugin [![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-htmlproofer-plugin.svg)](https://pypi.org/project/mkdocs-htmlproofer-plugin)
```

### Comparing `mkdocs-htmlproofer-plugin-0.8.1/setup.py` & `mkdocs-htmlproofer-plugin-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def read(fname: str):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='mkdocs-htmlproofer-plugin',
-    version='0.8.1',
+    version='0.9.0',
     description='A MkDocs plugin that validates URL in rendered HTML files',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown',
     url='https://github.com/manuzhang/mkdocs-htmlproofer-plugin',
     author='Manu Zhang',
     author_email='owenzhang1990@gmail.com',
```

