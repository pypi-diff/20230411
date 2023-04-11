# Comparing `tmp/kohlrahbi-0.0.3.tar.gz` & `tmp/kohlrahbi-0.0.4.tar.gz`

## Comparing `kohlrahbi-0.0.3.tar` & `kohlrahbi-0.0.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/README.md
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/requirements.in
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/requirements.txt
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/.github/dependabot.yml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/.github/workflows/black.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/_kohlrahbi_version.py
--rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/__init__.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/ahbfilefinder.py
--rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/all_known_pruefis.toml
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/collect_pruefis.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/logger.ini
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/logger.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/py.typed
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/read_functions.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/row_type_checker.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/seed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/ahb/__init__.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/ahb/ahbsubtable.py
--rw-r--r--   0        0        0     7849 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/ahb/ahbtable.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/ahb/ahbtablerow.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/docxtablecells/__init__.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/docxtablecells/bedinungscell.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/docxtablecells/bodycell.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/enums/__init__.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/enums/flat_ahb_row_type.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/enums/row_type.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/enums/row_type_color.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/unfoldedahb/__init__.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
--rw-r--r--   0        0        0    15223 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
--rw-r--r--   0        0        0   861363 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/temp/test-fobar.docx
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/.gitignore
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7419 2020-02-02 00:00:00.000000 kohlrahbi-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/README.md
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/requirements.in
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/workflows/black.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/_kohlrahbi_version.py
+-rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/__init__.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/ahbfilefinder.py
+-rw-r--r--   0        0        0     4299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/all_known_pruefis.toml
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/collect_pruefis.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/logger.ini
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/logger.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/py.typed
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/read_functions.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/row_type_checker.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/seed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/ahb/__init__.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/ahb/ahbsubtable.py
+-rw-r--r--   0        0        0     7849 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/ahb/ahbtable.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/ahb/ahbtablerow.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/__init__.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/bedinungscell.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/bodycell.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/edifactstrukturcell.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/enums/__init__.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/enums/flat_ahb_row_type.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/enums/row_type.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/enums/row_type_color.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/unfoldedahb/__init__.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/unfoldedahb/unfoldedahbline.py
+-rw-r--r--   0        0        0    15706 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/src/kohlrahbi/unfoldedahb/unfoldedahbtablemetadata.py
+-rw-r--r--   0        0        0   861363 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/temp/test-fobar.docx
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/.gitignore
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 kohlrahbi-0.0.4/PKG-INFO
```

### Comparing `kohlrahbi-0.0.3/.pre-commit-config.yaml` & `kohlrahbi-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/README.md` & `kohlrahbi-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 However, the technical specifications of this API are
 * prose
 * on DIN A4 pages.
 
 The Anwendungshandbücher are the epitome of digitization with some good intentions.
 
 Although the AHBs are publicly available as PDF or Word files on `edi-energy.de`, they are hardly accessible in a technical sense:
-* You cannot automatically extract information from the AHBs. 
+* You cannot automatically extract information from the AHBs.
 * You cannot run automatic comparisons between different versions.
 * You cannot automatically test your own API against the set of rules, described in the AHBs (as prose).
 * You cannot view or visualize the information from the AHBs in any more intuitive or practical way, than the raw tables from the AHB files.
 * ...any many more...
 
 The root cause for all these inaccessibility is a technical one:
 Information that are theoretically structured are published in an unstructured format (PDF or Word), which is not suited for technical specifications in IT.
@@ -72,39 +72,41 @@
 ```
 
 ## Usage
 
 There are two ways to use kohlrahbi.
 1. You can extract all prüfidentifikatoren listed in [all_known_pruefis.toml,](src/kohlrahbi/all_known_pruefis.toml)
 2. or you can extract a specific prüfidentifikator.
+
 ### Get all Prüfidentifikatoren
 If you want to extract all prüfidentifikatoren, you can run the following command.
+For the following steps we assume that you cloned our [edi_energy_mirror](https://github.com/Hochfrequenz/edi_energy_mirror/) to a neighbouring directory.
 
 ```bash
-kohlrahbi --input_path ../edi_energy_mirror/ --output_path ./output/
+kohlrahbi --input_path ../edi_energy_mirror/edi_energy_de/current --output_path ./output/ --file-type flatahb
 ```
 
 This will extract all prüfidentifikatoren listed in [all_known_pruefis.toml](src/kohlrahbi/all_known_pruefis.toml) and save them in the provided output path.
 
 ### `.docx` Data Sources
 kohlrahbi internally relies on a [specific naming schema](https://github.com/Hochfrequenz/kohlrahbi/blob/22a78dc076c7d5f9248cb9e8707b0cc14a2981d3/src/kohlrahbi/read_functions.py#L57) of the `.docx` files in which the file name holds information about the edifact format and validity period of the AHBs contained within the file.
 The easiest way to be compliant with this naming schema is to clone our [edi_energy_mirror](https://github.com/Hochfrequenz/edi_energy_mirror/) repository to your localhost.
 
 ### Get a specific Prüfidentifikator
 
 If you want to extract a specific prüfidentifikator, you can run the following command.
 
 ```bash
-kohlrahbi --input_path ../edi_energy_mirror/ --output_path ./output/ --pruefis 11039
+kohlrahbi --input_path ../edi_energy_mirror/edi_energy_de/current --output_path ./output/ --pruefis 11039 --file-type xslx
 ```
 
 You can also provide multiple prüfidentifikatoren.
 
 ```bash
-kohlrahbi --input_path ../edi_energy_mirror/ --output_path ./output/ --pruefis 11039 --pruefis 11040 --pruefi 11041
+kohlrahbi --input_path ../edi_energy_mirror/edi_energy_de/current --output_path ./output/ --pruefis 11039 --pruefis 11040 --pruefi 11041 --file-type csv
 ```
 
 ## Workflow
 
 ```mermaid
 flowchart TB
     S[Start] --> RD[Read docx]
```

### Comparing `kohlrahbi-0.0.3/requirements.txt` & `kohlrahbi-0.0.4/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,40 +5,44 @@
 #    pip-compile requirements.in
 #
 attrs==22.2.0
     # via
     #   -r requirements.in
     #   maus
 click==8.1.3
-    # via -r requirements.in
+    # via
+    #   -r requirements.in
+    #   maus
 colorlog==6.7.0
     # via -r requirements.in
 et-xmlfile==1.1.0
     # via openpyxl
 lxml==4.9.2
     # via python-docx
 marshmallow==3.19.0
     # via maus
-maus==0.3.2
+maus==0.3.11
     # via -r requirements.in
 more-itertools==9.0.0
     # via maus
 numpy==1.24.1
     # via pandas
-openpyxl==3.1.1
+openpyxl==3.1.2
     # via -r requirements.in
 packaging==22.0
     # via marshmallow
-pandas==1.5.3
+pandas==2.0.0
     # via -r requirements.in
 python-dateutil==2.8.2
     # via pandas
 python-docx==0.8.11
     # via -r requirements.in
-pytz==2022.7.1
+pytz==2023.3
     # via pandas
 six==1.16.0
     # via python-dateutil
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via -r requirements.in
-xlsxwriter==3.0.8
+tzdata==2023.3
+    # via pandas
+xlsxwriter==3.0.9
     # via -r requirements.in
```

### Comparing `kohlrahbi-0.0.3/tox.ini` & `kohlrahbi-0.0.4/tox.ini`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/.github/dependabot.yml` & `kohlrahbi-0.0.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/.github/workflows/black.yml` & `kohlrahbi-0.0.4/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/.github/workflows/coverage.yml` & `kohlrahbi-0.0.4/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/.github/workflows/packaging_test.yml` & `kohlrahbi-0.0.4/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/.github/workflows/python-publish.yml` & `kohlrahbi-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/.github/workflows/pythonlint.yml` & `kohlrahbi-0.0.4/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/.github/workflows/unittests.yml` & `kohlrahbi-0.0.4/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/__init__.py` & `kohlrahbi-0.0.4/src/kohlrahbi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     """
     if not path.exists():
         click.secho("⚠️ The output directory does not exist.", fg="red")
 
         if click.confirm(f"Should I try to create the directory at '{path}'?", default=True):
             try:
                 path.mkdir(exist_ok=True)
-                click.secho("📂 The output directory is created.", fg="yellow")
+                click.secho(f"📂 The output directory is created at {path.absolute()}.", fg="yellow")
             except FileNotFoundError as fnfe:
                 click.secho(
                     "😱 There was an path error. I can only create a new directory in an already existing directory.",
                     fg="red",
                 )
                 click.secho(f"Your given path is '{path}'", fg="red")
                 click.secho(str(fnfe), fg="red")
@@ -114,36 +114,44 @@
     help="Define the path where you want to save the generated files.",
 )
 @click.option(
     "--file-type",
     type=click.Choice(["flatahb", "csv", "xlsx"], case_sensitive=False),
     multiple=True,
 )
-def main(
-    pruefis: list[str],
-    input_path: Path,
-    output_path: Path,
-    file_type: list[str],
-):
+@click.option(
+    "--assume-yes",
+    "-y",
+    is_flag=True,
+    help="Confirm all prompts automatically.",
+)
+# pylint: disable=too-many-branches
+def main(pruefis: list[str], input_path: Path, output_path: Path, file_type: list[str], assume_yes: bool):
     """
     A program to get a machine readable version of the AHBs docx files published by edi@energy.
     """
     check_python_version()
 
-    check_output_path(path=output_path)
-
-    output_directory_path: Path = Path.cwd() / Path("output")
-    output_directory_path.mkdir(exist_ok=True)
+    if not assume_yes:
+        check_output_path(path=output_path)
+    else:
+        if output_path.exists():
+            click.secho(f"The output directory '{output_path}' exists already.", fg="yellow")
+        else:
+            output_path.mkdir(parents=True)
+            click.secho(f"I created a new directory at {output_path}", fg="yellow")
 
     if len(pruefis) == 0:
         click.secho("☝️ No pruefis were given. I will parse all known pruefis.", fg="yellow")
         pruefis = load_all_known_pruefis_from_file()
-
+    if len(file_type) == 0:
+        click.secho(
+            "ℹ You did not provide any value for the parameter --file-type. No files will be created.", fg="yellow"
+        )
     valid_pruefis: list[str] = get_valid_pruefis(list_of_pruefis=pruefis)
-
     if valid_pruefis == []:
         click.secho("⚠️ There are no valid pruefidentifkatoren.", fg="red")
         raise click.Abort()
 
     if len(valid_pruefis) != len(pruefis):
         click.secho("☝️ Not all given pruefidentifikatoren are valid.", fg="yellow")
         click.secho(f"I will continue with the following valid pruefis: {valid_pruefis}.", fg="yellow")
@@ -178,23 +186,25 @@
 
             if ahb_table is None:
                 continue
 
             if isinstance(ahb_table, AhbTable):
                 unfolded_ahb = UnfoldedAhb.from_ahb_table(ahb_table=ahb_table, pruefi=pruefi)
 
-                logger.info("💾 Saving files %s \n", pruefi)
                 if "xlsx" in file_type:
-                    unfolded_ahb.dump_xlsx(path_to_output_directory=output_directory_path)
+                    logger.info("💾 Saving xlsx file %s", pruefi)
+                    unfolded_ahb.dump_xlsx(path_to_output_directory=output_path)
 
                 if "flatahb" in file_type:
-                    unfolded_ahb.dump_flatahb_json(output_directory_path=output_directory_path)
+                    logger.info("💾 Saving flatahb file %s", pruefi)
+                    unfolded_ahb.dump_flatahb_json(output_directory_path=output_path)
 
                 if "csv" in file_type:
-                    unfolded_ahb.dump_csv(path_to_output_directory=output_directory_path)
+                    logger.info("💾 Saving csv file %s", pruefi)
+                    unfolded_ahb.dump_csv(path_to_output_directory=output_path)
 
                 break
 
 
 if __name__ == "__main__":
     # the parameter arguments gets provided over the CLI
     main()  # pylint:disable=no-value-for-parameter
```

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/ahbfilefinder.py` & `kohlrahbi-0.0.4/src/kohlrahbi/ahbfilefinder.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/all_known_pruefis.toml` & `kohlrahbi-0.0.4/src/kohlrahbi/all_known_pruefis.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/collect_pruefis.py` & `kohlrahbi-0.0.4/src/kohlrahbi/collect_pruefis.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/read_functions.py` & `kohlrahbi-0.0.4/src/kohlrahbi/read_functions.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/row_type_checker.py` & `kohlrahbi-0.0.4/src/kohlrahbi/row_type_checker.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module contains all functions to define the type of a row of the tables in an AHB.
 """
 from docx.oxml import OxmlElement  # type:ignore[import]
 from docx.oxml.ns import qn  # type:ignore[import]
 from docx.shared import RGBColor  # type:ignore[import]
 from docx.table import _Cell  # type:ignore[import]
 
-from kohlrahbi.enums import RowType, RowTypeColor
+from kohlrahbi.enums import RowType
 
 
 def set_table_header_bg_color(cell, hex_color: str):
     """
     set background shading for Header Rows
     """
     table_cell = cell._tc  # pylint:disable=protected-access
@@ -149,31 +149,25 @@
     Raises:
         NotImplemented: Gets raised if the RowType got not to be defined
 
     Returns:
         RowType: Type of the current row
     """
     if is_row_header(edifact_struktur_cell=edifact_struktur_cell):
-        set_table_header_bg_color(edifact_struktur_cell, RowTypeColor.HEADER)
         return RowType.HEADER
 
     if is_row_segmentname(edifact_struktur_cell=edifact_struktur_cell):
-        set_table_header_bg_color(edifact_struktur_cell, RowTypeColor.SEGMENTNAME)
         return RowType.SEGMENTNAME
 
     if is_row_segmentgruppe(edifact_struktur_cell=edifact_struktur_cell, left_indent_position=left_indent_position):
-        set_table_header_bg_color(edifact_struktur_cell, RowTypeColor.SEGMENTGRUPPE)
         return RowType.SEGMENTGRUPPE
 
     if is_row_segment(edifact_struktur_cell=edifact_struktur_cell, left_indent_position=left_indent_position):
-        set_table_header_bg_color(edifact_struktur_cell, RowTypeColor.SEGMENT)
         return RowType.SEGMENT
 
     if is_row_datenelement(edifact_struktur_cell=edifact_struktur_cell, left_indent_position=left_indent_position):
-        set_table_header_bg_color(edifact_struktur_cell, RowTypeColor.DATENELEMENT)
         return RowType.DATENELEMENT
 
     if is_row_empty(edifact_struktur_cell=edifact_struktur_cell):
-        set_table_header_bg_color(edifact_struktur_cell, RowTypeColor.EMPTY)
         return RowType.EMPTY
 
     raise NotImplementedError(f"Could not define row type of cell with text: {edifact_struktur_cell.text}")
```

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/seed.py` & `kohlrahbi-0.0.4/src/kohlrahbi/seed.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/ahb/ahbsubtable.py` & `kohlrahbi-0.0.4/src/kohlrahbi/ahb/ahbsubtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/ahb/ahbtable.py` & `kohlrahbi-0.0.4/src/kohlrahbi/ahb/ahbtable.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/ahb/ahbtablerow.py` & `kohlrahbi-0.0.4/src/kohlrahbi/ahb/ahbtablerow.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/docxtablecells/bedinungscell.py` & `kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/bedinungscell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/docxtablecells/bodycell.py` & `kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/bodycell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/docxtablecells/edifactstrukturcell.py` & `kohlrahbi-0.0.4/src/kohlrahbi/docxtablecells/edifactstrukturcell.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/enums/row_type.py` & `kohlrahbi-0.0.4/src/kohlrahbi/enums/row_type.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/unfoldedahb/unfoldedahbline.py` & `kohlrahbi-0.0.4/src/kohlrahbi/unfoldedahb/unfoldedahbline.py`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py` & `kohlrahbi-0.0.4/src/kohlrahbi/unfoldedahb/unfoldedahbtable.py`

 * *Files 3% similar despite different names*

```diff
@@ -273,30 +273,35 @@
             )
             raise
 
     def dump_flatahb_json(self, output_directory_path: Path) -> None:
         """
         Converts the unfolded AHB to a flat AHB and writes it to a json file.
         The file will be stored in the directory:
-            'output_directory_path/flatahb/<edifact_format>/<pruefidentifikator>.json'
+            'output_directory_path/<edifact_format>/flatahb/<pruefidentifikator>.json'
         """
         edifact_format = get_format_of_pruefidentifikator(self.meta_data.pruefidentifikator)
         if edifact_format is None:
             logger.warning("'%s' is not a pruefidentifikator", self.meta_data.pruefidentifikator)
             return
 
-        flatahb_output_directory_path = output_directory_path / "flatahb" / str(edifact_format)
+        flatahb_output_directory_path = output_directory_path / str(edifact_format) / "flatahb"
         flatahb_output_directory_path.mkdir(parents=True, exist_ok=True)
 
         dump_data = FlatAnwendungshandbuchSchema().dump(self.convert_to_flat_ahb())
 
         with open(
             flatahb_output_directory_path / f"{self.meta_data.pruefidentifikator}.json", "w", encoding="utf-8"
         ) as file:
-            json.dump(dump_data, file)
+            json.dump(dump_data, file, ensure_ascii=False, indent=2, sort_keys=True)
+        logger.info(
+            "The flatahb file for %s is saved at %s",
+            self.meta_data.pruefidentifikator,
+            flatahb_output_directory_path / f"{self.meta_data.pruefidentifikator}.json",
+        )
 
     def convert_to_dataframe(self) -> pd.DataFrame:
         """
         Converts the unfolded AHB to a pandas dataframe.
         """
         unfolded_ahb_lines = [
             {
@@ -317,41 +322,41 @@
         df.fillna(value="", inplace=True)
         return df
 
     def dump_csv(self, path_to_output_directory: Path) -> None:
         """
         Dump a UnfoldedAHB table into a csv file.
         The file will be stored in the directory:
-            'path_to_output_directory/csv/<edifact_format>/<pruefidentifikator>.csv'
+            'path_to_output_directory/<edifact_format>/csv/<pruefidentifikator>.csv'
         """
         df = self.convert_to_dataframe()
 
         edifact_format = get_format_of_pruefidentifikator(self.meta_data.pruefidentifikator)
         if edifact_format is None:
             logger.warning("'%s' is not a pruefidentifikator", self.meta_data.pruefidentifikator)
             return
 
-        csv_output_directory_path = path_to_output_directory / "csv" / str(edifact_format)
+        csv_output_directory_path = path_to_output_directory / str(edifact_format) / "csv"
         csv_output_directory_path.mkdir(parents=True, exist_ok=True)
 
         df.to_csv(csv_output_directory_path / f"{self.meta_data.pruefidentifikator}.csv")
         logger.info(
             "The csv file for %s is saved at %s",
             self.meta_data.pruefidentifikator,
             csv_output_directory_path / f"{self.meta_data.pruefidentifikator}.csv",
         )
 
     def dump_xlsx(self, path_to_output_directory: Path) -> None:
         """
         Dump a AHB table of a given pruefi into an excel file.
         The file will be stored in the directory:
-            'path_to_output_directory/xlsx/<edifact_format>/<pruefidentifikator>.xlsx'
+            'path_to_output_directory/<edifact_format>/xlsx/<pruefidentifikator>.xlsx'
         """
         edifact_format = get_format_of_pruefidentifikator(self.meta_data.pruefidentifikator)
-        xlsx_output_directory_path: Path = path_to_output_directory / "xlsx" / str(edifact_format)
+        xlsx_output_directory_path: Path = path_to_output_directory / str(edifact_format) / "xlsx"
         xlsx_output_directory_path.mkdir(parents=True, exist_ok=True)
 
         excel_file_name = f"{self.meta_data.pruefidentifikator}.xlsx"
 
         df = self.convert_to_dataframe()
 
         try:
@@ -365,7 +370,13 @@
                 wrap_format = workbook.add_format({"text_wrap": True})
                 for column_letter, column_width in _column_letter_width_mapping.items():
                     excel_header = f"{column_letter}:{column_letter}"
                     worksheet.set_column(excel_header, column_width, wrap_format)
                 logger.info("💾 Saved file(s) for Pruefidentifikator %s", self.meta_data.pruefidentifikator)
         except PermissionError:
             logger.error("The Excel file %s is open. Please close this file and try again.", excel_file_name)
+
+        logger.info(
+            "The xlsx file for %s is saved at %s",
+            self.meta_data.pruefidentifikator,
+            xlsx_output_directory_path / f"{self.meta_data.pruefidentifikator}.json",
+        )
```

### Comparing `kohlrahbi-0.0.3/temp/test-fobar.docx` & `kohlrahbi-0.0.4/temp/test-fobar.docx`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/.gitignore` & `kohlrahbi-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/pyproject.toml` & `kohlrahbi-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kohlrahbi-0.0.3/PKG-INFO` & `kohlrahbi-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kohlrahbi
-Version: 0.0.3
+Version: 0.0.4
 Summary: Tool to generate machine readable files from AHB documents
 Project-URL: Changelog, https://github.com/Hochfrequenz/kohlrahbi/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/kohlrahbi
 Author-email: Kevin Krechan <kevin.krechan@hochfrequenz.de>
 License: MIT
 Keywords: ahb,automation,bdew,edi@energy
 Classifier: Development Status :: 4 - Beta
@@ -53,15 +53,15 @@
 However, the technical specifications of this API are
 * prose
 * on DIN A4 pages.
 
 The Anwendungshandbücher are the epitome of digitization with some good intentions.
 
 Although the AHBs are publicly available as PDF or Word files on `edi-energy.de`, they are hardly accessible in a technical sense:
-* You cannot automatically extract information from the AHBs. 
+* You cannot automatically extract information from the AHBs.
 * You cannot run automatic comparisons between different versions.
 * You cannot automatically test your own API against the set of rules, described in the AHBs (as prose).
 * You cannot view or visualize the information from the AHBs in any more intuitive or practical way, than the raw tables from the AHB files.
 * ...any many more...
 
 The root cause for all these inaccessibility is a technical one:
 Information that are theoretically structured are published in an unstructured format (PDF or Word), which is not suited for technical specifications in IT.
@@ -102,39 +102,41 @@
 ```
 
 ## Usage
 
 There are two ways to use kohlrahbi.
 1. You can extract all prüfidentifikatoren listed in [all_known_pruefis.toml,](src/kohlrahbi/all_known_pruefis.toml)
 2. or you can extract a specific prüfidentifikator.
+
 ### Get all Prüfidentifikatoren
 If you want to extract all prüfidentifikatoren, you can run the following command.
+For the following steps we assume that you cloned our [edi_energy_mirror](https://github.com/Hochfrequenz/edi_energy_mirror/) to a neighbouring directory.
 
 ```bash
-kohlrahbi --input_path ../edi_energy_mirror/ --output_path ./output/
+kohlrahbi --input_path ../edi_energy_mirror/edi_energy_de/current --output_path ./output/ --file-type flatahb
 ```
 
 This will extract all prüfidentifikatoren listed in [all_known_pruefis.toml](src/kohlrahbi/all_known_pruefis.toml) and save them in the provided output path.
 
 ### `.docx` Data Sources
 kohlrahbi internally relies on a [specific naming schema](https://github.com/Hochfrequenz/kohlrahbi/blob/22a78dc076c7d5f9248cb9e8707b0cc14a2981d3/src/kohlrahbi/read_functions.py#L57) of the `.docx` files in which the file name holds information about the edifact format and validity period of the AHBs contained within the file.
 The easiest way to be compliant with this naming schema is to clone our [edi_energy_mirror](https://github.com/Hochfrequenz/edi_energy_mirror/) repository to your localhost.
 
 ### Get a specific Prüfidentifikator
 
 If you want to extract a specific prüfidentifikator, you can run the following command.
 
 ```bash
-kohlrahbi --input_path ../edi_energy_mirror/ --output_path ./output/ --pruefis 11039
+kohlrahbi --input_path ../edi_energy_mirror/edi_energy_de/current --output_path ./output/ --pruefis 11039 --file-type xslx
 ```
 
 You can also provide multiple prüfidentifikatoren.
 
 ```bash
-kohlrahbi --input_path ../edi_energy_mirror/ --output_path ./output/ --pruefis 11039 --pruefis 11040 --pruefi 11041
+kohlrahbi --input_path ../edi_energy_mirror/edi_energy_de/current --output_path ./output/ --pruefis 11039 --pruefis 11040 --pruefi 11041 --file-type csv
 ```
 
 ## Workflow
 
 ```mermaid
 flowchart TB
     S[Start] --> RD[Read docx]
```

