# Comparing `tmp/appstream-python-0.5.1.tar.gz` & `tmp/appstream-python-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appstream-python-0.5.1.tar", last modified: Thu Mar 16 15:45:08 2023, max compression
+gzip compressed data, was "appstream-python-0.6.tar", last modified: Tue Apr 11 13:01:28 2023, max compression
```

## Comparing `appstream-python-0.5.1.tar` & `appstream-python-0.6.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 15:45:08.423513 appstream-python-0.5.1/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-03-16 15:44:36.000000 appstream-python-0.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       71 2023-03-16 15:44:36.000000 appstream-python-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1404 2023-03-16 15:45:08.423513 appstream-python-0.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      112 2023-03-16 15:44:36.000000 appstream-python-0.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 15:45:08.423513 appstream-python-0.5.1/appstream_python/
--rw-r--r--   0 root         (0) root         (0)     2777 2023-03-16 15:44:36.000000 appstream-python-0.5.1/appstream_python/Collection.py
--rw-r--r--   0 root         (0) root         (0)    27664 2023-03-16 15:44:36.000000 appstream-python-0.5.1/appstream_python/Component.py
--rw-r--r--   0 root         (0) root         (0)     1933 2023-03-16 15:44:36.000000 appstream-python-0.5.1/appstream_python/StandardConstants.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-03-16 15:44:36.000000 appstream-python-0.5.1/appstream_python/__init__.py
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-16 15:44:36.000000 appstream-python-0.5.1/appstream_python/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 15:45:08.423513 appstream-python-0.5.1/appstream_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1404 2023-03-16 15:45:08.000000 appstream-python-0.5.1/appstream_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-03-16 15:45:08.000000 appstream-python-0.5.1/appstream_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 15:45:08.000000 appstream-python-0.5.1/appstream_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-03-16 15:45:08.000000 appstream-python-0.5.1/appstream_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-03-16 15:45:08.000000 appstream-python-0.5.1/appstream_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1475 2023-03-16 15:44:36.000000 appstream-python-0.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-16 15:45:08.423513 appstream-python-0.5.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 15:45:08.423513 appstream-python-0.5.1/tests/
--rw-r--r--   0 root         (0) root         (0)      983 2023-03-16 15:44:36.000000 appstream-python-0.5.1/tests/test_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:01:28.729500 appstream-python-0.6/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-04-11 13:00:59.000000 appstream-python-0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       71 2023-04-11 13:00:59.000000 appstream-python-0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-04-11 13:01:28.729500 appstream-python-0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      112 2023-04-11 13:00:59.000000 appstream-python-0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:01:28.729500 appstream-python-0.6/appstream_python/
+-rw-r--r--   0 root         (0) root         (0)     2777 2023-04-11 13:00:59.000000 appstream-python-0.6/appstream_python/Collection.py
+-rw-r--r--   0 root         (0) root         (0)    35396 2023-04-11 13:00:59.000000 appstream-python-0.6/appstream_python/Component.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-04-11 13:00:59.000000 appstream-python-0.6/appstream_python/StandardConstants.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-11 13:00:59.000000 appstream-python-0.6/appstream_python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-04-11 13:00:59.000000 appstream-python-0.6/appstream_python/_helper.py
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-11 13:00:59.000000 appstream-python-0.6/appstream_python/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:01:28.729500 appstream-python-0.6/appstream_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-04-11 13:01:28.000000 appstream-python-0.6/appstream_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      512 2023-04-11 13:01:28.000000 appstream-python-0.6/appstream_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 13:01:28.000000 appstream-python-0.6/appstream_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-11 13:01:28.000000 appstream-python-0.6/appstream_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-11 13:01:28.000000 appstream-python-0.6/appstream_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-04-11 13:00:59.000000 appstream-python-0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 13:01:28.729500 appstream-python-0.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:01:28.729500 appstream-python-0.6/tests/
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-04-11 13:00:59.000000 appstream-python-0.6/tests/test_appstream_data.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2023-04-11 13:00:59.000000 appstream-python-0.6/tests/test_description.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-04-11 13:00:59.000000 appstream-python-0.6/tests/test_display_length.py
```

### Comparing `appstream-python-0.5.1/LICENSE` & `appstream-python-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `appstream-python-0.5.1/PKG-INFO` & `appstream-python-0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appstream-python
-Version: 0.5.1
+Version: 0.6
 Summary: A library for dealing with Freedesktop Appstream data
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://appstream-python.readthedocs.io
 Project-URL: Issues, https://codeberg.org/JakobDev/appstream-python/issues
 Project-URL: Source, https://codeberg.org/JakobDev/appstream-python
 Project-URL: Donation, https://ko-fi.com/jakobdev
@@ -13,20 +13,18 @@
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # appstream-python
 
 A library for dealing with Freedesktop Appstream data. This lib is currently in development.
```

### Comparing `appstream-python-0.5.1/appstream_python/Collection.py` & `appstream-python-0.6/appstream_python/Collection.py`

 * *Files identical despite different names*

### Comparing `appstream-python-0.5.1/appstream_python/Component.py` & `appstream-python-0.6/appstream_python/Component.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,38 @@
-from typing import Optional, Literal, TypedDict, Union
+from typing import Any, Optional, Literal, TypedDict, Union
+from ._helper import assert_func
 from .StandardConstants import *
 from lxml import etree
 import datetime
 import io
 import os
 
 
+_XML_LANG = "{http://www.w3.org/XML/1998/namespace}lang"
+
+
+def _compare_relation_value(operator: RELATION_COMPARISON_OPERATOR_LITERAL, first: Any, second: Any) -> bool:
+    "Matches 2 relation values with the given Operator"
+    match operator:
+        case "eq":
+            return first == second
+        case "ne":
+            return first != second
+        case "lt":
+            return first < second
+        case "gt":
+            return first > second
+        case "le":
+            return first <= second
+        case "ge":
+            return first >= second
+        case _:
+            raise ValueError(f"Invalid Operator {operator}")
+
+
 class InternetRelationDict(TypedDict):
     "the type for the content of the Internet attribute"
     value: INTERNET_RELATION_VALUE_LITERAL
     bandwidth_mbitps: Optional[int]
 
 
 class TranslateableTag:
@@ -26,14 +49,18 @@
         """Sets the untranslated text"""
         self._text = text
 
     def get_translated_text(self, lang: str) -> Optional[str]:
         """Returns the translated text"""
         return self._translations.get(lang, None)
 
+    def get_translated_text_default(self, lang: str) -> Optional[str]:
+        """Returns the translated text. Returns the default text, if the translation does not exists"""
+        return self._translations.get(lang, self._text)
+
     def set_translated_text(self, lang: str, text: str) -> None:
         """Sets the translated text"""
         self._translations[lang] = text
 
     def get_available_languages(self) -> list[str]:
         """Returns a list with all languages of the tag"""
         return list(self._translations.keys())
@@ -64,47 +91,72 @@
     def __repr__(self) -> str:
         return f"<TranslateableTag default='{self._text}'>"
 
 
 class TranslateableList:
     "Represents a translatable list"
     def __init__(self) -> None:
-        self.default_list = []
-        self.translated_lists = {}
+        self._translated_data: dict[str, dict[str, str]] = {}
+        self._translated_lists: dict[str, list[str]] = {}
 
     def get_default_list(self) -> list[str]:
         "Returns a list with the default items"
-        return self.default_list
+        return list(self._translated_data.keys())
+
+    def get_translated_list(self, lang: str) -> list[str]:
+        "Returns the translated list for the given language"
+        if lang in self._translated_lists:
+            return self._translated_lists[lang]
+
+        return_list: list[str] = []
+        for untranslated_text, translations in self._translated_data.items():
+            return_list.append(translations.get(lang, untranslated_text))
+        return return_list
 
     def load_tag(self, tag: etree.Element) -> None:
-        "Loads a Tag Only for internal use."
+        "Loads an Tag. Only for internal use."
         if tag.get("{http://www.w3.org/XML/1998/namespace}lang") is None:
+            current_text = ""
             for i in tag.getchildren():
-                if i.get("{http://www.w3.org/XML/1998/namespace}lang") is None:
-                    self.default_list.append(i.text.strip())
+                if i.get(_XML_LANG) is None:
+                    current_text = i.text.strip()
+                    self._translated_data[current_text] = {}
                 else:
-                    if i.get("{http://www.w3.org/XML/1998/namespace}lang") not in self.translated_lists:
-                        self.translated_lists[i.get("{http://www.w3.org/XML/1998/namespace}lang")] = []
-                    self.translated_lists[i.get("{http://www.w3.org/XML/1998/namespace}lang")].append(i.text.strip())
+                    self._translated_data[current_text][i.get(_XML_LANG)] = i.text.strip()
         else:
-            if tag.get("{http://www.w3.org/XML/1998/namespace}lang") not in self.translated_lists:
-                self.translated_lists[tag.get("{http://www.w3.org/XML/1998/namespace}lang")] = []
+            if tag.get("{http://www.w3.org/XML/1998/namespace}lang") not in self._translated_lists:
+                self._translated_lists[tag.get("{http://www.w3.org/XML/1998/namespace}lang")] = []
             for i in tag.getchildren():
-                self.translated_lists[tag.get("{http://www.w3.org/XML/1998/namespace}lang")].append(i.text.strip())
+                self._translated_lists[tag.get("{http://www.w3.org/XML/1998/namespace}lang")].append(i.text.strip())
 
     def write_all_tag(self, parent_tag: etree.Element, tag_name: str) -> None:
-        "Writes the XML tags. Onyl for internal use."
-        for i in range(len(self.default_list)):
+        "Writes the XML tags. Onnly for internal use."
+        for untranslated_text, translations in self._translated_data.items():
             default_tag = etree.SubElement(parent_tag, tag_name)
-            default_tag.text = self.default_list[i]
+            default_tag.text = untranslated_text
+            for lang, translated_text in translations.items():
+                translated_tag = etree.SubElement(parent_tag, tag_name)
+                translated_tag.set(_XML_LANG, lang)
+                translated_tag.text = translated_text
+
+    def write_untranslated_tags(self, parent_tag: etree.Element, tag_name: str) -> None:
+        "Writes the untranslated XML tags. Onnly for internal use."
+        for untranslated_text in self._translated_data.keys():
+            default_tag = etree.SubElement(parent_tag, tag_name)
+            default_tag.text = untranslated_text
+
+    def write_translated_tags(self, parent_tag: etree.Element, tag_name: str, lang: str) -> None:
+        "Writes the translated XML tags. Onnly for internal use."
+        for untranslated_text, translations in self._translated_data.items():
+            child_tag = etree.SubElement(parent_tag, tag_name)
+            child_tag.text = translations.get(lang, untranslated_text)
 
     def clear(self) -> None:
         """Resets all data"""
-        self.default_list.clear()
-        self.translated_lists.clear()
+        self._translated_data.clear()
 
 
 class DescriptionItem:
     "The Interface for a Description Item"
     def get_type(self) -> Literal["paragraph", "unordered-list", "ordered-list"]:
         "Retutns the Type of the Item"
         return "none"
@@ -117,14 +169,18 @@
         "Get the XML Tag from the Element. Only for internal use."
         raise NotImplementedError()
 
     def get_translated_tag(self, lang: Optional[str]) -> etree.Element:
         "Loads the tag for a given language"
         raise NotImplementedError()
 
+    def to_plain_text(self, lang: Optional[str] = None) -> str:
+        "Returns the content as plain text"
+        raise NotImplementedError()
+
 
 class DescriptionParagraph(DescriptionItem):
     "Represents a paragraph <p> in the Description"
     def __init__(self) -> None:
         self.content = TranslateableTag()
         """The Text of the Paragraph"""
 
@@ -142,48 +198,69 @@
 
     def get_translated_tag(self, lang: Optional[str]) -> etree.Element:
         "Loads the tag for a given language"
         paragraph_tag = etree.Element("p")
         if lang is None:
             paragraph_tag.text = self.content.get_default_text()
         else:
-            paragraph_tag.text = self.content.get_translated_text(lang)
+            paragraph_tag.text = self.content.get_translated_text_default(lang)
         return paragraph_tag
 
+    def to_plain_text(self, lang: Optional[str] = None) -> str:
+        "Returns the content as plain text"
+        return self.content.get_translated_text_default(lang).strip()
+
 
 class DescriptionList(DescriptionItem):
     "Represents a list <ul>/<ol> in the Description"
     def __init__(self, list_type: str) -> None:
         self._list_type = list_type
 
         self.content: TranslateableList = TranslateableList()
         "The list"
 
     def get_type(self) -> Literal["paragraph", "unordered-list", "ordered-list"]:
         "Retutns the Type of the Item"
-        if self.list_type == "ul":
+        if self._list_type == "ul":
             return "unordered-list"
         else:
             return "ordered-list"
 
     def load_tags(self, tag_list: list[etree.Element]) -> None:
-        "Loads teh XML tags into the Elemnt. Only for internal use."
+        "Loads the XML tags into the Elemnt. Only for internal use."
         self.content.load_tag(tag_list)
 
     def get_tags(self, parent_tag: etree.Element) -> None:
         "Get the XML Tag from the Element. Only for internal use."
         list_tag = etree.SubElement(parent_tag, self._list_type)
         self.content.write_all_tag(list_tag, "li")
 
-    def get_translated_tag(self, lang: Optional[str]) -> etree.Element:
+    def get_translated_tag(self, lang: Optional[str] = None) -> etree.Element:
         "Loads the tag for a given language"
         list_tag = etree.Element(self._list_type)
-        self.content.write_all_tag(list_tag, "li")
+        if lang is None:
+            self.content.write_untranslated_tags(list_tag, "li")
+        else:
+            self.content.write_translated_tags(list_tag, "li", lang)
         return list_tag
 
+    def to_plain_text(self, lang: Optional[str] = None) -> str:
+        "Returns the content as plain text"
+        tag_list = self.content.get_translated_list(lang)
+
+        return_text = ""
+        if self.get_type() == "unordered-list":
+            for tag_text in tag_list:
+                return_text += f"• {tag_text}\n"
+        elif self.get_type() == "ordered-list":
+            for count, tag_text in enumerate(tag_list):
+                return_text += f"{count + 1}. {tag_text}\n"
+
+        return return_text.strip()
+
 
 class Description:
     "Represents a <description> tag"
     def __init__(self) -> None:
         self.items: list[DescriptionItem] = []
         """All Description Items"""
 
@@ -219,26 +296,48 @@
 
     def get_tags(self, parent_tag: etree.Element) -> None:
         "Writes a Description tag. Only for internal use."
         description_tag = etree.SubElement(parent_tag, "description")
         for i in self.items:
             i.get_tags(description_tag)
 
-    def to_html(self, lang: Optional[str]) -> str:
+    def to_html(self, lang: Optional[str] = None) -> str:
         "Get the HTML code of the description in the given language"
         description_tag = etree.Element("description")
 
         for i in self.items:
             description_tag.append(i.get_translated_tag(lang))
 
-        text = etree.tostring(description_tag).decode("utf-8")
+        text = etree.tostring(description_tag, pretty_print=True, encoding="utf-8").decode("utf-8")
+
+        # Remove the description tag
         text = text.replace("<description>", "")
         text = text.replace("</description>", "")
         text = text.replace("<description/>", "")
-        text = text.replace("\n", "")
+
+        # Remove the 2 spaces at the start of each line, after we removed the description tag
+        return_text = ""
+        for line in text.splitlines():
+            return_text += line.removeprefix("  ") + "\n"
+
+        return return_text.strip()
+
+    def to_plain_text(self, lang: Optional[str] = None) -> str:
+        """
+        Converts the Description into Plain Text
+
+        :param lang: The language
+        :return: The Description
+        """
+        text = ""
+
+        for i in self.items:
+            text += f"{i.to_plain_text(lang)}\n\n"
+
+        text = text.removesuffix("\n\n")
 
         return text.strip()
 
 
 class Release:
     "Represents a <release> tag"
     def __init__(self) -> None:
@@ -333,14 +432,99 @@
             img = Image()
             img.load_tag(i)
             self.images.append(img)
 
         self.caption.load_tags(tag.findall("caption"))
 
 
+class DisplayLength:
+    "Represents a <display_length> tag"
+    def __init__(self, px: int = 0, compare: Optional[str] = None) -> None:
+        self.px: int = px
+        "The logical pixels"
+
+        self.compare: Optional[str] = compare
+        "Compare"
+
+    def compare_px(self, value: int) -> bool:
+        """
+        Compares the length with the given logical pixels
+
+        :param value: The logical pixels to compare
+        :return: If it is valid
+        """
+        return _compare_relation_value(self.compare, value, self.px)
+
+    def get_tag(self) -> etree.Element:
+        """
+        Returns the XML Tag
+
+        :return: The Tag
+        """
+        tag = etree.Element("display_length")
+        tag.text = str(self.px)
+
+        if self.compare is not None:
+            tag.set("compare", self.compare)
+
+        return tag
+
+    @classmethod
+    def from_tag(cls: "DisplayLength", tag: etree.Element) -> "DisplayLength":
+        "Creates the Object from an XML Tag"
+        display_length = cls()
+
+        try:
+            display_length.px = int(tag.text)
+        except ValueError:
+            display_length.px = cls.string_to_px(tag.text)
+
+        display_length.compare = tag.get("compare")
+
+        return display_length
+
+    @staticmethod
+    def string_to_px(string: str) -> int:
+        """
+        Converts a Lenght String (e.g.small) to logical pixels value
+
+        :param string: The String
+        :raises ValueError: The Length String is invalid
+        :return: The logical pixels  pixels
+        """
+        # https://github.com/ximion/appstream/blob/8d43c78288889d97a3e8502f4a4e777532bb6b04/src/as-relation.c#L418
+        match string:
+            case "xsmall":
+                return 360
+            case "small":
+                return 420
+            case "medium":
+                return 760
+            case "large":
+                return 900
+            case "xlarge":
+                return 1200
+            case _:
+                raise ValueError(f"{string} is not a valid size")
+
+    def __repr__(self) -> str:
+        return f"<AppstreamPythonDisplayLength px={self.px} compare='{self.compare}>'"
+
+    def __eq__(self, value: object) -> bool:
+        if not isinstance(value, DisplayLength):
+            return False
+
+        try:
+            assert_func(self.px == value.px)
+            assert_func(self.compare == value.compare)
+            return True
+        except AssertionError:
+            return False
+
+
 class AppstreamComponent:
     "Represents AppStream Component"
     def __init__(self) -> None:
         self.id: str = ""
         "The component ID"
 
         self.type: str = "desktop"
@@ -393,14 +577,17 @@
 
         self.keywords: TranslateableList = TranslateableList()
         "The Keywords"
 
         self.controls: dict[CONTROL_TYPES_LITERAL, Optional[Literal["requires", "recommends", "supports"]]] = {}
         "The Controls"
 
+        self.display_length: dict[Literal["requires", "recommends", "supports"], list[DisplayLength]] = {}
+        "The Display Length"
+
         self.internet: dict[Literal["requires", "recommends", "supports"], InternetRelationDict] = {}
 
         self.kudos: list[str] = []
         "The Kudos"
 
         self.update_contact: Optional[str] = None
         "The update contact"
@@ -436,14 +623,15 @@
         self.releases.clear()
         self.screenshots.clear
         self.project_group = None
         self.translation.clear()
         self.languages.clear()
         self.keywords.clear()
         self.controls.clear()
+        self.display_length.clear()
         self.internet.clear()
         self.kudos.clear()
         self.update_contact = None
         self.replaces.clear()
         self.suggests.clear()
         self.custom.clear()
         self.extends.clear()
@@ -459,17 +647,23 @@
         lang_list = self.name.get_available_languages() + self.summary.get_available_languages() + self.developer_name.get_available_languages()
         return list(set(lang_list))
 
     def _parse_relation_tag(self, tag: etree.Element) -> None:
         "Parses a relation tag"
         relation = tag.tag
 
-        for i in tag.findall("control"):
-            if i.text.strip() in CONTROL_TYPES:
-                self.controls[i.text.strip()] = relation
+        for control_tag in tag.findall("control"):
+            if control_tag.text.strip() in CONTROL_TYPES:
+                self.controls[control_tag.text.strip()] = relation
+
+        for display_length_tag in tag.findall("display_length"):
+            if relation in self.display_length:
+                self.display_length[relation].append(DisplayLength.from_tag(display_length_tag))
+            else:
+                self.display_length[relation] = [DisplayLength.from_tag(display_length_tag)]
 
         internet_tag = tag.find("internet")
         if internet_tag is not None:
             internet_dict: InternetRelationDict = {"value": internet_tag.text.strip()}
 
             try:
                 internet_dict["bandwidth_mbitps"] = int(internet_tag.get("bandwidth_mbitps"))
@@ -616,32 +810,56 @@
             self.extends.append(i.text.strip())
 
     def load_file(self, path: Union[str, os.PathLike, io.RawIOBase]) -> None:
         """Load an appdata.xml or metainfo.xml file"""
         root = etree.parse(path)
         self.parse_component_tag(root)
 
+    @classmethod
+    def from_file(cls: "AppstreamComponent", path: Union[str, os.PathLike, io.RawIOBase]) -> "AppstreamComponent":
+        "Load an appdata.xml or metainfo.xml file"
+        component = cls()
+        component.load_file(path)
+        return component
+
     def load_bytes(self, data: bytes, encoding: Optional[str] = None) -> None:
         """Load an appdata.xml or metainfo.xml byte string"""
         root = etree.fromstring(data, parser=etree.XMLParser(encoding=encoding))
         self.parse_component_tag(root)
 
+    @classmethod
+    def from_bytes(cls: "AppstreamComponent", data: bytes, encoding: Optional[str] = None) -> "AppstreamComponent":
+        "Load an appdata.xml or metainfo.xml byte string"
+        component = cls()
+        component.load_bytes(data, encoding)
+        return component
+
     def load_string(self, text: str) -> None:
         """Load an appdata.xml or metainfo.xml string"""
         self.load_bytes(text.encode("utf-8"), encoding="utf-8")
 
+    @classmethod
+    def from_string(cls: "AppstreamComponent", text: str) -> "AppstreamComponent":
+        "Load an appdata.xml or metainfo.xml string"
+        component = cls()
+        component.load_string(text)
+        return component
+
     def _get_relation_tag(self, parent_tag: etree.Element, relation: Literal["supports", "recommends", "requires"]) -> None:
         "Craetes a relation tag from the Component."
         relation_tag = etree.SubElement(parent_tag, relation)
 
         for key, value in self.controls.items():
             if key in CONTROL_TYPES and value == relation:
                 control_tag = etree.SubElement(relation_tag, "control")
                 control_tag.text = key
 
+        for display_length in self.display_length.get(relation, []):
+            relation_tag.append(display_length.get_tag())
+
         if relation in self.internet:
             internet_tag = etree.SubElement(relation_tag, "internet")
 
             if self.internet[relation]["bandwidth_mbitps"] is not None:
                 internet_tag.set("bandwidth_mbitps", str(self.internet[relation]["bandwidth_mbitps"]))
 
             internet_tag.text = self.internet[relation]["value"]
@@ -694,14 +912,15 @@
         provides_tag = etree.SubElement(tag, "provides")
         for key, value in self.provides.items():
             if key not in PROVIDES_TYPES:
                 continue
             for i in value:
                 single_provides_tag = etree.SubElement(provides_tag, key)
                 single_provides_tag.text = i
+
         # Don't write empty provides tag
         if len(provides_tag.getchildren()) == 0:
             tag.remove(provides_tag)
 
         if self.project_group:
             project_group_tag = etree.SubElement(tag, "project_group")
             project_group_tag.text = self.project_group
@@ -755,15 +974,15 @@
             extends_tag = etree.SubElement(tag, "extends")
             extends_tag.text = i
 
         return tag
 
     def get_xml_string(self) -> str:
         """Returns the XML data of the Component as string"""
-        return etree.tostring(self.get_component_tag(), pretty_print=True, encoding="utf-8").decode("utf-8")
+        return etree.tostring(self.get_component_tag(), pretty_print=True, encoding="utf-8").decode("utf-8").strip()
 
     def save_file(self, path: str) -> None:
         """Saves the Component as XML file"""
         with open(path, "w", encoding="utf-8") as f:
             f.write(etree.tostring(self.get_component_tag(), pretty_print=True, xml_declaration=True, encoding="utf-8").decode("utf-8"))
 
     def __repr__(self) -> str:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `appstream-python-0.5.1/appstream_python/StandardConstants.py` & `appstream-python-0.6/appstream_python/StandardConstants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 "This module contains constansts for Appstream"
-
 from typing import Literal, get_args
 
 URL_TYPES_LITERAL = Literal[
     "homepage",
     "bugtracker",
     "faq",
     "help",
@@ -56,14 +55,23 @@
     "firmware",
     "python2",
     "python3",
     "dbus",
     "id"
 ]
 
+RELATION_COMPARISON_OPERATOR_LITERAL = Literal[
+    "eq",
+    "ne",
+    "lt",
+    "gt",
+    "le",
+    "ge"
+]
+
 CONTROL_TYPES_LITERAL = Literal[
     "pointing",
     "keyboard",
     "console",
     "tablet",
     "touch",
     "gamepad",
@@ -86,12 +94,15 @@
 
 OARS_VALUE_TYPES = list(get_args(OARS_VALUE_TYPES_LITERAL))
 "All ORAS value types"
 
 PROVIDES_TYPES = list(get_args(PROVIDES_TYPES_LITERAL))
 "The list with all types for provides"
 
+RELATION_COMPARISON_OPERATOR = list(get_args(RELATION_COMPARISON_OPERATOR_LITERAL))
+"The aviable Operators for the relation compare attribute"
+
 CONTROL_TYPES = list(get_args(CONTROL_TYPES_LITERAL))
 "The list with all possible values for control"
 
 INTERNET_RELATION_VALUE = list(get_args(INTERNET_RELATION_VALUE_LITERAL))
 "The list with all possible values for internet"
```

### Comparing `appstream-python-0.5.1/appstream_python.egg-info/PKG-INFO` & `appstream-python-0.6/appstream_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appstream-python
-Version: 0.5.1
+Version: 0.6
 Summary: A library for dealing with Freedesktop Appstream data
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://appstream-python.readthedocs.io
 Project-URL: Issues, https://codeberg.org/JakobDev/appstream-python/issues
 Project-URL: Source, https://codeberg.org/JakobDev/appstream-python
 Project-URL: Donation, https://ko-fi.com/jakobdev
@@ -13,20 +13,18 @@
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Other Environment
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # appstream-python
 
 A library for dealing with Freedesktop Appstream data. This lib is currently in development.
```

### Comparing `appstream-python-0.5.1/pyproject.toml` & `appstream-python-0.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "appstream-python"
 description = "A library for dealing with Freedesktop Appstream data"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 keywords = ["JakobDev", "AppStream", "Freedesktop", "Linux"]
 license = { text = "BSD-2-Clause" }
 authors = [
     { name = "JakobDev", email = "jakobdev@gmx.de" }
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Environment :: Other Environment",
     "License :: OSI Approved :: BSD License",
     "Operating System :: POSIX",
     "Operating System :: POSIX :: BSD",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
+    "Programming Language :: Python :: Implementation :: CPython"
 ]
 dependencies = [
     "lxml"
 ]
 dynamic = ["version"]
 
 [project.urls]
```

### Comparing `appstream-python-0.5.1/tests/test_data.py` & `appstream-python-0.6/tests/test_appstream_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import appstream_python
 import pathlib
 
 
-DATA_DIR = pathlib.Path(__file__).parent / "data"
+DATA_DIR = pathlib.Path(__file__).parent / "data" / "AppStream"
 
 
 def test_data_jdtextedit() -> None:
-    component = appstream_python.AppstreamComponent()
-    component.load_file(DATA_DIR / "com.gitlab.JakobDev.jdTextEdit.metainfo.xml")
+    component = appstream_python.AppstreamComponent.from_file(DATA_DIR / "com.gitlab.JakobDev.jdTextEdit.metainfo.xml")
 
     assert component.id == "com.gitlab.JakobDev.jdTextEdit"
     assert component.name.get_default_text() == "jdTextEdit"
     assert component.summary.get_default_text() == "An advanced text editor"
     assert component.project_license == "GPL-3.0-only"
     assert component.metadata_license == "CC0-1.0"
     assert component.project_group is None
 
     assert len(component.urls) == 4
     assert component.urls["homepage"] == "https://gitlab.com/JakobDev/jdTextEdit"
     assert component.urls["bugtracker"] == "https://gitlab.com/JakobDev/jdTextEdit/-/issues"
     assert component.urls["help"] == "https://jdtextedit.readthedocs.io"
     assert component.urls["vcs-browser"] == "https://gitlab.com/JakobDev/jdTextEdit"
+
+    assert component.display_length["recommends"][0].px == 760
+    assert component.display_length["recommends"][0].compare == "ge"
```

