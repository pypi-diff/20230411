# Comparing `tmp/postleid-0.6.3.tar.gz` & `tmp/postleid-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postleid-0.6.3.tar", last modified: Thu Apr  6 15:57:27 2023, max compression
+gzip compressed data, was "postleid-0.6.4.tar", last modified: Tue Apr 11 11:26:37 2023, max compression
```

## Comparing `postleid-0.6.3.tar` & `postleid-0.6.4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-06 15:57:27.876777 postleid-0.6.3/
--rw-r--r--   0 rainer    (1000) rainer    (1000)     1075 2023-04-05 15:58:25.000000 postleid-0.6.3/LICENSE
--rw-r--r--   0 rainer    (1000) rainer    (1000)     2906 2023-04-06 15:57:27.876777 postleid-0.6.3/PKG-INFO
--rw-r--r--   0 rainer    (1000) rainer    (1000)      270 2023-04-06 15:51:50.000000 postleid-0.6.3/README.md
--rw-r--r--   0 rainer    (1000) rainer    (1000)     1716 2023-04-06 15:52:37.000000 postleid-0.6.3/pyproject.toml
--rw-r--r--   0 rainer    (1000) rainer    (1000)       38 2023-04-06 15:57:27.876777 postleid-0.6.3/setup.cfg
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-06 15:57:27.876777 postleid-0.6.3/src/
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-06 15:57:27.876777 postleid-0.6.3/src/postleid/
--rw-r--r--   0 rainer    (1000) rainer    (1000)      580 2023-04-05 18:53:34.000000 postleid-0.6.3/src/postleid/__init__.py
--rwxr-xr-x   0 rainer    (1000) rainer    (1000)     7090 2023-04-06 08:55:53.000000 postleid-0.6.3/src/postleid/__main__.py
--rw-r--r--   0 rainer    (1000) rainer    (1000)     5605 2023-04-06 08:25:49.000000 postleid-0.6.3/src/postleid/commons.py
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-06 15:57:27.876777 postleid-0.6.3/src/postleid/data/
--rw-r--r--   0 rainer    (1000) rainer    (1000)     1487 2023-04-05 15:58:25.000000 postleid-0.6.3/src/postleid/data/country_names_by_cc.yaml
--rw-r--r--   0 rainer    (1000) rainer    (1000)     1476 2023-04-06 06:34:58.000000 postleid-0.6.3/src/postleid/data/default_user_settings.yaml
--rw-r--r--   0 rainer    (1000) rainer    (1000)     9074 2023-04-05 15:58:25.000000 postleid-0.6.3/src/postleid/data/postal_code_rules_by_cc.yaml
--rw-r--r--   0 rainer    (1000) rainer    (1000)    10379 2023-04-06 08:40:47.000000 postleid-0.6.3/src/postleid/fix_excel_files.py
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-06 15:57:27.876777 postleid-0.6.3/src/postleid/locale/
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-06 15:57:27.876777 postleid-0.6.3/src/postleid/locale/de/
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-06 15:57:27.876777 postleid-0.6.3/src/postleid/locale/de/LC_MESSAGES/
--rw-r--r--   0 rainer    (1000) rainer    (1000)     3749 2023-04-05 15:58:26.000000 postleid-0.6.3/src/postleid/locale/de/LC_MESSAGES/argparse.mo
--rw-r--r--   0 rainer    (1000) rainer    (1000)     1194 2023-04-06 08:11:50.000000 postleid-0.6.3/src/postleid/presets.py
--rw-r--r--   0 rainer    (1000) rainer    (1000)    13925 2023-04-05 15:58:26.000000 postleid-0.6.3/src/postleid/rule_checks.py
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-06 15:57:27.876777 postleid-0.6.3/src/postleid.egg-info/
--rw-r--r--   0 rainer    (1000) rainer    (1000)     2906 2023-04-06 15:57:27.000000 postleid-0.6.3/src/postleid.egg-info/PKG-INFO
--rw-r--r--   0 rainer    (1000) rainer    (1000)      638 2023-04-06 15:57:27.000000 postleid-0.6.3/src/postleid.egg-info/SOURCES.txt
--rw-r--r--   0 rainer    (1000) rainer    (1000)        1 2023-04-06 15:57:27.000000 postleid-0.6.3/src/postleid.egg-info/dependency_links.txt
--rw-r--r--   0 rainer    (1000) rainer    (1000)       52 2023-04-06 15:57:27.000000 postleid-0.6.3/src/postleid.egg-info/entry_points.txt
--rw-r--r--   0 rainer    (1000) rainer    (1000)       54 2023-04-06 15:57:27.000000 postleid-0.6.3/src/postleid.egg-info/requires.txt
--rw-r--r--   0 rainer    (1000) rainer    (1000)        9 2023-04-06 15:57:27.000000 postleid-0.6.3/src/postleid.egg-info/top_level.txt
-drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-06 15:57:27.876777 postleid-0.6.3/tests/
--rw-r--r--   0 rainer    (1000) rainer    (1000)    13336 2023-04-05 15:58:26.000000 postleid-0.6.3/tests/test_commons.py
--rw-r--r--   0 rainer    (1000) rainer    (1000)     3630 2023-04-05 15:58:26.000000 postleid-0.6.3/tests/test_rule_checks.py
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     1075 2023-04-05 15:58:25.000000 postleid-0.6.4/LICENSE
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     2920 2023-04-11 11:26:37.741488 postleid-0.6.4/PKG-INFO
+-rw-r--r--   0 rainer    (1000) rainer    (1000)      288 2023-04-11 10:58:17.000000 postleid-0.6.4/README.md
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     1712 2023-04-07 14:20:30.000000 postleid-0.6.4/pyproject.toml
+-rw-r--r--   0 rainer    (1000) rainer    (1000)       38 2023-04-11 11:26:37.741488 postleid-0.6.4/setup.cfg
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.737488 postleid-0.6.4/src/
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/src/postleid/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)      580 2023-04-08 12:11:49.000000 postleid-0.6.4/src/postleid/__init__.py
+-rwxr-xr-x   0 rainer    (1000) rainer    (1000)     7013 2023-04-09 19:19:40.000000 postleid-0.6.4/src/postleid/__main__.py
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     5403 2023-04-09 19:15:27.000000 postleid-0.6.4/src/postleid/commons.py
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/src/postleid/data/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     3709 2023-04-11 10:34:20.000000 postleid-0.6.4/src/postleid/data/country_names_by_cc.yaml
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     1490 2023-04-11 07:13:07.000000 postleid-0.6.4/src/postleid/data/default_user_settings.yaml
+-rw-r--r--   0 rainer    (1000) rainer    (1000)    13200 2023-04-11 09:44:57.000000 postleid-0.6.4/src/postleid/data/postal_code_rules_by_cc.yaml
+-rw-r--r--   0 rainer    (1000) rainer    (1000)    10384 2023-04-09 19:17:40.000000 postleid-0.6.4/src/postleid/fix_excel_files.py
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/src/postleid/locale/
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/src/postleid/locale/de/
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/src/postleid/locale/de/LC_MESSAGES/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     3749 2023-04-05 15:58:26.000000 postleid-0.6.4/src/postleid/locale/de/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 rainer    (1000) rainer    (1000)      738 2023-04-09 19:13:52.000000 postleid-0.6.4/src/postleid/paths.py
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     1194 2023-04-06 08:11:50.000000 postleid-0.6.4/src/postleid/presets.py
+-rw-r--r--   0 rainer    (1000) rainer    (1000)    13925 2023-04-05 15:58:26.000000 postleid-0.6.4/src/postleid/rule_checks.py
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/src/postleid.egg-info/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     2920 2023-04-11 11:26:37.000000 postleid-0.6.4/src/postleid.egg-info/PKG-INFO
+-rw-r--r--   0 rainer    (1000) rainer    (1000)      660 2023-04-11 11:26:37.000000 postleid-0.6.4/src/postleid.egg-info/SOURCES.txt
+-rw-r--r--   0 rainer    (1000) rainer    (1000)        1 2023-04-11 11:26:37.000000 postleid-0.6.4/src/postleid.egg-info/dependency_links.txt
+-rw-r--r--   0 rainer    (1000) rainer    (1000)       52 2023-04-11 11:26:37.000000 postleid-0.6.4/src/postleid.egg-info/entry_points.txt
+-rw-r--r--   0 rainer    (1000) rainer    (1000)       54 2023-04-11 11:26:37.000000 postleid-0.6.4/src/postleid.egg-info/requires.txt
+-rw-r--r--   0 rainer    (1000) rainer    (1000)        9 2023-04-11 11:26:37.000000 postleid-0.6.4/src/postleid.egg-info/top_level.txt
+drwxr-xr-x   0 rainer    (1000) rainer    (1000)        0 2023-04-11 11:26:37.741488 postleid-0.6.4/tests/
+-rw-r--r--   0 rainer    (1000) rainer    (1000)    13336 2023-04-05 15:58:26.000000 postleid-0.6.4/tests/test_commons.py
+-rw-r--r--   0 rainer    (1000) rainer    (1000)     3630 2023-04-05 15:58:26.000000 postleid-0.6.4/tests/test_rule_checks.py
```

### Comparing `postleid-0.6.3/LICENSE` & `postleid-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `postleid-0.6.3/PKG-INFO` & `postleid-0.6.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postleid
-Version: 0.6.3
+Version: 0.6.4
 Summary: Fix postal codes notation in spreadsheet documents
 Author-email: Rainer Schwarzbach <undisclosed@example.com>
 License: MIT License
         
         Copyright (c) 2023 Rainer Schwarzbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://codeberg.org/blackstream-x/postleid
 Project-URL: Changelog, https://codeberg.org/blackstream-x/postleid/src/branch/main/CHANGELOG.md
 Project-URL: Documentation, https://blackstream-x.codeberg.page/postleid/
-Project-URL: Repository, https://codeberg.org/blackstream-x/postleid.git
+Project-URL: Repository, https://codeberg.org/blackstream-x/postleid
 Project-URL: Bug Tracker, https://codeberg.org/blackstream-x/postleid/issues
 Keywords: postleitzahlen,plz,postal codes,excel
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: German
@@ -50,11 +50,11 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Postleid
 
 Skript zum Korrigieren von Postleitzahlen in Excel-Dateien
 
-Bisher werden Postleitzahlenregeln für 36 Länder,
+Bisher werden Postleitzahlenregeln für 83 Länder,
 darunter Belgien, Deutschland, Österreich und die Schweiz,
-unterstützt (siehe CHANGELOG.md).
+unterstützt (siehe CHANGELOG.md und countries.txt).
 Die Unterstützung weiterer Länder ist in Arbeit.
```

### Comparing `postleid-0.6.3/pyproject.toml` & `postleid-0.6.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   "xlrd>=2.0.1",
 ]
 
 [project.urls]
 "Homepage" = "https://codeberg.org/blackstream-x/postleid"
 "Changelog" = "https://codeberg.org/blackstream-x/postleid/src/branch/main/CHANGELOG.md"
 "Documentation" = "https://blackstream-x.codeberg.page/postleid/"
-"Repository" = "https://codeberg.org/blackstream-x/postleid.git"
+"Repository" = "https://codeberg.org/blackstream-x/postleid"
 "Bug Tracker" = "https://codeberg.org/blackstream-x/postleid/issues"
 
 [project.scripts]
 postleid = "postleid.__main__:main"
 
 [tool.setuptools.dynamic]
 version = {attr = "postleid.__version__"}
```

### Comparing `postleid-0.6.3/src/postleid/__init__.py` & `postleid-0.6.4/src/postleid/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
 
-__version__ = "0.6.3"
+__version__ = "0.6.4"
 
 
 # vim: fileencoding=utf-8 sw=4 ts=4 sts=4 expandtab autoindent syntax=python:
```

### Comparing `postleid-0.6.3/src/postleid/__main__.py` & `postleid-0.6.4/src/postleid/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,31 +21,27 @@
 
 """
 
 
 import argparse
 import gettext
 import logging
-import pathlib
 import shutil
 import sys
 
 from typing import List, Optional
 
 # local imports
 from postleid import __version__
 from postleid import commons
 from postleid import fix_excel_files
+from postleid import paths
 from postleid import presets
 
 
-# Absolute script path
-SCRIPT_PATH = pathlib.Path(sys.argv[0]).resolve()
-
-
 def list_supported_countries() -> int:
     """List supported countries and exit with the matching returncode"""
     try:
         country_names = commons.load_country_names_from_file()
     except OSError as error:
         commons.LogWrapper.error(f"{error}")
         return commons.RETURNCODE_ERROR
@@ -100,28 +96,28 @@
         by argparse.ArgumentParser().parse_args()
     """
     # ------------------------------------------------------------------
     # Argparse translation code adapted from
     # <https://github.com/s-ball/i18nparse>
     translation = gettext.translation(
         "argparse",
-        localedir=SCRIPT_PATH.parent / "locale",
+        localedir=paths.PACKAGE_LOCALE_PATH,
         languages=["de"],
         fallback=True,
     )
     argparse._ = translation.gettext  # type: ignore
     argparse.ngettext = translation.ngettext  # type: ignore
     # ------------------------------------------------------------------
     main_parser = argparse.ArgumentParser(
         prog="postleid",
         description="Postleitzahlen in Excel-Dateien korrigieren",
     )
     main_parser.set_defaults(
         loglevel=logging.INFO,
-        settings_file=pathlib.Path(presets.DEFAULT_USER_SETTINGS_FILE_NAME),
+        settings_file=paths.Path(presets.DEFAULT_USER_SETTINGS_FILE_NAME),
     )
     main_parser.add_argument(
         "--version",
         action="version",
         version=f"%(prog)s {__version__}",
         help="Version ausgeben und beenden",
     )
@@ -154,30 +150,30 @@
         " (der Dateiname muss in diesem Fall zwar auch angegeben werden,"
         " wird jedoch ignoriert)",
     )
     main_parser.add_argument(
         "-o",
         "--output-file",
         metavar="AUSGABEDATEI",
-        type=pathlib.Path,
+        type=paths.Path,
         help="die Ausgabedatei (Standardwert: Name der Original-Exceldatei"
         f" mit vorangestelltem {presets.DEFAULT_FIXED_FILE_PREFIX!r})",
     )
     main_parser.add_argument(
         "-s",
         "--settings-file",
         metavar="EINSTELLUNGSDATEI",
-        type=pathlib.Path,
+        type=paths.Path,
         help="die Datei mit Benutzereinstellungen"
         " (Standardwert: %(default)s im aktuellen Verzeichnis)",
     )
     main_parser.add_argument(
         "excel_file",
         metavar="EXCELDATEI",
-        type=pathlib.Path,
+        type=paths.Path,
         help="die Original-Exceldatei",
     )
     return main_parser.parse_args(args)
 
 
 def main(args: Optional[List[str]] = None) -> int:
     """Check the zip codes in the input file,
@@ -195,16 +191,16 @@
     else:
         target_path = (
             source_path.parent
             / f"{presets.DEFAULT_FIXED_FILE_PREFIX}{source_path.name}"
         )
     #
     if not arguments.settings_file.exists():
-        default_settings_path = commons.build_data_file_path(
-            "default_user_settings.yaml"
+        default_settings_path = (
+            paths.PACKAGE_DATA_PATH / "default_user_settings.yaml"
         )
         commons.LogWrapper.info(
             f"Einstellungsdatei {arguments.settings_file}"
             " noch nicht vorhanden",
             f" → erzeuge eine neue aus {default_settings_path} …",
         )
         shutil.copy2(default_settings_path, arguments.settings_file)
```

### Comparing `postleid-0.6.3/src/postleid/commons.py` & `postleid-0.6.4/src/postleid/commons.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 
 """
 
 
 import bisect
 import dataclasses
 import logging
-import pathlib
 import textwrap
 
 from collections import Counter
 
 from typing import Any, List, Tuple, Union
 
 import yaml
 
 # local imports
+from postleid import paths
 from postleid import presets
 
 
 # STATISTICS KEYWORDS
 S_UNCHANGED = "(=) unverändert"
 S_FIXED = "(✔) korrigiert"
 S_MISSING_RULES = "(✘) Regeln fehlen"
@@ -159,32 +159,27 @@
                 f" {f'{keyword}:':<{max_kw_width + 1}} {frequency}",
             )
         #
     #
     return everything_is_fine, data_changed
 
 
-def build_data_file_path(file_name: Union[str, pathlib.Path]) -> pathlib.Path:
-    """Build a data file path from the provided file name"""
-    return pathlib.Path(__file__).resolve().parent / "data" / file_name
-
-
-def load_yaml_from_path(path: pathlib.Path) -> Any:
+def load_yaml_from_path(path: paths.Path) -> Any:
     """Load a YAML file from the provided path
     and return its deserialized contents
     """
     return yaml.safe_load(path.read_text(encoding="utf-8"))
 
 
-def load_yaml_data_file(file_name: Union[str, pathlib.Path]) -> Any:
+def load_yaml_data_file(file_name: Union[str, paths.Path]) -> Any:
     """Load YAML from the provided file
     located in the data subdirectory
     and return its deserialized contents
     """
-    return load_yaml_from_path(build_data_file_path(file_name))
+    return load_yaml_from_path(paths.PACKAGE_DATA_PATH / file_name)
 
 
 def load_rules_from_file() -> Any:
     """Load the postal code rules by country code
     from the appropriate file
     """
     return load_yaml_data_file("postal_code_rules_by_cc.yaml")
```

### Comparing `postleid-0.6.3/src/postleid/data/default_user_settings.yaml` & `postleid-0.6.4/src/postleid/data/default_user_settings.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #     - true bzw. yes
 #     - false bzw. no
 #   Falls diese Option auf true oder yes gesetzt wird, wird
 #   beispielsweise aus der ungültigen Angabe 77 die (theoretisch)
 #   gültige Postleitzahl 77000 abgeleitet, oder auch aus dem
 #   Dezimalbruch 1.234567 die (ebenfalls theoretisch) gültige
 #   Postleitzahl 1234.
-#   Für einzelne Zielländer (z.B. Bahrain) sind allerdings
+#   Für einzelne Zielländer (z.B. Bahrain, Guinea, ...) sind allerdings
 #   auch 3-stellige Postleitzahlen gültig, daher wurde der Standardwert
 #   dieser Option auf no gesetzt.
 
 guess_1000s: no
 
 # country_headings:
 #   Liste möglicher Überschriften für die Spalte mit der Angabe
@@ -40,7 +40,8 @@
 #   Liste möglicher ÜberschriftTEILE für die Spalte mit der Angabe
 #   der Postleitzahl, Groß- und Kleinschreibung ist irrelevant.
 
 postal_code_heading_parts:
 - PLZ
 - Postleit
 - Zip Code
+
```

### Comparing `postleid-0.6.3/src/postleid/data/postal_code_rules_by_cc.yaml` & `postleid-0.6.4/src/postleid/data/postal_code_rules_by_cc.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -10,63 +10,64 @@
 # postleid is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the LICENSE file for more details.
 #
 # The rules are adapted from
 # <https://github.com/zauberware/postal-codes-json-xml-csv>,
-# <https://en.wikipedia.org/wiki/List_of_postal_codes>
+# <https://en.wikipedia.org/wiki/List_of_postal_codes>,
+# <https://en.youbianku.com/>
 # and linked pages/websites
 #
 ad:
-  comment: Andorra (ccnnn)
+  comment: Andorra
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Andorra"
   compound:
   - pattern: cc
   - pattern: n
     min: 1
     max: 7
   - pattern: nn
 af:
-  comment: Afghanistan (nnnn)
+  comment: Afghanistan
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Afghanistan"
   compound:
   - pattern: nn
     min: 10
     max: 43
   - pattern: nn
 ai:
-  comment: Anguilla ("AI-2640")
+  comment: Anguilla
   compound:
   - pattern: cc
   - literal: "-2640"
 al:
-  comment: Albania (nnnn)
+  comment: Albania
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Albania"
   compound:
   - pattern: nn
     min: 10
     max: 97
   - pattern: nn
 am:
-  comment: Armenia (nnnn)
+  comment: Armenia
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Armenia"
   compound:
   - pattern: nn
     max: 42
   - pattern: nn
 aq:
-  comment: British Antarctic Territory ("BIQQ 1ZZ")
+  comment: British Antarctic Territory
   literal: "BIQQ 1ZZ"
 ar:
-  comment: Argentina (annnnaaa, nnnn)
+  comment: Argentina
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Argentina"
   - "https://en.wikipedia.org/wiki/ISO_3166-2:AR"
   variants:
   - compound:
     - pattern: n
       min: 1
@@ -75,194 +76,194 @@
     - pattern: a
       except: [I, O]
     - pattern: n
       min: 1
     - pattern: nnn
     - pattern: aaa
 as:
-  comment: American Samoa (96799-nnnn, 96799; part of US system)
+  comment: American Samoa (part of US system)
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Oceania"
   variants:
   - compound:
     - literal: "96799-"
     - pattern: nnnn
   - literal: "96799"
 at:
-  comment: Austria (nnnn)
+  comment: Austria
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Austria"
   compound:
   - pattern: n
     min: 1
   - pattern: nnn
 au:
-  comment: Australia (nnnn)
+  comment: Australia
   urls:
   - "https://en.wikipedia.org/wiki/Postcodes_in_Australia"
   compound:
   - pattern: nn
     min: 2
   - pattern: nn
 ax:
-  comment: Åland (AX-22nnn, part of finnish system)
+  comment: Åland (part of Finnish system)
   compound:
   - pattern: cc
   - literal: "-22"
   - pattern: nnn
 az:
-  comment: Azerbaijan (AZ nnnn)
+  comment: Azerbaijan
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Azerbaijan"
   compound:
   - pattern: cc
   - literal: " "
   - pattern: nn
     min: 1
     max: 69
   - pattern: nn
 ba:
-  comment: Bosnia and Herzegovina (nnnnn)
+  comment: Bosnia and Herzegovina
   pattern: nnnnn
 bb:
-  comment: Barbados (ccnnnnn)
+  comment: Barbados
   urls:
   - "https://en.wikipedia.org/wiki/Barbados_Postal_Service#Postal_codes"
   compound:
   - pattern: cc
   - pattern: nnnnn
 bd:
-  comment: Bangladesh (nnnn)
+  comment: Bangladesh
   urls:
   - "https://en.wikipedia.org/wiki/List_of_postal_codes_in_Bangladesh"
   compound:
   - pattern: nn
     min: 10
   - pattern: nn
 be:
-  comment: Belgium (nnnn)
+  comment: Belgium
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Belgium"
   compound:
   - pattern: nn
     min: 10
   - pattern: nn
 bg:
-  comment: Bulgaria (nnnn)
+  comment: Bulgaria
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Bulgaria"
   compound:
   - pattern: n
     min: 1
   - pattern: nnn
 bh:
-  comment: Bahrain (nnn or nnnn)
+  comment: Bahrain
   pattern: nnnn
   min: 101
   max: 1216
   remove_leading_zeroes: yes
 bm:
-  comment: Bermuda (aa nn, aa aa)
+  comment: Bermuda
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Bermuda"
   variants:
   - compound:
     - pattern: aa
     - literal: " "
     - pattern: nn
   - compound:
     - pattern: aa
     - literal: " "
     - pattern: aa
 bn:
-  comment: Brunei (aannnn)
+  comment: Brunei
   urls:
   - "https://en.wikipedia.org/wiki/Postcodes_in_Brunei"
   compound:
   - pattern: a
     only: [B, K, T, P]
   - pattern: a
   - pattern: nnnn
 br:
-  comment: Brazil (nnnnn, nnnnn-nnn)
+  comment: Brazil
   urls:
   - "https://en.wikipedia.org/wiki/C%C3%B3digo_de_Endere%C3%A7amento_Postal"
   variants:
   - pattern: nnnnn
   - compound:
     - pattern: nnnnn
     - literal: "-"
     - pattern: nnn
 bt:
-  comment: Bhutan (nnnnn)
+  comment: Bhutan
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Bhutan"
   pattern: nnnnn
 by:
-  comment: Belarus (nnnnnn)
+  comment: Belarus
   pattern: nnnnnn
 ca:
-  comment: Canada (ana nan)
+  comment: Canada
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Canada"
   compound:
   - pattern: a
     except: [D, F, I, O, Q, U, W, Z]
   - pattern: n
   - pattern: a
     except: [D, F, I, O, Q, U]
   - literal: " "
   - pattern: n
   - pattern: a
     except: [D, F, I, O, Q, U]
   - pattern: n
 cc:
-  comment: Cocos (Keeling) Island (nnnn, part of Australian system)
+  comment: Cocos (Keeling) Island (part of Australian system)
   pattern: nnnn
 ch:
-  comment: Switzerland (nnnn)
+  comment: Switzerland
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Switzerland_and_Liechtenstein"
   compound:
   - pattern: n
     min: 1
   - pattern: nnn
 cl:
-  comment: Chile (nnnnnnn, nnn-nnnn)
+  comment: Chile
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Chile"
   variants:
   - compound:
     - pattern: n
       min: 1
     - pattern: nnnnnn
   - compound:
     - pattern: n
       min: 1
     - pattern: nn
     - literal: "-"
     - pattern: nnnn
 cn:
-  comment: "People's Republic of China (nnnnnn)"
+  comment: "People's Republic of China"
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_China"
   compound:
   - pattern: nn
     min: 1
   - pattern: nnnn
 co:
-  comment: Colombia (nnnnnn)
+  comment: Colombia
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Colombia"
   compound:
   - pattern: nn
     max: 32
   - pattern: nnnn
 cr:
-  comment: Costa Rica (nnnnn, nnnnn-nnnn)
+  comment: Costa Rica
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Costa_Rica"
   variants:
   - compound:
     - pattern: n
       min: 1
       max: 7
@@ -271,165 +272,396 @@
     - pattern: n
       min: 1
       max: 7
     - pattern: nnnn
     - literal: "-"
     - pattern: nnnn
 cu:
-  comment: Cuba (nnnnn, CP nnnnn)
+  comment: Cuba
   variants:
   - pattern: nnnnn
   - compound:
     - literal: "CP "
     - pattern: nnnnn
 cv:
-  comment: Cape Verde (nnnn)
+  comment: Cape Verde
   pattern: nnnn
 cx:
-  comment: Christmas Island (nnnn, part of Australian system)
+  comment: Christmas Island
   pattern: nnnn
 cy:
-  comment: Cyprus (nnnn)
+  comment: Cyprus
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Cyprus"
   compound:
   - pattern: n
     min: 1
   - pattern: nnn
 cz:
-  comment: Czech Republic (nnn nn, common system with Slovakia)
+  comment: Czech Republic (common system with Slovakia)
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_the_Czech_Republic"
   compound:
   - pattern: n
     min: 1
     max: 7
   - pattern: nn
   - literal: " "
   - pattern: nn
 de:
-  comment: Germany (nnnnn)
+  comment: Germany
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Germany"
   compound:
   - pattern: nn
     min: 1
   - pattern: nnn
 dk:
-  comment: Denmark (nnnn, cc-nnnn)
+  comment: Denmark
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Denmark"
   variants:
   - pattern: nnnn
   - compound:
     - pattern: cc
     - literal: "-"
     - pattern: nnnn
 do:
-  comment: Dominican Republic (nnnnn)
+  comment: Dominican Republic
   pattern: nnnnn
 dz:
-  comment: Algeria (nnnnn)
+  comment: Algeria
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Algeria"
   - "https://en.wikipedia.org/wiki/ISO_3166-2:DZ"
   compound:
   - pattern: nn
     min: 10
     max: 58
   - pattern: nnn
 ec:
-  comment: Ecuador (nnnnnn)
+  comment: Ecuador
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Ecuador"
   compound:
   - pattern: nn
     min: 1
     max: 24
   - pattern: nnnn
 ee:
-  comment: Estonia (nnnnn)
+  comment: Estonia
   pattern: nnnnn
 eg:
-  comment: Egypt (nnnnn)
+  comment: Egypt
   pattern: nnnnn
 et:
-  comment: Ethiopia (nnnn)
+  comment: Ethiopia
   pattern: nnnn
 fi:
-  comment: Finland (nnnnn)
+  comment: Finland
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Finland"
   pattern: nnnnn
 fk:
-  comment: Falkland Islands ("FIQQ 1ZZ")
+  comment: Falkland Islands
   literal: "FIQQ 1ZZ"
+fo:
+  comment: Faroe Islands
+  compound:
+    - pattern: cc
+    - pattern: nnn
+fr:
+  comment: France
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
+  compound:
+    - pattern: nn
+      min: 1
+    - pattern: nnn
 ge:
-  comment: Georgia (nnnn)
+  comment: Georgia
   pattern: nnnn
+gf:
+  comment: French Guiana
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
+  compound:
+    - literal: "973"
+    - pattern: nn
+      max: 90
+gg:
+  comment: Guernsey (part of UK  system)
+  urls:
+  - "https://en.wikipedia.org/wiki/GY_postcode_area"
+  compound:
+  - literal: "GY"
+  - pattern: nn
+    min: 1
+    max: 10
+    remove_leading_zeroes: yes
+  - literal: " "
+  - pattern: n
+  - pattern: aa
 gh:
-  comment: Ghana (a?nnn, a?nnnn, a?nnnnn)
+  comment: Ghana
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Ghana"
   variants:
   - compound:
     - pattern: a?
     - pattern: nnn
   - compound:
     - pattern: a?
     - pattern: nnnn
   - compound:
     - pattern: a?
     - pattern: nnnnn
+gi:
+  comment: Gibraltar
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_addresses_in_Gibraltar"
+  literal: "GX11 1AA"
+gl:
+  comment: Greenland (part of Danish system)
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Greenland"
+  compound:
+  - pattern: cc
+  - literal: "-39"
+  - pattern: nn
+gn:
+  comment: Guinea
+  pattern: nnn
+gp:
+  comment: Guadeloupe
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_France"
+  compound:
+    - literal: "971"
+    - pattern: nn
+      max: 90
+gr:
+  comment: Greece
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Greece"
+  compound:
+  - pattern: nnn
+    min: 100
+    max: 899
+  - literal: " "
+  - pattern: nn
+gt:
+  comment: Guatemala
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Guatemala"
+  - "https://en.wikipedia.org/wiki/Departments_of_Guatemala"
+  - pattern: nn
+    min: 1
+    max: 22
+  - pattern: nnn
+gu:
+  comment: Guam (part of US system)
+  variants:
+  - compound:
+    - literal: "969"
+    - pattern: nn
+      min: 10
+      max: 32
+  - compound:
+    - literal: "969"
+    - pattern: nn
+      min: 10
+      max: 32
+    - literal: "-"
+    - pattern: nnnn
+gw:
+  comment: Guinea-Bissau
+  pattern: nnnn
+hn:
+  comment: Honduras
+  urls:
+  - "https://www.grcdi.nl/gsb/honduras.html"
+  - "https://en.youbianku.com/honduras"
+  variants:
+  - compound:
+    - pattern: aa
+    - pattern: nnnn
+    deprecated: probably to avoid confusion of the department with an ISO-3166 code
+  - pattern: nnnnn
 hr:
-  comment: Croatia (nnnnn)
+  comment: Croatia
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Croatia"
   compound:
   - pattern: nn
     min: 10
     max: 53
   - pattern: nnn
+ht:
+  comment: Haiti
+  pattern: nnnn
+hu:
+  comment: Hungary
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Hungary"
+  compound:
+  - pattern: n
+    max: 9
+  - pattern: nnn
+id:
+  comment: Indonesia
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Indonesia"
+  compound:
+  - pattern: nn
+    min: 10
+  - pattern: nnn
+ie:
+  comment: Ireland
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_addresses_in_the_Republic_of_Ireland"
+  - "https://en.youbianku.com/Ireland"
+  compound:
+  - pattern: a
+    except: [B, G, I, J, L, M, O, Q, S, U, Z]
+  - pattern: n
+  - pattern: "?"
+    except: [B, G, I, J, L, M, O, Q, S, U, Z]
+  - literal: " "
+  - pattern: ????
+il:
+  comment: Israel
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Israel"
+  pattern: nnnnnnn
+im:
+  comment: Isle of Man (part of UK system)
+  urls:
+  - "https://en.wikipedia.org/wiki/IM_postcode_area"
+  compound:
+  - pattern: cc
+  - pattern: nn
+    remove_leading_zeroes: yes
+  - literal: " "
+  - pattern: n
+  - pattern: aa
+in:
+  comment: India
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_Index_Number"
+  variants:
+  - compound:
+    - pattern: nn
+      min: 11
+    - pattern: nnnn
+  - compound:
+    - pattern: nn
+      min: 11
+    - pattern: n
+    - literal: " "
+    - pattern: nnn
 io:
-  comment: British Indian Ocean Territory ("BBND 1ZZ")
+  comment: British Indian Ocean Territory
   literal: "BBND 1ZZ"
+iq:
+  comment: Iraq
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Iraq"
+  - "https://en.youbianku.com/Iraq"
+  compound:
+  - pattern: nn
+    min: 10
+  - pattern: nnn
+ir:
+  comment: Iran
+  urls:
+  - "https://en.wikipedia.org/wiki/Identity_documents_in_Iran#Postal_code_in_Iran"
+  - "https://en.youbianku.com/Iran"
+  variants:
+  - compound:
+    - pattern: nnnnn
+    - literal: "-"
+    - pattern: nnnnn
+  - compound:
+    - pattern: nnnnn
+    - pattern: nnnnn
+is:
+  comment: Iceland
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Iceland"
+  pattern: nnn
+it:
+  comment: Italy
+  urls:
+  - "https://en.wikipedia.org/wiki/Codice_di_avviamento_postale"
+  pattern: nnnnn
+je:
+  comment: Jersey (part of UK  system)
+  urls:
+  - "https://en.wikipedia.org/wiki/JE_postcode_area"
+  compound:
+  - literal: cc
+  - pattern: nn
+    remove_leading_zeroes: yes
+  - literal: " "
+  - pattern: n
+  - pattern: aa
+jo:
+  comment: Jordan
+  pattern: nnnnn
+jp:
+  comment: Japan
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Japan"
+  compound:
+  - pattern: nnn
+    literal: "-"
+  - pattern: nnnn
 kh:
-  comment: Cambodia (nnnnnn)
+  comment: Cambodia
   pattern: nnnnnn
 ky:
-  comment: Cayman Islands (ccn-nnnn)
+  comment: Cayman Islands
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_the_Cayman_Islands"
   compound:
   - pattern: cc
   - pattern: n
     min: 1
     max: 3
   - literal: "-"
   - pattern: nnnn
 li:
-  comment: Liechtenstein (nnnn; part of swiss system)
+  comment: Liechtenstein (part of Swiss system)
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_Liechtenstein"
   compound:
   - pattern: nnn
     min: 948
     max: 949
   - pattern: n
+pf:
+  comment: French Polynesia
+  urls:
+  - "https://en.wikipedia.org/wiki/Postal_codes_in_Oceania#French_overseas_territories"
+  compound:
+    - literal: "987"
+    - pattern: nn
+      max: 90
 sv:
-  comment: El Salvador (nnnn)
+  comment: El Salvador
   pattern: nnnn
 sz:
-  comment: Eswatini (annn)
+  comment: Eswatini
   compound:
   - pattern: a
     only: [H, M, S, L]
   - pattern: nnn
 vg:
-  comment: British Virgin Islands (ccnnnn)
+  comment: British Virgin Islands
   urls:
   - "https://en.wikipedia.org/wiki/Postal_codes_in_the_British_Virgin_Islands"
   compound:
   - pattern: cc
   - pattern: nnn
     min: 111
     max: 116
```

### Comparing `postleid-0.6.3/src/postleid/fix_excel_files.py` & `postleid-0.6.4/src/postleid/fix_excel_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,22 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the LICENSE file for more details.
 
 """
 
 
-import pathlib
-
 from typing import Any, Dict, List, Union
 
 import numpy
 import pandas
 
 # local imports
 from postleid import commons
+from postleid import paths
 from postleid import rule_checks
 
 
 class DataFixer:
 
     """Fix cells in a workbook"""
 
@@ -233,23 +232,23 @@
         commons.LogWrapper.info(
             "Sortiere Daten nach Land und Postleitzahl ..."
         )
         self.dataframe = self.dataframe.sort_values(
             [self.cc_column, self.zip_column]
         )
 
-    def save(self, output_file: pathlib.Path) -> None:
+    def save(self, output_file: paths.Path) -> None:
         """Save the dataframe"""
         del self.dataframe[self.cc_column]
         self.dataframe.to_excel(output_file, index=False)
 
 
 def process_file(
-    source_path: pathlib.Path,
-    target_path: pathlib.Path,
+    source_path: paths.Path,
+    target_path: paths.Path,
     user_settings: commons.UserSettings = commons.UserSettings(),
 ) -> int:
     """Process the file provided in source_path,
     write output to target_path
     and return the appropriate return code
     """
     commons.LogWrapper.info(f"Lade Datei {source_path} …")
```

### Comparing `postleid-0.6.3/src/postleid/locale/de/LC_MESSAGES/argparse.mo` & `postleid-0.6.4/src/postleid/locale/de/LC_MESSAGES/argparse.mo`

 * *Files identical despite different names*

### Comparing `postleid-0.6.3/src/postleid/presets.py` & `postleid-0.6.4/src/postleid/presets.py`

 * *Files identical despite different names*

### Comparing `postleid-0.6.3/src/postleid/rule_checks.py` & `postleid-0.6.4/src/postleid/rule_checks.py`

 * *Files identical despite different names*

### Comparing `postleid-0.6.3/src/postleid.egg-info/PKG-INFO` & `postleid-0.6.4/src/postleid.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postleid
-Version: 0.6.3
+Version: 0.6.4
 Summary: Fix postal codes notation in spreadsheet documents
 Author-email: Rainer Schwarzbach <undisclosed@example.com>
 License: MIT License
         
         Copyright (c) 2023 Rainer Schwarzbach
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://codeberg.org/blackstream-x/postleid
 Project-URL: Changelog, https://codeberg.org/blackstream-x/postleid/src/branch/main/CHANGELOG.md
 Project-URL: Documentation, https://blackstream-x.codeberg.page/postleid/
-Project-URL: Repository, https://codeberg.org/blackstream-x/postleid.git
+Project-URL: Repository, https://codeberg.org/blackstream-x/postleid
 Project-URL: Bug Tracker, https://codeberg.org/blackstream-x/postleid/issues
 Keywords: postleitzahlen,plz,postal codes,excel
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: German
@@ -50,11 +50,11 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Postleid
 
 Skript zum Korrigieren von Postleitzahlen in Excel-Dateien
 
-Bisher werden Postleitzahlenregeln für 36 Länder,
+Bisher werden Postleitzahlenregeln für 83 Länder,
 darunter Belgien, Deutschland, Österreich und die Schweiz,
-unterstützt (siehe CHANGELOG.md).
+unterstützt (siehe CHANGELOG.md und countries.txt).
 Die Unterstützung weiterer Länder ist in Arbeit.
```

### Comparing `postleid-0.6.3/src/postleid.egg-info/SOURCES.txt` & `postleid-0.6.4/src/postleid.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 src/postleid/__init__.py
 src/postleid/__main__.py
 src/postleid/commons.py
 src/postleid/fix_excel_files.py
+src/postleid/paths.py
 src/postleid/presets.py
 src/postleid/rule_checks.py
 src/postleid.egg-info/PKG-INFO
 src/postleid.egg-info/SOURCES.txt
 src/postleid.egg-info/dependency_links.txt
 src/postleid.egg-info/entry_points.txt
 src/postleid.egg-info/requires.txt
```

### Comparing `postleid-0.6.3/tests/test_commons.py` & `postleid-0.6.4/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `postleid-0.6.3/tests/test_rule_checks.py` & `postleid-0.6.4/tests/test_rule_checks.py`

 * *Files identical despite different names*

