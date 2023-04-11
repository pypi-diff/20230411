# Comparing `tmp/open_mastr-0.13.0.tar.gz` & `tmp/open_mastr-0.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_mastr-0.13.0.tar", last modified: Thu Feb 16 12:36:29 2023, max compression
+gzip compressed data, was "open_mastr-0.13.1.tar", last modified: Tue Apr 11 08:53:57 2023, max compression
```

## Comparing `open_mastr-0.13.0.tar` & `open_mastr-0.13.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:36:29.184469 open_mastr-0.13.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34521 2023-02-16 12:36:20.000000 open_mastr-0.13.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-02-16 12:36:29.184469 open_mastr-0.13.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-02-16 12:36:20.000000 open_mastr-0.13.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:36:29.180469 open_mastr-0.13.0/open_mastr/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/mastr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:36:29.180469 open_mastr-0.13.0/open_mastr/soap_api/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/soap_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48299 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/soap_api/download.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:36:29.180469 open_mastr-0.13.0/open_mastr/soap_api/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/soap_api/metadata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/soap_api/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15770 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/soap_api/metadata/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/soap_api/metadata/description.py
--rw-r--r--   0 runner    (1001) docker     (123)    41889 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/soap_api/mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/soap_api/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/soap_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:36:29.184469 open_mastr-0.13.0/open_mastr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:36:29.184469 open_mastr-0.13.0/open_mastr/utils/config/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/utils/config/logging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/utils/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/utils/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    35412 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/utils/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:36:29.184469 open_mastr-0.13.0/open_mastr/xml_download/
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/xml_download/colums_to_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/xml_download/utils_cleansing_bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/xml_download/utils_download_bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-02-16 12:36:20.000000 open_mastr-0.13.0/open_mastr/xml_download/utils_write_to_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:36:29.180469 open_mastr-0.13.0/open_mastr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-02-16 12:36:29.000000 open_mastr-0.13.0/open_mastr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-02-16 12:36:29.000000 open_mastr-0.13.0/open_mastr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 12:36:29.000000 open_mastr-0.13.0/open_mastr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-16 12:36:29.000000 open_mastr-0.13.0/open_mastr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-16 12:36:29.000000 open_mastr-0.13.0/open_mastr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-16 12:36:29.184469 open_mastr-0.13.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-02-16 12:36:20.000000 open_mastr-0.13.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 12:36:29.184469 open_mastr-0.13.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-16 12:36:20.000000 open_mastr-0.13.0/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-02-16 12:36:20.000000 open_mastr-0.13.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-16 12:36:20.000000 open_mastr-0.13.0/tests/test_mastr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.817996 open_mastr-0.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34521 2023-04-11 08:53:46.000000 open_mastr-0.13.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-04-11 08:53:57.817996 open_mastr-0.13.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-11 08:53:46.000000 open_mastr-0.13.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.813996 open_mastr-0.13.1/open_mastr/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/mastr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.813996 open_mastr-0.13.1/open_mastr/soap_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48271 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/download.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.813996 open_mastr-0.13.1/open_mastr/soap_api/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/metadata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15770 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/metadata/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/metadata/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41853 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/soap_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.813996 open_mastr-0.13.1/open_mastr/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.813996 open_mastr-0.13.1/open_mastr/utils/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/config/logging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25342 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36267 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/utils/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.817996 open_mastr-0.13.1/open_mastr/xml_download/
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/xml_download/colums_to_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/xml_download/utils_cleansing_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/xml_download/utils_download_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-04-11 08:53:46.000000 open_mastr-0.13.1/open_mastr/xml_download/utils_write_to_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.813996 open_mastr-0.13.1/open_mastr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-04-11 08:53:57.000000 open_mastr-0.13.1/open_mastr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-11 08:53:57.000000 open_mastr-0.13.1/open_mastr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:53:57.000000 open_mastr-0.13.1/open_mastr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 08:53:57.000000 open_mastr-0.13.1/open_mastr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 08:53:57.000000 open_mastr-0.13.1/open_mastr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-11 08:53:57.817996 open_mastr-0.13.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-11 08:53:47.000000 open_mastr-0.13.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:53:57.817996 open_mastr-0.13.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-11 08:53:47.000000 open_mastr-0.13.1/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-04-11 08:53:47.000000 open_mastr-0.13.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-11 08:53:47.000000 open_mastr-0.13.1/tests/test_mastr.py
```

### Comparing `open_mastr-0.13.0/LICENSE.md` & `open_mastr-0.13.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/PKG-INFO` & `open_mastr-0.13.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: open_mastr
-Version: 0.13.0
+Version: 0.13.1
 Summary: A package that provides an interface for downloading and processing the data of the Marktstammdatenregister (MaStR)
 Home-page: https://github.com/OpenEnergyPlatform/open-MaStR
-Download-URL: https://github.com/OpenEnergyPlatform/open-MaStR/archive/refs/tags/v0.13.0.tar.gz
+Download-URL: https://github.com/OpenEnergyPlatform/open-MaStR/archive/refs/tags/v0.13.1.tar.gz
 Author: Open Energy Family
 Author-email: datenzentrum@rl-institut.de
 Maintainer: Ludwig Hülk
 Maintainer-email: datenzentrum@rl-institut.de
 Project-URL: Documentation, https://open-mastr.readthedocs.io/
 Project-URL: Changelog, https://open-mastr.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/OpenEnergyPlatform/open-MaStR/issues
```

### Comparing `open_mastr-0.13.0/README.rst` & `open_mastr-0.13.1/README.rst`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/open_mastr/mastr.py` & `open_mastr-0.13.1/open_mastr/mastr.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
                 "electricity_consumer", "Yes", "No"
                 "location", "Yes", "Yes"
                 "market", "Yes", "No"
                 "grid", "Yes", "No"
                 "balancing_area", "Yes", "No"
                 "permit", "Yes", "Yes"
                 "deleted_units", "Yes", "No"
+                "retrofit_units", "Yes", "No"
 
         date: None or :class:`datetime.datetime` or str, optional
             For bulk method:
 
             Either "today" or None if the newest data dump should be downloaded
             rom the MaStR website. If an already downloaded dump should be used,
             state the date of the download in the format
```

### Comparing `open_mastr-0.13.0/open_mastr/soap_api/download.py` & `open_mastr-0.13.1/open_mastr/soap_api/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -475,23 +475,23 @@
                     "NichtBiogenerAbfall",
                     "Waerme",
                 ],
                 "kwk_data": "GetAnlageKwk",
                 "permit_data": "GetEinheitGenehmigung",
             },
             "gsgk": {
-                "unit_data": "GetEinheitGeoSolarthermieGrubenKlaerschlammDruckentspannung",
+                "unit_data": "GetEinheitGeothermieGrubengasDruckentspannung",
                 "energietraeger": [
                     "Geothermie",
                     "Solarthermie",
                     "Grubengas",
                     "Klaerschlamm",
                 ],
                 "kwk_data": "GetAnlageKwk",
-                "eeg_data": "GetAnlageEegGeoSolarthermieGrubenKlaerschlammDruckentspannung",
+                "eeg_data": "GetAnlageEegGeothermieGrubengasDruckentspannung",
                 "permit_data": "GetEinheitGenehmigung",
             },
             "nuclear": {
                 "unit_data": "GetEinheitKernkraft",
                 "energietraeger": ["Kernenergie"],
                 "permit_data": "GetEinheitGenehmigung",
             },
```

### Comparing `open_mastr-0.13.0/open_mastr/soap_api/metadata/LICENSE` & `open_mastr-0.13.1/open_mastr/soap_api/metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/open_mastr/soap_api/metadata/create.py` & `open_mastr-0.13.1/open_mastr/soap_api/metadata/create.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/open_mastr/soap_api/metadata/description.py` & `open_mastr-0.13.1/open_mastr/soap_api/metadata/description.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/open_mastr/soap_api/mirror.py` & `open_mastr-0.13.1/open_mastr/soap_api/mirror.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,15 +314,15 @@
                     break
 
                 # Retrieve data
                 unit_data, missed_units = self.mastr_dl.additional_data(
                     data, requested_ids, download_functions[data_type]
                 )
 
-                unit_data = flatten_dict(unit_data)
+                unit_data = flatten_dict(unit_data, serialize_with_json=False)
                 number_units_merged = 0
 
                 # Prepare data and add to database table
                 for unit_dat in unit_data:
                     unit = self._preprocess_additional_data_entry(
                         unit_dat, data, data_type
                     )
@@ -835,28 +835,29 @@
                 if ertuechtigung["DatumWiederinbetriebnahme"]:
                     ertuechtigung["DatumWiederinbetriebnahme"] = ertuechtigung[
                         "DatumWiederinbetriebnahme"
                     ].isoformat()
                 ertuechtigung["ProzentualeErhoehungDesLv"] = float(
                     ertuechtigung["ProzentualeErhoehungDesLv"]
                 )
-        # The NetzbetreiberMastrNummer is handed over as type:list, hence
-        # non-compatible with sqlite)
-        # This replaces the list with the first (string)element in the list
-        # to make it sqlite compatible
-        if (
-            "NetzbetreiberMastrNummer" in unit_dat
-            and type(unit_dat["NetzbetreiberMastrNummer"]) == list
-        ):
-            if len(unit_dat["NetzbetreiberMastrNummer"]) > 0:
-                unit_dat["NetzbetreiberMastrNummer"] = unit_dat[
-                    "NetzbetreiberMastrNummer"
-                ][0]
-            else:
-                unit_dat["NetzbetreiberMastrNummer"] = None
+        # Some data (data_in_list) is handed over as type:list, hence
+        # non-compatible with sqlite or postgresql
+        # This replaces the list with the first element in the list
+
+        data_as_list = ["NetzbetreiberMastrNummer","Netzbetreiberzuordnungen"]
+
+        for dat in data_as_list:
+            if (
+                dat in unit_dat
+                and type(unit_dat[dat]) == list
+            ):
+                if len(unit_dat[dat]) > 0:
+                    unit_dat[dat] = f"{unit_dat[dat][0]}"
+                else:
+                    unit_dat[dat] = None
 
         # Rename the typo in column zugeordneteWirkleistungWechselrichter
         if "zugeordneteWirkleistungWechselrichter" in unit_dat.keys():
             unit_dat["ZugeordneteWirkleistungWechselrichter"] = unit_dat.pop(
                 "zugeordneteWirkleistungWechselrichter"
             )
```

### Comparing `open_mastr-0.13.0/open_mastr/soap_api/parallel.py` & `open_mastr-0.13.1/open_mastr/soap_api/parallel.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/open_mastr/soap_api/utils.py` & `open_mastr-0.13.1/open_mastr/soap_api/utils.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/open_mastr/utils/config.py` & `open_mastr-0.13.1/open_mastr/utils/config.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/open_mastr/utils/constants.py` & `open_mastr-0.13.1/open_mastr/utils/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "electricity_consumer",
     "location",
     "market",
     "grid",
     "balancing_area",
     "permit",
     "deleted_units",
+    "retrofit_units",
 ]
 
 # Possible values for parameter 'data' with API download method
 API_DATA = [
     "wind",
     "solar",
     "biomass",
@@ -55,15 +56,16 @@
     "gas_storage_extended",
     "grid_connections",
     "grids",
     "locations_extended",
     "market_actors",
     "market_roles",
     "permit",
-    "deleted_units"
+    "deleted_units",
+    "retrofit_units",
 ]
 
 # Possible data types for API download
 API_DATA_TYPES = ["unit_data", "eeg_data", "kwk_data", "permit_data"]
 
 # Possible location types for API download
 API_LOCATION_TYPES = [
@@ -95,14 +97,15 @@
     "electricity_consumer": ["einheitenstromverbraucher"],
     "location": ["lokationen"],
     "market": ["marktakteure", "marktrollen"],
     "grid": ["netzanschlusspunkte", "netze"],
     "balancing_area": ["bilanzierungsgebiete"],
     "permit": ["einheitengenehmigung"],
     "deleted_units": ["geloeschteunddeaktivierteeinheiten"],
+    "retrofit_units": ["ertuechtigungen"],
 }
 
 # Map bulk data to database table names, for csv export
 BULK_ADDITIONAL_TABLES_CSV_EXPORT_MAP = {
     "gas": [
         "gas_consumer",
         "gas_producer",
@@ -112,14 +115,15 @@
     "electricity_consumer": ["electricity_consumer"],
     "location": ["locations_extended"],
     "market": ["market_actors", "market_roles"],
     "grid": ["grid_connections", "grids"],
     "balancing_area": ["balancing_area"],
     "permit": ["permit"],
     "deleted_units": ["deleted_units"],
+    "retrofit_units": ["retrofit_units"],
 }
 
 # used to map the parameter options in open-mastr to the exact table class names in orm.py
 ORM_MAP = {
     "wind": {
         "unit_data": "WindExtended",
         "eeg_data": "WindEeg",
@@ -148,18 +152,15 @@
         "permit_data": "Permit",
     },
     "hydro": {
         "unit_data": "HydroExtended",
         "eeg_data": "HydroEeg",
         "permit_data": "Permit",
     },
-    "nuclear": {
-        "unit_data": "NuclearExtended",
-        "permit_data": "Permit"
-    },
+    "nuclear": {"unit_data": "NuclearExtended", "permit_data": "Permit"},
     "storage": {
         "unit_data": "StorageExtended",
         "eeg_data": "StorageEeg",
         "permit_data": "Permit",
     },
     "gas_consumer": "GasConsumer",
     "gas_producer": "GasProducer",
@@ -169,19 +170,19 @@
     "locations_extended": "LocationExtended",
     "market_actors": "MarketActors",
     "market_roles": "MarketRoles",
     "grid_connections": "GridConnections",
     "grids": "Grids",
     "balancing_area": "BalancingArea",
     "permit": "Permit",
-    "deleted_units": "DeletedUnits"
+    "deleted_units": "DeletedUnits",
+    "retrofit_units": "RetrofitUnits",
 }
 
 
-
 UNIT_TYPE_MAP = {
     "Windeinheit": "wind",
     "Solareinheit": "solar",
     "Biomasse": "biomass",
     "Wasser": "hydro",
     "Geothermie": "gsgk",
     "Verbrennung": "combustion",
```

### Comparing `open_mastr-0.13.0/open_mastr/utils/credentials.py` & `open_mastr-0.13.1/open_mastr/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/open_mastr/utils/docs.py` & `open_mastr-0.13.1/open_mastr/utils/docs.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/open_mastr/utils/helpers.py` & `open_mastr-0.13.1/open_mastr/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/open_mastr/utils/orm.py` & `open_mastr-0.13.1/open_mastr/utils/orm.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     Anlagenbetreiber = Column(String)
     EegMastrNummer = Column(String)
     KwkMastrNummer = Column(String)
     SpeMastrNummer = Column(String)
     GenMastrNummer = Column(String)
     BestandsanlageMastrNummer = Column(String)
     NichtVorhandenInMigriertenEinheiten = Column(String)
+    EinheitSystemstatus = Column(String)
 
 
 class AdditionalDataRequested(Base):
     __tablename__ = "additional_data_requested"
 
     id = Column(
         Integer,
@@ -130,14 +131,15 @@
     Einsatzverantwortlicher = Column(String)
     FernsteuerbarkeitNb = Column(Boolean)
     FernsteuerbarkeitDv = Column(Boolean)
     FernsteuerbarkeitDr = Column(Boolean)
     Einspeisungsart = Column(String)
     PraequalifiziertFuerRegelenergie = Column(Boolean)
     GenMastrNummer = Column(String)
+    Netzbetreiberzuordnungen = Column(String)
     # from bulk download
     Hausnummer_nv = Column(Boolean)
     Weic_nv = Column(Boolean)
     Kraftwerksnummer_nv = Column(Boolean)
 
 
 class WindExtended(Extended, ParentAllTables, Base):
@@ -223,14 +225,15 @@
     BestandteilGrenzkraftwerk = Column(Boolean)
     NettonennleistungDeutschland = Column(Float)
     AnteiligNutzungsberechtigte = Column(String)
     Notstromaggregat = Column(Boolean)
     Einsatzort = Column(String)
     KwkMastrNummer = Column(String)
     Technologie = Column(String)
+    AusschliesslicheVerwendungImKombibetrieb = Column(Boolean)
 
 
 class GsgkExtended(Extended, ParentAllTables, Base):
     __tablename__ = "gsgk_extended"
 
     Technologie = Column(String)
     KwkMastrNummer = Column(String)
@@ -288,14 +291,15 @@
     DatumLetzteAktualisierung = Column(DateTime(timezone=True))
     EegInbetriebnahmedatum = Column(Date)
     VerknuepfteEinheit = Column(String)
     AnlagenschluesselEeg = Column(String)
     AusschreibungZuschlag = Column(Boolean)
     AnlagenkennzifferAnlagenregister = Column(String)
     AnlagenkennzifferAnlagenregister_nv = Column(Boolean)
+    Netzbetreiberzuordnungen = Column(String)
 
 
 class WindEeg(Eeg, ParentAllTables, Base):
     __tablename__ = "wind_eeg"
 
     PrototypAnlage = Column(Boolean)
     PilotAnlage = Column(Boolean)
@@ -381,14 +385,15 @@
     Inbetriebnahmedatum = Column(Date)
     Meldedatum = Column(Date)
     ThermischeNutzleistung = Column(Float)
     ElektrischeKwkLeistung = Column(Float)
     VerknuepfteEinheiten = Column(String)
     AnlageBetriebsstatus = Column(String)
     AusschreibungZuschlag = Column(Boolean)
+    Netzbetreiberzuordnungen = Column(String)
 
 
 class Permit(ParentAllTables, Base):
     __tablename__ = "permit"
 
     Registrierungsdatum = Column(Date)
     GenMastrNummer = Column(String, primary_key=True)
@@ -400,14 +405,15 @@
     Frist = Column(Date)
     WasserrechtsNummer = Column(String)
     WasserrechtAblaufdatum = Column(Date)
     Meldedatum = Column(Date)
     VerknuepfteEinheiten = Column(String)
     Frist_nv = Column(Boolean)
     WasserrechtAblaufdatum_nv = Column(Boolean)
+    Netzbetreiberzuordnungen = Column(String)
 
 
 class LocationBasic(Base):
     __tablename__ = "locations_basic"
 
     LokationMastrNummer = Column(String, primary_key=True)
     NameDerTechnischenLokation = Column(String)
@@ -737,14 +743,15 @@
     MastrNummer = Column(String, primary_key=True)
     DatumLetzteAktualisierung = Column(DateTime(timezone=True))
     Sparte = Column(String)
     KundenAngeschlossen = Column(String)
     GeschlossenesVerteilnetz = Column(String)
     Bezeichnung = Column(String)
     Marktgebiet = Column(String)
+    Bundesland = Column(String)
 
 
 class GridConnections(ParentAllTables, Base):
     __tablename__ = "grid_connections"
 
     NetzanschlusspunktMastrNummer = Column(String, primary_key=True)
     NetzanschlusspunktBezeichnung = Column(String)
@@ -770,14 +777,26 @@
     DatumLetzteAktualisierung = Column(DateTime(timezone=True))
     EinheitMastrNummer = Column(String, primary_key=True)
     Einheittyp = Column(String)
     EinheitSystemstatus = Column(String)
     EinheitBetriebsstatus = Column(String)
 
 
+class RetrofitUnits(ParentAllTables, Base):
+    __tablename__ = "retrofit_units"
+
+    Id = Column(Integer, primary_key=True)
+    EegMastrNummer = Column(String)
+    Leistungserhoehung = Column(Float)
+    WiederinbetriebnahmeDatum = Column(Date)
+    DatumLetzteAktualisierung = Column(DateTime(timezone=True))
+    Ertuechtigungsart = Column(String)
+    ErtuechtigungIstZulassungspflichtig = Column(Boolean)
+
+
 tablename_mapping = {
     "anlageneegbiomasse": {
         "__name__": BiomassEeg.__tablename__,
         "__class__": BiomassEeg,
         "replace_column_names": {
             "EegMaStRNummer": "EegMastrNummer",
             "VerknuepfteEinheitenMaStRNummern": "VerknuepfteEinheit",
@@ -789,23 +808,23 @@
         "__class__": BiomassExtended,
         "replace_column_names": {
             "EegMaStRNummer": "EegMastrNummer",
             "KwkMaStRNummer": "KwkMastrNummer",
             "LokationMaStRNummer": "LokationMastrNummer",
         },
     },
-    "anlageneeggeosolarthermiegrubenklaerschlammdruckentspannung": {
+    "anlageneeggeothermiegrubengasdruckentspannung": {
         "__name__": GsgkEeg.__tablename__,
         "__class__": GsgkEeg,
         "replace_column_names": {
             "EegMaStRNummer": "EegMastrNummer",
             "VerknuepfteEinheitenMaStRNummern": "VerknuepfteEinheit",
         },
     },
-    "einheitengeosolarthermiegrubenklaerschlammdruckentspannung": {
+    "einheitengeothermiegrubengasdruckentspannung": {
         "__name__": GsgkExtended.__tablename__,
         "__class__": GsgkExtended,
         "replace_column_names": {
             "EegMaStRNummer": "EegMastrNummer",
             "KwkMaStRNummer": "KwkMastrNummer",
             "LokationMaStRNummer": "LokationMastrNummer",
         },
@@ -954,14 +973,19 @@
         "__name__": CombustionExtended.__tablename__,
         "__class__": CombustionExtended,
         "replace_column_names": {
             "LokationMaStRNummer": "LokationMastrNummer",
             "KwkMaStRNummer": "KwkMastrNummer",
         },
     },
+    "ertuechtigungen": {
+        "__name__": RetrofitUnits.__tablename__,
+        "__class__": RetrofitUnits,
+        "replace_column_names": None,
+    },
     "geloeschteunddeaktivierteeinheiten": {
         "__name__": DeletedUnits.__tablename__,
         "__class__": DeletedUnits,
         "replace_column_names": None,
     },
     "marktrollen": {
         "__name__": MarketRoles.__tablename__,
```

### Comparing `open_mastr-0.13.0/open_mastr/xml_download/colums_to_replace.py` & `open_mastr-0.13.1/open_mastr/xml_download/colums_to_replace.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/open_mastr/xml_download/utils_cleansing_bulk.py` & `open_mastr-0.13.1/open_mastr/xml_download/utils_cleansing_bulk.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 def replace_mastr_katalogeintraege(
     zipped_xml_file_path: str,
     df: pd.DataFrame,
 ) -> pd.DataFrame:
     """Replaces the IDs from the mastr database by its mapped string values from
     the table katalogwerte"""
     katalogwerte = create_katalogwerte_from_bulk_download(zipped_xml_file_path)
-
     for column_name in df.columns:
         if column_name in columns_replace_list:
             if df[column_name].dtype == "O":
                 # Handle comma seperated strings from catalog values
                 df[column_name] = (
                     df[column_name]
                     .str.split(",", expand=True)
                     .apply(lambda x: x.str.strip())
+                    .replace("", None)
                     .astype("Int64")
                     .applymap(katalogwerte.get)
                     .agg(lambda d: ",".join(i for i in d if isinstance(i, str)), axis=1)
                     .replace("", None)
                 )
             else:
                 df[column_name] = (
```

### Comparing `open_mastr-0.13.0/open_mastr/xml_download/utils_download_bulk.py` & `open_mastr-0.13.1/open_mastr/xml_download/utils_download_bulk.py`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/open_mastr/xml_download/utils_write_to_database.py` & `open_mastr-0.13.1/open_mastr/xml_download/utils_write_to_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,17 +281,24 @@
     primary_key = next(c for c in table.columns if c.primary_key)
 
     with engine.connect() as con:
         with con.begin():
             key_list = (
                 pd.read_sql(sql=select(primary_key), con=con).values.squeeze().tolist()
             )
-    df = df.set_index(primary_key.name)
+
     len_df_before = len(df)
-    df = df.drop(labels=key_list, errors="ignore")
+    df = df.drop_duplicates(
+        subset=[primary_key.name]
+    )  # drop all entries with duplicated primary keys in the dataframe
+    df = df.set_index(primary_key.name)
+
+    df = df.drop(
+        labels=key_list, errors="ignore"
+    )  # drop primary keys that already exist in the table
     df = df.reset_index()
     print(f"{len_df_before-len(df)} entries already existed in the database.")
 
     return df
 
 
 def add_missing_column_to_table(
@@ -374,9 +381,7 @@
         if evaluated_string == "<":
             break
         else:
             decoded_data = decoded_data[:start_char] + decoded_data[start_char + 1 :]
     df = pd.read_xml(decoded_data)
     print("One invalid xml expression was deleted.")
     return df
-
-
```

### Comparing `open_mastr-0.13.0/open_mastr.egg-info/PKG-INFO` & `open_mastr-0.13.1/open_mastr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: open-mastr
-Version: 0.13.0
+Version: 0.13.1
 Summary: A package that provides an interface for downloading and processing the data of the Marktstammdatenregister (MaStR)
 Home-page: https://github.com/OpenEnergyPlatform/open-MaStR
-Download-URL: https://github.com/OpenEnergyPlatform/open-MaStR/archive/refs/tags/v0.13.0.tar.gz
+Download-URL: https://github.com/OpenEnergyPlatform/open-MaStR/archive/refs/tags/v0.13.1.tar.gz
 Author: Open Energy Family
 Author-email: datenzentrum@rl-institut.de
 Maintainer: Ludwig Hülk
 Maintainer-email: datenzentrum@rl-institut.de
 Project-URL: Documentation, https://open-mastr.readthedocs.io/
 Project-URL: Changelog, https://open-mastr.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/OpenEnergyPlatform/open-MaStR/issues
```

### Comparing `open_mastr-0.13.0/open_mastr.egg-info/SOURCES.txt` & `open_mastr-0.13.1/open_mastr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open_mastr-0.13.0/setup.py` & `open_mastr-0.13.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,22 @@
         "open_mastr",
         "open_mastr.soap_api",
         "open_mastr.soap_api.metadata",
         "open_mastr.utils",
         "open_mastr.utils.config",
         "open_mastr.xml_download",
     ],
-    version="0.13.0",
+    version="0.13.1",
     description="A package that provides an interface for downloading and"
     " processing the data of the Marktstammdatenregister (MaStR)",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/OpenEnergyPlatform/open-MaStR",
     download_url="https://github.com/OpenEnergyPlatform/open-MaStR/archive"
-    "/refs/tags/v0.13.0.tar.gz",
+    "/refs/tags/v0.13.1.tar.gz",
     author="Open Energy Family",
     author_email="datenzentrum@rl-institut.de",
     maintainer="Ludwig Hülk",
     maintainer_email="datenzentrum@rl-institut.de",
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `open_mastr-0.13.0/tests/test_helpers.py` & `open_mastr-0.13.1/tests/test_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,16 @@
             "storage",
             "electricity_consumer",
             "location",
             "market",
             "grid",
             "balancing_area",
             "permit",
+            "deleted_units",
+            "retrofit_units",
             None,
             ["wind", "solar"],
         ],
         "date": ["today", "20200108"],
         "bulk_cleansing": [True, False],
         "api_processes": [None],
         "api_limit": [50],
```

