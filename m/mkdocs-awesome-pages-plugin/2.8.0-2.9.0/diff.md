# Comparing `tmp/mkdocs-awesome-pages-plugin-2.8.0.tar.gz` & `tmp/mkdocs_awesome_pages_plugin-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-awesome-pages-plugin-2.8.0.tar", max compression
+gzip compressed data, was "mkdocs_awesome_pages_plugin-2.9.0.tar", max compression
```

## Comparing `mkdocs-awesome-pages-plugin-2.8.0.tar` & `mkdocs_awesome_pages_plugin-2.9.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1071 2022-07-24 17:43:46.593323 mkdocs-awesome-pages-plugin-2.8.0/LICENSE.md
--rw-r--r--   0        0        0    11600 2022-07-24 17:43:46.593323 mkdocs-awesome-pages-plugin-2.8.0/README.md
--rw-r--r--   0        0        0        0 2022-07-24 17:43:46.593323 mkdocs-awesome-pages-plugin-2.8.0/mkdocs_awesome_pages_plugin/__init__.py
--rw-r--r--   0        0        0     9524 2022-07-24 17:43:46.593323 mkdocs-awesome-pages-plugin-2.8.0/mkdocs_awesome_pages_plugin/meta.py
--rw-r--r--   0        0        0     8650 2022-07-24 17:43:46.593323 mkdocs-awesome-pages-plugin-2.8.0/mkdocs_awesome_pages_plugin/navigation.py
--rw-r--r--   0        0        0      221 2022-07-24 17:43:46.593323 mkdocs-awesome-pages-plugin-2.8.0/mkdocs_awesome_pages_plugin/options.py
--rw-r--r--   0        0        0     4967 2022-07-24 17:43:46.597323 mkdocs-awesome-pages-plugin-2.8.0/mkdocs_awesome_pages_plugin/plugin.py
--rw-r--r--   0        0        0     1209 2022-07-24 17:43:46.597323 mkdocs-awesome-pages-plugin-2.8.0/mkdocs_awesome_pages_plugin/utils.py
--rw-r--r--   0        0        0     1059 2022-07-24 17:43:46.597323 mkdocs-awesome-pages-plugin-2.8.0/pyproject.toml
--rw-r--r--   0        0        0    12962 2022-07-24 17:44:04.331203 mkdocs-awesome-pages-plugin-2.8.0/setup.py
--rw-r--r--   0        0        0    12629 2022-07-24 17:44:04.332285 mkdocs-awesome-pages-plugin-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/LICENSE.md
+-rw-r--r--   0        0        0    12162 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/__init__.py
+-rw-r--r--   0        0        0    10451 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/meta.py
+-rw-r--r--   0        0        0    10039 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/navigation.py
+-rw-r--r--   0        0        0      451 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/options.py
+-rw-r--r--   0        0        0     5194 2023-04-11 20:30:35.429559 mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/plugin.py
+-rw-r--r--   0        0        0     1209 2023-04-11 20:30:35.433559 mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/utils.py
+-rw-r--r--   0        0        0     1056 2023-04-11 20:30:35.433559 mkdocs_awesome_pages_plugin-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0    13240 1970-01-01 00:00:00.000000 mkdocs_awesome_pages_plugin-2.9.0/PKG-INFO
```

### Comparing `mkdocs-awesome-pages-plugin-2.8.0/LICENSE.md` & `mkdocs_awesome_pages_plugin-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-awesome-pages-plugin-2.8.0/README.md` & `mkdocs_awesome_pages_plugin-2.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 > **Note:** This plugin won't do anything if your `mkdocs.yml` defines a `nav` or `pages` entry. To make use of the features listed below, you'll either have to remove the entry completely or [add a `...` entry to it](#combine-custom-navigation--file-structure).
 
 <br/>
 
 ## Installation
 
-> **Note:** This package requires Python >=3.5 and MkDocs version 1.0 or higher.  
+> **Note:** This package requires Python >=3.7 and MkDocs version 1.0 or higher.  
 > If you're still on MkDocs 0.17 use [version 1 of this plugin][github-v1].
 
 Install the package with pip:
 
 ```bash
 pip install mkdocs-awesome-pages-plugin
 ```
@@ -122,14 +122,24 @@
 
 This can be combined with `order` above.
 
 ```yaml
 sort_type: natural
 ```
 
+### Order Navigation By Preference
+
+Create a file named `.pages` in a directory and set the `order_by` attribute to `filename` or `title` to change the order of navigation items.
+
+```yaml
+order_by: title
+```
+
+This can be combined with `order` and/or `sort_type` above. If `order` is not set it will order ascending. If no preference is set, it will order by filename.
+
 ### Collapse Single Nested Pages
 
 > **Note:** This feature is disabled by default. More on how to use it below
 
 If you have directories that only contain a single page, awesome-pages can "collapse" them, so the folder doesn't show up in the navigation.
 
 For example if you have the following file structure:
@@ -376,14 +386,17 @@
 
 ```yaml
 plugins:
     - awesome-pages:
         filename: .index
         collapse_single_pages: true
         strict: false
+        order: asc
+        sort_type: natural
+        order_by: title
 ```
 
 ### `filename`
 
 Name of the file used to configure pages of a directory. Default is `.pages`
 
 ### `collapse_single_pages`
@@ -395,14 +408,18 @@
 Raise errors instead of warnings when:
 
 - `arrange` entries cannot be found
 - `nav` entries cannot be found
 
 Default is `true`
 
+### `order`, `sort_type` and `order_by`
+
+Global fallback values for the Meta attributes. Default is `None` or `filename`.
+
 <br/>
 
 ## Contributing
 
 From reporting a bug to submitting a pull request: every contribution is appreciated and welcome.
 Report bugs, ask questions and request features using [Github issues][github-issues].
 If you want to contribute to the code of this project, please read the [Contribution Guidelines][contributing].
```

### Comparing `mkdocs-awesome-pages-plugin-2.8.0/mkdocs_awesome_pages_plugin/meta.py` & `mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 class RestType(Enum):
     GLOB = "glob"
     REGEX = "regex"
     ALL = "all"
 
 
 class MetaNavRestItem(MetaNavItem):
-
     _REGEX = r"^\.{3}\s*(?:\|\s*(flat)\s*)?\s*(?:\|\s*(?:(regex|glob)=)?(.*))?"
 
     def __init__(self, value: str):
         super().__init__(value)
 
         match = re.search(self._REGEX, value)
         if match.group(2) is not None:
@@ -97,56 +96,59 @@
             yield self.all
 
     def __len__(self):
         return len(self.patterns) + (1 if self.all is not None else 0)
 
 
 class Meta:
-
     TITLE_ATTRIBUTE = "title"
     NAV_ATTRIBUTE = "nav"
     ARRANGE_ATTRIBUTE = "arrange"
     ARRANGE_REST_TOKEN = "..."
     COLLAPSE_ATTRIBUTE = "collapse"
     COLLAPSE_SINGLE_PAGES_ATTRIBUTE = "collapse_single_pages"
     HIDE_ATTRIBUTE = "hide"
     ORDER_ATTRIBUTE = "order"
     SORT_TYPE_ATTRIBUTE = "sort_type"
+    ORDER_BY_ATTRIBUTE = "order_by"
 
     ORDER_ASC = "asc"
     ORDER_DESC = "desc"
     SORT_NATURAL = "natural"
+    ORDER_BY_FILENAME = "filename"
+    ORDER_BY_TITLE = "title"
 
     def __init__(
         self,
         *,
         title: Optional[str] = None,
         arrange: Optional[List[str]] = None,
         nav: Optional[List[MetaNavItem]] = None,
         path: Optional[str] = None,
         collapse: bool = None,
         collapse_single_pages: bool = None,
         hide: bool = None,
         order: Optional[str] = None,
         sort_type: Optional[str] = None,
+        order_by: Optional[str] = None,
     ):
-
         if nav is None and arrange is not None:
             nav = [MetaNavItem.from_yaml(value, path) for value in arrange]
             if MetaNavRestItem("...") not in nav:
                 nav.append(MetaNavRestItem("..."))
 
         self.title = title
         self.nav = nav
         self.path = path
         self.collapse = collapse
         self.collapse_single_pages = collapse_single_pages
         self.hide = hide
         self.order = order
         self.sort_type = sort_type
+        self.order_by = order_by
 
     @staticmethod
     def try_load_from(path: Optional[str]) -> "Meta":
         if path is None:
             return Meta()
         try:
             return Meta.load_from(path)
@@ -161,14 +163,15 @@
             arrange = contents.get(Meta.ARRANGE_ATTRIBUTE)
             nav = contents.get(Meta.NAV_ATTRIBUTE)
             collapse = contents.get(Meta.COLLAPSE_ATTRIBUTE)
             collapse_single_pages = contents.get(Meta.COLLAPSE_SINGLE_PAGES_ATTRIBUTE)
             hide = contents.get(Meta.HIDE_ATTRIBUTE)
             order = contents.get(Meta.ORDER_ATTRIBUTE)
             sort_type = contents.get(Meta.SORT_TYPE_ATTRIBUTE)
+            order_by = contents.get(Meta.ORDER_BY_ATTRIBUTE)
 
             if title is not None:
                 if not isinstance(title, str):
                     raise TypeError(
                         'Expected "{attribute}" attribute to be a string - got {type} [{context}]'.format(
                             attribute=Meta.TITLE_ATTRIBUTE,
                             type=type(title),
@@ -241,18 +244,33 @@
                 if sort_type != Meta.SORT_NATURAL:
                     raise TypeError(
                         'Expected "{attribute}" to be "natural" - got "{sort_type}" [{context}]'.format(
                             attribute=Meta.SORT_TYPE_ATTRIBUTE, sort_type=sort_type, context=path
                         )
                     )
 
+            if order_by is not None:
+                if order_by != Meta.ORDER_BY_TITLE and order_by != Meta.ORDER_BY_FILENAME:
+                    raise TypeError(
+                        'Expected "{attribute}" attribute to be one of {those} - got "{order_by}" [{context}]'.format(
+                            attribute=Meta.ORDER_BY_ATTRIBUTE,
+                            those=[
+                                Meta.ORDER_BY_FILENAME,
+                                Meta.ORDER_BY_TITLE,
+                            ],
+                            order_by=order_by,
+                            context=path,
+                        )
+                    )
+
             return Meta(
                 title=title,
                 arrange=arrange,
                 nav=nav,
                 path=path,
                 collapse=collapse,
                 collapse_single_pages=collapse_single_pages,
                 hide=hide,
                 order=order,
                 sort_type=sort_type,
+                order_by=order_by,
             )
```

### Comparing `mkdocs-awesome-pages-plugin-2.8.0/mkdocs_awesome_pages_plugin/navigation.py` & `mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/navigation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import warnings
 from pathlib import Path
+
+import mkdocs.utils
+import mkdocs.utils.meta
 from natsort import natsort_keygen
-from typing import List, Optional, Union, Set
+from typing import List, Optional, Union, Set, Dict
 
 from mkdocs.structure.nav import (
     Navigation as MkDocsNavigation,
     Section,
     Link,
     _add_parent_links,
     _add_previous_and_next_links,
@@ -75,20 +78,32 @@
                 if item is None:
                     continue
             result.append(item)
 
         return result
 
     def _order(self, items: List[NavigationItem], meta: Meta):
-        order, sort_type = meta.order, meta.sort_type
-        if order is None and sort_type is None:
+        if len(items) < 2:
+            return
+
+        order = meta.order or self.options.order
+        sort_type = meta.sort_type or self.options.sort_type
+        order_by = meta.order_by or self.options.order_by
+
+        if order is None and sort_type is None and order_by is None:
             return
-        key = lambda i: basename(self._get_item_path(i))
+
+        if order_by == Meta.ORDER_BY_TITLE:
+            key = lambda i: get_title(i)
+        else:
+            key = lambda i: basename(self._get_item_path(i))
+
         if sort_type == Meta.SORT_NATURAL:
             key = natsort_keygen(key)
+
         items.sort(key=key, reverse=order == Meta.ORDER_DESC)
 
     def _nav(self, items: List[NavigationItem], meta: Meta) -> List[NavigationItem]:
         if meta.nav is None:
             return items
 
         items_by_basename = {basename(self._get_item_path(item)): item for item in items}
@@ -202,40 +217,42 @@
         self,
         items: List[NavigationItem],
         options: Options,
         docs_dir: str,
         explicit_sections: Set[Section],
     ):
         self.options = options
-        self.sections = {}
+        self.sections: Dict[Section, Meta] = {}
         self.docs_dir = docs_dir
         self.explicit_sections = explicit_sections
 
-        root_path = self._gather_metadata(items)
-        self.root = Meta.try_load_from(join_paths(root_path, self.options.filename))
+        self.root: Meta = self._gather_metadata(items)
 
-    def _gather_metadata(self, items: List[NavigationItem]) -> Optional[str]:
-        paths = []
+    def _gather_metadata(self, items: List[NavigationItem]) -> Meta:
+        paths: List[str] = []
         for item in items:
             if isinstance(item, Page):
                 if Path(self.docs_dir) in Path(item.file.abs_src_path).parents:
                     paths.append(item.file.abs_src_path)
             elif isinstance(item, Section):
-                section_dir = self._gather_metadata(item.children)
+                section_meta = self._gather_metadata(item.children)
+
                 if item in self.explicit_sections:
                     self.sections[item] = Meta()
-                else:
-                    if section_dir is not None:
-                        paths.append(section_dir)
-                    self.sections[item] = Meta.try_load_from(join_paths(section_dir, self.options.filename))
+                    continue
+
+                if section_meta.path is not None:
+                    paths.append(dirname(section_meta.path))
+
+                self.sections[item] = section_meta
 
-        return self._common_dirname(paths)
+        return Meta.try_load_from(join_paths(self._common_dirname(paths), self.options.filename))
 
     @staticmethod
-    def _common_dirname(paths: List[Optional[str]]) -> Optional[str]:
+    def _common_dirname(paths: List[str]) -> Optional[str]:
         if paths:
             dirnames = [dirname(path) for path in paths]
             if len(set(dirnames)) == 1:
                 return dirnames[0]
 
 
 # Copy of mkdocs.structure.nav._get_by_type with fix for nested sections
@@ -244,7 +261,42 @@
     ret = []
     for item in nav:
         if isinstance(item, T):
             ret.append(item)
         if item.children:
             ret.extend(get_by_type(item.children, T))
     return ret
+
+
+# Copy of mkdocs.structure.pages.Page._set_title and Page.read_source
+def get_title(item: NavigationItem) -> str:
+    if item.title is not None:
+        return item.title
+
+    if not isinstance(item, Page):
+        return str(item.title)
+
+    try:
+        with open(item.file.abs_src_path, encoding="utf-8-sig", errors="strict") as f:
+            source = f.read()
+    except OSError:
+        raise OSError(f"File not found: {item.file.src_path}")
+    except ValueError:
+        raise ValueError(f"Encoding error reading file: {item.file.src_path}")
+
+    page_markdown, page_meta = mkdocs.utils.meta.get_data(source)
+
+    if "title" in page_meta:
+        return page_meta["title"]
+
+    title = mkdocs.utils.get_markdown_title(page_markdown)
+
+    if title is None:
+        if item.is_homepage:
+            title = "Home"
+        else:
+            title = item.file.name.replace("-", " ").replace("_", " ")
+            # Capitalize if the filename was all lowercase, otherwise leave it as-is.
+            if title.lower() == title:
+                title = title.capitalize()
+
+    return title
```

### Comparing `mkdocs-awesome-pages-plugin-2.8.0/mkdocs_awesome_pages_plugin/plugin.py` & `mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,22 +24,24 @@
             "plugins. It defines an on_nav handler that will be overridden by awesome-pages in some circumstances.".format(
                 plugin_name=plugin_name
             )
         )
 
 
 class AwesomePagesPlugin(BasePlugin):
-
     DEFAULT_META_FILENAME = ".pages"
     REST_PLACEHOLDER = "AWESOME_PAGES_REST"
 
     config_scheme = (
         ("filename", config_options.Type(str, default=DEFAULT_META_FILENAME)),
         ("collapse_single_pages", config_options.Type(bool, default=False)),
         ("strict", config_options.Type(bool, default=True)),
+        ("order", config_options.Choice(["asc", "desc"], default=None)),
+        ("sort_type", config_options.Choice(["natural"], default=None)),
+        ("order_by", config_options.Choice(["filename", "title"], default=None)),
     )
 
     def __init__(self):
         self.nav_config_with_rest = None
         self.rest_items = RestItemList()
         self.rest_blocks = {}
```

### Comparing `mkdocs-awesome-pages-plugin-2.8.0/mkdocs_awesome_pages_plugin/utils.py` & `mkdocs_awesome_pages_plugin-2.9.0/mkdocs_awesome_pages_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs-awesome-pages-plugin-2.8.0/pyproject.toml` & `mkdocs_awesome_pages_plugin-2.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-awesome-pages-plugin"
-version = "2.8.0"
+version = "2.9.0"
 description = "An MkDocs plugin that simplifies configuring page titles and their order"
 authors = ["Lukas Geiter <info@lukasgeiter.com>"]
 repository = "https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin/"
 readme = "README.md"
 license = "MIT"
 keywords = ["mkdocs", "python", "markdown", "wiki"]
 classifiers = [
@@ -14,24 +14,24 @@
 ]
 exclude = ["mkdocs_awesome_pages_plugin/tests"]
 
 [tool.poetry.plugins."mkdocs.plugins"]
 awesome-pages = "mkdocs_awesome_pages_plugin.plugin:AwesomePagesPlugin"
 
 [tool.poetry.dependencies]
-python = ">=3.6.2"
+python = ">=3.7"
 mkdocs = ">=1"
 wcmatch = ">=7"
 natsort = ">=8.1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 beautifulsoup4 = "^4.10.0"
 mock-open = "^1.4.0"
-black = { extras = ["d"], version = "^21.12b0" }
+black = { extras = ["d"], version = "^23.1.0" }
 
 [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mkdocs-awesome-pages-plugin-2.8.0/PKG-INFO` & `mkdocs_awesome_pages_plugin-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: mkdocs-awesome-pages-plugin
-Version: 2.8.0
+Version: 2.9.0
 Summary: An MkDocs plugin that simplifies configuring page titles and their order
 Home-page: https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin/
 License: MIT
 Keywords: mkdocs,python,markdown,wiki
 Author: Lukas Geiter
 Author-email: info@lukasgeiter.com
-Requires-Python: >=3.6.2
+Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: mkdocs (>=1)
 Requires-Dist: natsort (>=8.1.0)
 Requires-Dist: wcmatch (>=7)
 Project-URL: Repository, https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin/
 Description-Content-Type: text/markdown
 
 # MkDocs Awesome Pages Plugin [![Tests Status][status-tests-badge]][status-tests-link]
@@ -31,15 +32,15 @@
 
 > **Note:** This plugin won't do anything if your `mkdocs.yml` defines a `nav` or `pages` entry. To make use of the features listed below, you'll either have to remove the entry completely or [add a `...` entry to it](#combine-custom-navigation--file-structure).
 
 <br/>
 
 ## Installation
 
-> **Note:** This package requires Python >=3.5 and MkDocs version 1.0 or higher.  
+> **Note:** This package requires Python >=3.7 and MkDocs version 1.0 or higher.  
 > If you're still on MkDocs 0.17 use [version 1 of this plugin][github-v1].
 
 Install the package with pip:
 
 ```bash
 pip install mkdocs-awesome-pages-plugin
 ```
@@ -147,14 +148,24 @@
 
 This can be combined with `order` above.
 
 ```yaml
 sort_type: natural
 ```
 
+### Order Navigation By Preference
+
+Create a file named `.pages` in a directory and set the `order_by` attribute to `filename` or `title` to change the order of navigation items.
+
+```yaml
+order_by: title
+```
+
+This can be combined with `order` and/or `sort_type` above. If `order` is not set it will order ascending. If no preference is set, it will order by filename.
+
 ### Collapse Single Nested Pages
 
 > **Note:** This feature is disabled by default. More on how to use it below
 
 If you have directories that only contain a single page, awesome-pages can "collapse" them, so the folder doesn't show up in the navigation.
 
 For example if you have the following file structure:
@@ -401,14 +412,17 @@
 
 ```yaml
 plugins:
     - awesome-pages:
         filename: .index
         collapse_single_pages: true
         strict: false
+        order: asc
+        sort_type: natural
+        order_by: title
 ```
 
 ### `filename`
 
 Name of the file used to configure pages of a directory. Default is `.pages`
 
 ### `collapse_single_pages`
@@ -420,14 +434,18 @@
 Raise errors instead of warnings when:
 
 - `arrange` entries cannot be found
 - `nav` entries cannot be found
 
 Default is `true`
 
+### `order`, `sort_type` and `order_by`
+
+Global fallback values for the Meta attributes. Default is `None` or `filename`.
+
 <br/>
 
 ## Contributing
 
 From reporting a bug to submitting a pull request: every contribution is appreciated and welcome.
 Report bugs, ask questions and request features using [Github issues][github-issues].
 If you want to contribute to the code of this project, please read the [Contribution Guidelines][contributing].
```

