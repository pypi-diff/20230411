# Comparing `tmp/leximpact_prepare_data-0.0.8.tar.gz` & `tmp/leximpact_prepare_data-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leximpact_prepare_data-0.0.8.tar", max compression
+gzip compressed data, was "leximpact_prepare_data-0.0.9.tar", max compression
```

## Comparing `leximpact_prepare_data-0.0.8.tar` & `leximpact_prepare_data-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    34523 2022-03-16 18:53:20.625224 leximpact_prepare_data-0.0.8/LICENSE
--rw-r--r--   0        0        0     1791 2022-03-22 15:16:42.396336 leximpact_prepare_data-0.0.8/README.md
--rw-r--r--   0        0        0       22 2022-03-22 16:27:46.945443 leximpact_prepare_data-0.0.8/leximpact_prepare_data/__init__.py
--rw-r--r--   0        0        0     4966 2022-03-22 16:27:46.945443 leximpact_prepare_data-0.0.8/leximpact_prepare_data/_nbdev.py
--rw-r--r--   0        0        0    11594 2022-03-22 16:27:46.945443 leximpact_prepare_data-0.0.8/leximpact_prepare_data/aging_tools.py
--rw-r--r--   0        0        0    33180 2022-03-22 16:27:46.945443 leximpact_prepare_data-0.0.8/leximpact_prepare_data/calib_and_copules.py
--rw-r--r--   0        0        0    42821 2022-03-22 16:27:46.945443 leximpact_prepare_data-0.0.8/leximpact_prepare_data/calibration_tools.py
--rw-r--r--   0        0        0    10660 2022-03-22 16:27:46.945443 leximpact_prepare_data-0.0.8/leximpact_prepare_data/calmar_tools.py
--rw-r--r--   0        0        0     4947 2022-03-22 16:27:46.945443 leximpact_prepare_data-0.0.8/leximpact_prepare_data/copules_add_var.py
--rw-r--r--   0        0        0     2521 2022-03-22 16:27:46.945443 leximpact_prepare_data-0.0.8/leximpact_prepare_data/enlargement.py
--rw-r--r--   0        0        0      146 2022-03-22 16:27:46.945443 leximpact_prepare_data-0.0.8/leximpact_prepare_data/fusion_fake.py
--rw-r--r--   0        0        0     9483 2022-03-22 16:27:46.945443 leximpact_prepare_data-0.0.8/leximpact_prepare_data/monte_carlo.py
--rw-r--r--   0        0        0     3719 2022-03-22 16:27:46.945443 leximpact_prepare_data-0.0.8/leximpact_prepare_data/reduce_data.py
--rw-r--r--   0        0        0    11420 2022-03-22 16:27:46.945443 leximpact_prepare_data-0.0.8/leximpact_prepare_data/toolbase.py
--rw-r--r--   0        0        0     2109 2022-03-22 14:26:16.906425 leximpact_prepare_data-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3092 2022-03-22 16:29:19.605361 leximpact_prepare_data-0.0.8/setup.py
--rw-r--r--   0        0        0     3117 2022-03-22 16:29:19.605656 leximpact_prepare_data-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2022-03-27 08:29:47.188782 leximpact_prepare_data-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1791 2022-03-27 08:29:47.188782 leximpact_prepare_data-0.0.9/README.md
+-rw-r--r--   0        0        0       22 2022-03-27 20:19:50.038798 leximpact_prepare_data-0.0.9/leximpact_prepare_data/__init__.py
+-rw-r--r--   0        0        0     4966 2022-03-27 20:19:50.038798 leximpact_prepare_data-0.0.9/leximpact_prepare_data/_nbdev.py
+-rw-r--r--   0        0        0    11594 2022-03-27 20:19:50.038798 leximpact_prepare_data-0.0.9/leximpact_prepare_data/aging_tools.py
+-rw-r--r--   0        0        0    33180 2022-03-27 20:19:50.038798 leximpact_prepare_data-0.0.9/leximpact_prepare_data/calib_and_copules.py
+-rw-r--r--   0        0        0    42821 2022-03-27 20:19:50.038798 leximpact_prepare_data-0.0.9/leximpact_prepare_data/calibration_tools.py
+-rw-r--r--   0        0        0    10660 2022-03-27 20:19:50.038798 leximpact_prepare_data-0.0.9/leximpact_prepare_data/calmar_tools.py
+-rw-r--r--   0        0        0     4947 2022-03-27 20:19:50.038798 leximpact_prepare_data-0.0.9/leximpact_prepare_data/copules_add_var.py
+-rw-r--r--   0        0        0     2521 2022-03-27 20:19:50.038798 leximpact_prepare_data-0.0.9/leximpact_prepare_data/enlargement.py
+-rw-r--r--   0        0        0      146 2022-03-27 20:19:50.038798 leximpact_prepare_data-0.0.9/leximpact_prepare_data/fusion_fake.py
+-rw-r--r--   0        0        0     9483 2022-03-27 20:19:50.038798 leximpact_prepare_data-0.0.9/leximpact_prepare_data/monte_carlo.py
+-rw-r--r--   0        0        0     3719 2022-03-27 20:19:50.038798 leximpact_prepare_data-0.0.9/leximpact_prepare_data/reduce_data.py
+-rw-r--r--   0        0        0    11420 2022-03-27 20:19:50.038798 leximpact_prepare_data-0.0.9/leximpact_prepare_data/toolbase.py
+-rw-r--r--   0        0        0     2109 2022-03-27 20:12:36.747514 leximpact_prepare_data-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3092 2022-03-27 20:21:23.456471 leximpact_prepare_data-0.0.9/setup.py
+-rw-r--r--   0        0        0     3117 2022-03-27 20:21:23.456771 leximpact_prepare_data-0.0.9/PKG-INFO
```

### Comparing `leximpact_prepare_data-0.0.8/LICENSE` & `leximpact_prepare_data-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `leximpact_prepare_data-0.0.8/README.md` & `leximpact_prepare_data-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `leximpact_prepare_data-0.0.8/leximpact_prepare_data/_nbdev.py` & `leximpact_prepare_data-0.0.9/leximpact_prepare_data/_nbdev.py`

 * *Files identical despite different names*

### Comparing `leximpact_prepare_data-0.0.8/leximpact_prepare_data/aging_tools.py` & `leximpact_prepare_data-0.0.9/leximpact_prepare_data/aging_tools.py`

 * *Files identical despite different names*

### Comparing `leximpact_prepare_data-0.0.8/leximpact_prepare_data/calib_and_copules.py` & `leximpact_prepare_data-0.0.9/leximpact_prepare_data/calib_and_copules.py`

 * *Files identical despite different names*

### Comparing `leximpact_prepare_data-0.0.8/leximpact_prepare_data/calibration_tools.py` & `leximpact_prepare_data-0.0.9/leximpact_prepare_data/calibration_tools.py`

 * *Files identical despite different names*

### Comparing `leximpact_prepare_data-0.0.8/leximpact_prepare_data/calmar_tools.py` & `leximpact_prepare_data-0.0.9/leximpact_prepare_data/calmar_tools.py`

 * *Files identical despite different names*

### Comparing `leximpact_prepare_data-0.0.8/leximpact_prepare_data/copules_add_var.py` & `leximpact_prepare_data-0.0.9/leximpact_prepare_data/copules_add_var.py`

 * *Files identical despite different names*

### Comparing `leximpact_prepare_data-0.0.8/leximpact_prepare_data/enlargement.py` & `leximpact_prepare_data-0.0.9/leximpact_prepare_data/enlargement.py`

 * *Files identical despite different names*

### Comparing `leximpact_prepare_data-0.0.8/leximpact_prepare_data/monte_carlo.py` & `leximpact_prepare_data-0.0.9/leximpact_prepare_data/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `leximpact_prepare_data-0.0.8/leximpact_prepare_data/reduce_data.py` & `leximpact_prepare_data-0.0.9/leximpact_prepare_data/reduce_data.py`

 * *Files identical despite different names*

### Comparing `leximpact_prepare_data-0.0.8/leximpact_prepare_data/toolbase.py` & `leximpact_prepare_data-0.0.9/leximpact_prepare_data/toolbase.py`

 * *Files identical despite different names*

### Comparing `leximpact_prepare_data-0.0.8/pyproject.toml` & `leximpact_prepare_data-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leximpact_prepare_data"
-version = "0.0.8"
+version = "0.0.9"
 description = "Prepare data for LexImpact"
 authors = ["LexImpact <leximpact@an.fr>"]
 license = "AGPL-3.0"
 readme = "README.md"
 homepage = "https://leximpact.an.fr/"
 repository = "https://git.leximpact.dev/leximpact/leximpact-prepare-data"
```

### Comparing `leximpact_prepare_data-0.0.8/setup.py` & `leximpact_prepare_data-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                           'diagrams[pipeline]>=0.20.0,<0.21.0',
                           'vaex-core[pipeline]>=4.8.0,<5.0.0',
                           'tables[pipeline]>=3.6.1,<4.0.0',
                           'python-dotenv[pipeline]>=0.19.2,<0.20.0']}
 
 setup_kwargs = {
     'name': 'leximpact-prepare-data',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Prepare data for LexImpact',
     'long_description': "# LexImpact Prepare Data\n\n\n\nCe projet regroupe les scripts permettant de préparer les données des différents projets [Leximpact](https://leximpact.an.fr).\n\n## Schéma complet de préparation et d'utilisation des données\n![LexImpact Pipeline](notebooks/schemas/leximpact_pipeline.png)\n\n\n    \nLe pipeline prepare-data est donc le suivant :\n\nInput: erfs_flat_2018.h5\n\n### 01_db_reduce.ipynb   \nObjectif: Réduit le nombre de variables dans la base\n\nOutput: 01_erfs_reduced_2018.h5\n\n### 02_db_enlarge.ipynb\nObjectif: Ajoute des gens fictifs dans la base pour pouvoir calibrer\n\n\nOutput: 02_erfs_enlarged_2018.h5\n\n\n### 03_db_add_rfr.ipynb\nInput : CalibPote-2018-revkire.json\n\nObjectifs: \n-\tCalculer le RFR dans OpenFisca\n-\tCalibrer le RFR ERFS_2018 sur POTE_2018\n\nOutput: 03_erfs_rfr_2018.h5\n\n\n### 04_db_add_var\n0403_db_add_var_copules.ipynb\n\n0401_db_add_var_copules-algo_monte-carlo.ipynb  \n\n\n0402_db_add_var_copules-validate.ipynb\n\nInput : ExportCopule-2018-variable.json\n\nObjectif: Ajoute les variables issues de POTE 2018 dans la base ERFS 2018\n\nOutput:  04_erfs_var_copules_2018.h5\n\n\n### 05_db_calib_var_copules.ipynb\n\nInput : CalibPote-2019-variable.json\n\nObjectifs: \n-\tVieillit la base ERFS_2018 vers 2019 (nos données les plus récentes) : inflation économique et inflation des foyers\n-\tCalibre chacune des variables issues de POTE sur POTE 2019\n\nOutput:  05_erfs_calibrated_ff_2018_to_2019.h5\n\n### 06_db_aging_final.ipynb\nObjectifs:\n\n-\tVieillit la base ERFS_2019 vers 2021 (année voulue pour les calculs) : inflation économique et inflation des foyers\n-\tBruitage statistique de la base pour anonymisation\n\nOutput: 06_erfs_ff_2018_aged_2021.h5\n\n    \n\n# How to contribute\n\nPlease see the [contributing page](https://documentation.leximpact.dev/leximpact_prepare_data/contributing).\n",
     'author': 'LexImpact',
     'author_email': 'leximpact@an.fr',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://leximpact.an.fr/',
```

### Comparing `leximpact_prepare_data-0.0.8/PKG-INFO` & `leximpact_prepare_data-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leximpact-prepare-data
-Version: 0.0.8
+Version: 0.0.9
 Summary: Prepare data for LexImpact
 Home-page: https://leximpact.an.fr/
 License: AGPL-3.0
 Author: LexImpact
 Author-email: leximpact@an.fr
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

