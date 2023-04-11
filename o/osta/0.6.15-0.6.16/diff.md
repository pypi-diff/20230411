# Comparing `tmp/osta-0.6.15.tar.gz` & `tmp/osta-0.6.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osta-0.6.15.tar", last modified: Wed Apr  5 15:12:43 2023, max compression
+gzip compressed data, was "osta-0.6.16.tar", last modified: Tue Apr 11 16:03:25 2023, max compression
```

## Comparing `osta-0.6.15.tar` & `osta-0.6.16.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxr-x   0 tvborm    (1000) tvborm    (1000)        0 2023-04-05 15:12:43.495074 osta-0.6.15/
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     9073 2023-01-06 09:23:10.000000 osta-0.6.15/LICENSE
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     1350 2023-04-05 15:12:43.495074 osta-0.6.15/PKG-INFO
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)      808 2023-03-22 08:22:53.000000 osta-0.6.15/README.md
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)      994 2023-03-21 11:04:56.000000 osta-0.6.15/pyproject.toml
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)      793 2023-04-05 15:12:43.495074 osta-0.6.15/setup.cfg
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)      155 2023-01-19 13:04:57.000000 osta-0.6.15/setup.py
-drwxrwxr-x   0 tvborm    (1000) tvborm    (1000)        0 2023-04-05 15:12:43.495074 osta-0.6.15/src/
-drwxrwxr-x   0 tvborm    (1000) tvborm    (1000)        0 2023-04-05 15:12:43.495074 osta-0.6.15/src/osta/
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)      152 2023-03-22 08:22:53.000000 osta-0.6.15/src/osta/__init__.py
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    20794 2023-03-30 06:54:10.000000 osta-0.6.15/src/osta/__utils.py
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    46700 2023-04-05 14:53:04.000000 osta-0.6.15/src/osta/__utils_enrich.py
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    39051 2023-04-05 14:53:04.000000 osta-0.6.15/src/osta/__utils_imports.py
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    68646 2023-03-30 11:32:40.000000 osta-0.6.15/src/osta/__utils_wrangle.py
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    39426 2023-04-05 15:11:45.000000 osta-0.6.15/src/osta/enrich.py
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    21297 2023-04-05 14:53:04.000000 osta-0.6.15/src/osta/imports.py
-drwxrwxr-x   0 tvborm    (1000) tvborm    (1000)        0 2023-04-05 15:12:43.495074 osta-0.6.15/src/osta/resources/
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    95570 2023-03-21 08:31:14.000000 osta-0.6.15/src/osta/resources/data_account.csv
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    28842 2023-03-21 08:31:14.000000 osta-0.6.15/src/osta/resources/data_financial.csv
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    12969 2023-03-21 08:31:14.000000 osta-0.6.15/src/osta/resources/data_land.csv
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    38366 2023-03-30 06:54:10.000000 osta-0.6.15/src/osta/resources/data_municipality.csv
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)   239124 2023-03-21 08:31:14.000000 osta-0.6.15/src/osta/resources/data_service.csv
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     2541 2023-03-21 08:31:14.000000 osta-0.6.15/src/osta/resources/fields_mandatory.csv
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     2315 2023-03-21 08:31:14.000000 osta-0.6.15/src/osta/resources/fields_optional.csv
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)      283 2023-03-21 08:31:14.000000 osta-0.6.15/src/osta/resources/fields_pairs.csv
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     3313 2023-03-25 13:23:45.000000 osta-0.6.15/src/osta/resources.py
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    17725 2023-03-22 08:22:53.000000 osta-0.6.15/src/osta/wrangle.py
-drwxrwxr-x   0 tvborm    (1000) tvborm    (1000)        0 2023-04-05 15:12:43.495074 osta-0.6.15/src/osta.egg-info/
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     1350 2023-04-05 15:12:43.000000 osta-0.6.15/src/osta.egg-info/PKG-INFO
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)      823 2023-04-05 15:12:43.000000 osta-0.6.15/src/osta.egg-info/SOURCES.txt
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)        1 2023-04-05 15:12:43.000000 osta-0.6.15/src/osta.egg-info/dependency_links.txt
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)        1 2023-02-02 06:22:02.000000 osta-0.6.15/src/osta.egg-info/not-zip-safe
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)        5 2023-04-05 15:12:43.000000 osta-0.6.15/src/osta.egg-info/top_level.txt
-drwxrwxr-x   0 tvborm    (1000) tvborm    (1000)        0 2023-04-05 15:12:43.495074 osta-0.6.15/tests/
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    15436 2023-04-05 14:53:04.000000 osta-0.6.15/tests/test_enrich.py
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    19566 2023-03-24 14:29:58.000000 osta-0.6.15/tests/test_imports.py
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     3458 2023-03-25 13:23:45.000000 osta-0.6.15/tests/test_resources.py
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     3001 2023-03-21 08:31:14.000000 osta-0.6.15/tests/test_utils.py
--rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    31589 2023-03-25 13:23:45.000000 osta-0.6.15/tests/test_wrangle.py
+drwxrwxr-x   0 tvborm    (1000) tvborm    (1000)        0 2023-04-11 16:03:25.173960 osta-0.6.16/
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     9073 2023-01-06 09:23:10.000000 osta-0.6.16/LICENSE
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     4012 2023-04-11 16:03:25.173960 osta-0.6.16/PKG-INFO
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     3471 2023-04-11 15:47:30.000000 osta-0.6.16/README.md
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)      994 2023-03-21 11:04:56.000000 osta-0.6.16/pyproject.toml
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)      793 2023-04-11 16:03:25.173960 osta-0.6.16/setup.cfg
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)      155 2023-01-19 13:04:57.000000 osta-0.6.16/setup.py
+drwxrwxr-x   0 tvborm    (1000) tvborm    (1000)        0 2023-04-11 16:03:25.169960 osta-0.6.16/src/
+drwxrwxr-x   0 tvborm    (1000) tvborm    (1000)        0 2023-04-11 16:03:25.169960 osta-0.6.16/src/osta/
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     2596 2023-04-11 15:47:16.000000 osta-0.6.16/src/osta/__init__.py
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    20794 2023-03-30 06:54:10.000000 osta-0.6.16/src/osta/__utils.py
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    46837 2023-04-09 11:08:00.000000 osta-0.6.16/src/osta/__utils_enrich.py
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    39051 2023-04-05 14:53:04.000000 osta-0.6.16/src/osta/__utils_imports.py
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    74859 2023-04-11 16:00:50.000000 osta-0.6.16/src/osta/__utils_wrangle.py
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    39575 2023-04-09 12:13:47.000000 osta-0.6.16/src/osta/enrich.py
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    21297 2023-04-05 14:53:04.000000 osta-0.6.16/src/osta/imports.py
+drwxrwxr-x   0 tvborm    (1000) tvborm    (1000)        0 2023-04-11 16:03:25.173960 osta-0.6.16/src/osta/resources/
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    95570 2023-03-21 08:31:14.000000 osta-0.6.16/src/osta/resources/data_account.csv
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    28842 2023-03-21 08:31:14.000000 osta-0.6.16/src/osta/resources/data_financial.csv
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    12969 2023-03-21 08:31:14.000000 osta-0.6.16/src/osta/resources/data_land.csv
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    38366 2023-03-30 06:54:10.000000 osta-0.6.16/src/osta/resources/data_municipality.csv
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)   239124 2023-03-21 08:31:14.000000 osta-0.6.16/src/osta/resources/data_service.csv
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)      548 2023-04-09 16:17:52.000000 osta-0.6.16/src/osta/resources/fields_export.csv
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     2541 2023-03-21 08:31:14.000000 osta-0.6.16/src/osta/resources/fields_mandatory.csv
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     2315 2023-03-21 08:31:14.000000 osta-0.6.16/src/osta/resources/fields_optional.csv
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)      283 2023-03-21 08:31:14.000000 osta-0.6.16/src/osta/resources/fields_pairs.csv
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     3313 2023-03-25 13:23:45.000000 osta-0.6.16/src/osta/resources.py
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    22546 2023-04-11 15:59:47.000000 osta-0.6.16/src/osta/wrangle.py
+drwxrwxr-x   0 tvborm    (1000) tvborm    (1000)        0 2023-04-11 16:03:25.169960 osta-0.6.16/src/osta.egg-info/
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     4012 2023-04-11 16:03:25.000000 osta-0.6.16/src/osta.egg-info/PKG-INFO
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)      860 2023-04-11 16:03:25.000000 osta-0.6.16/src/osta.egg-info/SOURCES.txt
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)        1 2023-04-11 16:03:25.000000 osta-0.6.16/src/osta.egg-info/dependency_links.txt
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)        1 2023-02-02 06:22:02.000000 osta-0.6.16/src/osta.egg-info/not-zip-safe
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)        5 2023-04-11 16:03:25.000000 osta-0.6.16/src/osta.egg-info/top_level.txt
+drwxrwxr-x   0 tvborm    (1000) tvborm    (1000)        0 2023-04-11 16:03:25.173960 osta-0.6.16/tests/
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    15436 2023-04-05 14:53:04.000000 osta-0.6.16/tests/test_enrich.py
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    19566 2023-03-24 14:29:58.000000 osta-0.6.16/tests/test_imports.py
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     3458 2023-03-25 13:23:45.000000 osta-0.6.16/tests/test_resources.py
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)     3001 2023-03-21 08:31:14.000000 osta-0.6.16/tests/test_utils.py
+-rw-rw-r--   0 tvborm    (1000) tvborm    (1000)    40759 2023-04-11 16:02:57.000000 osta-0.6.16/tests/test_wrangle.py
```

### Comparing `osta-0.6.15/LICENSE` & `osta-0.6.16/LICENSE`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/pyproject.toml` & `osta-0.6.16/pyproject.toml`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/setup.cfg` & `osta-0.6.16/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = osta
 description = OSTolaskujen Analysointi -- package for analysing invoices of Finnish public organizations
-version = 0.6.15
+version = 0.6.16
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/TuomasBorman/osta
 author = Tuomas Borman
 author_email = tvborm@utu.fi
 license = Artistic License 2.0
 license_files = LICENSE
```

### Comparing `osta-0.6.15/src/osta/__utils.py` & `osta-0.6.16/src/osta/__utils.py`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/src/osta/__utils_enrich.py` & `osta-0.6.16/src/osta/__utils_enrich.py`

 * *Files 1% similar despite different names*

```diff
@@ -928,14 +928,16 @@
         values_num = int(len(values)/len(code))
         df_temp = pd.DataFrame()
         for i in range(0, len(values), values_num):
             # Split based on organization
             temp = pd.Series(values[i:i+values_num])
             temp = pd.DataFrame(temp).transpose()
             df_temp = pd.concat([df_temp, temp], axis=0)
+        # Convert values to numeric
+        df_temp = df_temp.apply(pd.to_numeric, errors="ignore")
         # Add label, municipality and year
         df_temp.columns = label
         df_temp["code"] = code
         df_temp["year"] = year
         # Add to results
         res = pd.concat([res, df_temp], axis=0)
     # Subset the data sp that it includes only wanted codes and years
@@ -1005,14 +1007,16 @@
     # Get ktpe data including only tax rate
     key_figs = df_key.loc[
         df_key["entrypoint"] == "KTPE", "tunnusluku"].tolist()
     df = __fetch_financial_data(
         df=df, df_info=df_info,
         datatype="KTPE", year=year, key_figs=key_figs,
         subset=True, language=language, **args)
+    # Add year
+    df["year"] = year
     # Reset index and return whole data
     df = df.reset_index(drop=True)
     return df
 
 
 def __fetch_financial_data(df, df_info,
                            datatype, year, key_figs,
```

### Comparing `osta-0.6.15/src/osta/__utils_imports.py` & `osta-0.6.16/src/osta/__utils_imports.py`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/src/osta/__utils_wrangle.py` & `osta-0.6.16/src/osta/__utils_wrangle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1627,7 +1627,186 @@
                 message=f"It seems that the data includes rows with up to "
                 f"{max_num} empty values. Please check them for errors. "
                 f"Rows with empty values printed below.\n"
                 f"{df.loc[empty_values>0,:]}",
                 category=Warning
                 )
     return df
+
+
+# organize
+
+def __subset_data(df, subset):
+    """
+    This function subset the data; takes only specific columns
+    Input: df
+    Output: df
+    """
+    if subset:
+        # Load fields from file
+        path = pkg_resources.resource_filename(
+            "osta", "resources/" + "fields_export.csv")
+        fields = pd.read_csv(path)
+        fields = fields["key"]
+        # Get those fields that are in DF
+        fields = [x for x in fields if x in df.columns]
+        # Subset the data
+        df = df.loc[:, fields]
+    return df
+
+
+def __rename_columns(df, rename):
+    """
+    This function rename columns
+    Input: df
+    Output: df
+    """
+    if rename:
+        # Load fields from file
+        path = pkg_resources.resource_filename(
+            "osta", "resources/" + "fields_export.csv")
+        fields = pd.read_csv(path)
+        # Create a dictionary from field data
+        fields = fields.set_index("key")["value"].to_dict()
+        # Rename columns
+        df = df.rename(columns=fields)
+    return df
+
+
+def __modify_account(
+        df, subset_account, add_account_group, language="fi", **args):
+    """
+    This function take only accounts 4300-4999.
+    Input: df
+    Output: df
+    """
+    # INPUT CHECK
+    if not (language == "fi" or language == "en"):
+        raise Exception(
+            "'language' must be 'fi' or 'en'."
+            )
+    # INPUT CHECK END
+    # Take only specific accounts
+    if subset_account and "account_code" in df.columns:
+        # Take index of rows that have account between 4300-4999
+        ind = df["account_code"].astype(str).isin(
+            [str(x) for x in range(4300, 5000)])
+        # Subset the data
+        df = df.loc[ind, :]
+    # Add account group
+    if subset_account and add_account_group and "account_code" in df.columns:
+        # Initialize column
+        column = "Kirjanpidon tiliryhmät" if language == "fi" else \
+            "Account groups"
+        df = df.reindex(columns=df.columns.tolist() + [column])
+        # Get account codes
+        accounts = pd.to_numeric(df["account_code"], errors="coerce")
+        # Create account group 1
+        ind = (accounts >= 4300) & (accounts <= 4499)
+        value = "Palvelujen ostot" if language == "fi" else "Services"
+        df.loc[ind, column] = value
+        # Create account group 2
+        ind = (accounts >= 4500) & (accounts <= 4699)
+        value = "Aineet, tarvikkeet ja tavarat" if language == "fi" else \
+            "Materials, supplies and goods"
+        df.loc[ind, column] = value
+        # Create account group 3
+        ind = (accounts >= 4700) & (accounts <= 4799)
+        value = "Avustukset" if language == "fi" else "Allowances"
+        df.loc[ind, column] = value
+        # Create account group 4
+        ind = (accounts >= 4800) & (accounts <= 4999)
+        value = "Muut toimintakulut" if language == "fi" else \
+            "Other operating expenses"
+        df.loc[ind, column] = value
+    return df
+
+
+def __convert_foreign_bid(
+        df, drop_foreign_bid, foreign_bid="0000000-1", land_col=None, **args):
+    """
+    This function replace foreign bids.
+    Input: df
+    Output: df
+    """
+    # INPUT CHECK
+    if not isinstance(foreign_bid, str):
+        raise Exception(
+            "'foreign_bid' must be a string."
+            )
+    if not (land_col is None or (
+            isinstance(land_col, str) and land_col in df.columns)):
+        raise Exception(
+            "'land_col' must be None or string specifying a column."
+            )
+    # INPUT CHECK END
+    # Get correct column
+    if land_col is None:
+        column = "suppl_land"
+    else:
+        column = land_col
+    # If specified and column is found
+    if (drop_foreign_bid and column in df.columns and
+            "suppl_bid" in df.columns):
+        # Load land codes from file
+        path = pkg_resources.resource_filename(
+            "osta", "resources/" + "data_land.csv")
+        land = pd.read_csv(path, index_col=0, dtype="str")
+        # Taken only those lands that are not Finnish
+        land = land.loc[land["code_2char"] != "FI", :]
+        # Get index of those values that are other that Finnish
+        ind = land.apply(
+            lambda x: df[column].astype(str).isin(x)).sum(axis=1) > 0
+        # Replace those business IDs that are from foreign companies
+        df.loc[ind, "suppl_bid"] = foreign_bid
+    return df
+
+
+def __drop_private_entrepreneur(
+        df, drop_private, private_bid="0000000-0", language="fi",
+        form_col=None, **args):
+    """
+    This function drops off sensitive data of private entrepreneurs.
+    Input: df
+    Output: df
+    """
+    # INPUT CHECK
+    if not isinstance(private_bid, str):
+        raise Exception(
+            "'private_bid' must be a string."
+            )
+    if not (language == "fi" or language == "en"):
+        raise Exception(
+            "'language' must be 'fi' or 'en'."
+            )
+    if not (form_col is None or (
+            isinstance(form_col, str) and form_col in df.columns)):
+        raise Exception(
+            "'form_col' must be None or string specifying a column."
+            )
+    # INPUT CHECK END
+    private_name = "Yksityinen elinkeinonharjoittaja" if language == "fi" \
+        else "Private person carrying on trade"
+    # Check if correct column is available
+    if form_col is None:
+        column = ["suppl_yhtiömuoto", "suppl_company form",
+                  "suppl_företagsform"]
+    else:
+        column = [form_col]
+    column = [x for x in column if x in df.columns]
+    # If there are column that tells the company form
+    if drop_private and len(column) == 1:
+        # List certain company type in different languages
+        comp_type = [
+            "yksityinen elinkeinonharjoittaja",
+            "private person carrying on trade",
+            "enskild näringsidkare"
+            ]
+        # Search those companies from the data
+        ind = df[column[0]].astype(str).str.lower().isin(comp_type)
+        # Change name if available
+        if "suppl_name" in df.columns:
+            df.loc[ind, "suppl_name"] = private_name
+        # Change bid if available
+        if "suppl_bid" in df.columns:
+            df.loc[ind, "suppl_bid"] = private_bid
+    return df
```

### Comparing `osta-0.6.15/src/osta/enrich.py` & `osta-0.6.16/src/osta/enrich.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,14 +310,17 @@
         bid_cols = df.loc[:, ind]
         bid_col = bid_cols.apply(lambda x: ', '.join(x.dropna(
             ).astype(str)), axis=1)
         # Remove additional BID columns, keep only one
         ind = [False if regex.search(x) else True for x in df.columns]
         df = df.loc[:, ind]
         df["old_bid"] = bid_col
+    # Capitalize municipality (some might be in uppercase)
+    if "muni" in df.columns:
+        df["muni"] = df["muni"].astype(str).str.capitalize()
     # Convert column names into right language if Finnish or Swedish
     if language == "fi":
         columns = {
             "registration_date": "rekisteröintipäivä",
             "company_form_short": "yhtiömuoto_lyhyt",
             "liquidation": "konkurssitiedot",
             "company_form": "yhtiömuoto",
```

### Comparing `osta-0.6.15/src/osta/imports.py` & `osta-0.6.16/src/osta/imports.py`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/src/osta/resources/data_account.csv` & `osta-0.6.16/src/osta/resources/data_account.csv`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/src/osta/resources/data_financial.csv` & `osta-0.6.16/src/osta/resources/data_financial.csv`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/src/osta/resources/data_land.csv` & `osta-0.6.16/src/osta/resources/data_land.csv`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/src/osta/resources/data_municipality.csv` & `osta-0.6.16/src/osta/resources/data_municipality.csv`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/src/osta/resources/data_service.csv` & `osta-0.6.16/src/osta/resources/data_service.csv`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/src/osta/resources/fields_mandatory.csv` & `osta-0.6.16/src/osta/resources/fields_mandatory.csv`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/src/osta/resources/fields_optional.csv` & `osta-0.6.16/src/osta/resources/fields_optional.csv`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/src/osta/resources.py` & `osta-0.6.16/src/osta/resources.py`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/src/osta/wrangle.py` & `osta-0.6.16/src/osta/wrangle.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 # -*- coding: utf-8 -*-
 import osta.__utils as utils
 import pandas as pd
 import warnings
 from os import listdir
 from os.path import isfile, isdir, join
 import sys
-from osta.__utils_wrangle import clean_data
+from osta.__utils_wrangle import clean_data, __subset_data, \
+    __rename_columns, __convert_foreign_bid, __drop_private_entrepreneur, \
+    __modify_account
 
 
 def clean(df_list, save_dir=None, log_file=False, verbose=True, **args):
     """
     Standardize data
 
     This function standardize the data that is in pandas.DataFrame. The
@@ -423,7 +425,127 @@
     # Save file if specified
     if save_file is not None:
         df.to_csv(save_file, index=False)
     # Reset logging; do not capture warnings anymore
     if log_file:
         utils.__stop_logging(logger)
     return df
+
+
+def organize(
+        df, subset=True, rename=True, drop_foreign_bid=True,
+        drop_private=True, subset_account=True, add_account_group=True,
+        **args):
+    """
+    This function clean the data for export.
+
+    Arguments:
+        `df`: A pandas.DataFrame.
+
+        `subset`: A boolean value for selecting whether to subset the data
+        taking only certain columns. These columns include fields that
+        are suggested to be published by Association of Finnish municipalities.
+        (By default: subset=True)
+
+        `rename`: A boolean value for selecting whether to rename the columns
+        based on suggestion of Association of Finnish municipalities.
+        (By default: rename=True)
+
+        `drop_foreign_bid`: A boolean value for selecting whether to remove
+        business IDs of foreign companies. The land of supplier is detected
+        based on 'suppl_land' column by default. See land_col argument.
+        (By default: drop_foreign_bid=True)
+
+        `drop_private`: A boolean value for selecting whether to remove name
+        and business ID of private person carrying a trade. The company format
+        is detected based on 'suppl_yhtiömuoto', 'suppl_form_col', or
+        'suppl_företagsform' columns by default. Check form_col argument.
+        (By default: drop_private=True)
+
+        `subset_account`: A boolean value for selecting whether to keep only
+        rows with account codes from 4300 to 4999.
+        (By default: subset_account=True)
+
+        `add_account_group`: A boolean value for selecting whether to add
+        account group information. (By default: add_account_group=True)
+
+        `**args`: Additional arguments passes into other functions:
+
+        `foreign_bid`: A string specifying business ID that is used to replace
+        business IDs of foreign companies.
+        (By default: foreign_bid="0000000-1")
+
+        `private_bid`: A string specifying business ID that is used to replace
+        business IDs of private people carrying a trade.
+        (By default: private_bid="0000000-0")
+
+        `language`: A string specifying a language. Must be 'fi' (Finnish) or
+        'en' (English). (By default: language="fi")
+
+        `drop_foreign_bid`: A string specifying a column. This column is used to
+        check company form of supplier. If None, default choice is used.
+        (By default: form_col=None)
+
+        `land_col`: A string specifying a column. This column is used to
+        check land of supplier. If None, default choice is used.
+        (By default: land_col=None)
+
+    Details:
+        This function is used to clean the data for export. The cleaning
+        follows suggestions of Association of Finnish municipalities. In
+        subsetting, only the columns containing mandatory and optional fields
+        are kept. Additional information that is not mentioned in the
+        association's guide is removed. The columns can also be renamed so
+        that they follow the guide.
+
+        For sensitive data concerning private person carrying a trade,
+        there is functionality that drops them off. Moreover, foreign
+        business IDs can be removed. For account data, the method includes
+        functionality that keeps only certain accounts of income statement.
+        The code of these accounts are from 4300 to 4999.
+
+    Examples:
+        ```
+        df = organize(df)
+
+        ```
+
+    Output:
+        A pandas.DataFrame
+
+    """
+    # INPUT CHECK
+    if not utils.__is_non_empty_df(df):
+        raise Exception(
+            "'df' must be non-empty pandas.DataFrame."
+            )
+    if not isinstance(subset, bool):
+        raise Exception(
+            "'subset' must be True or False."
+            )
+    if not isinstance(rename, bool):
+        raise Exception(
+            "'rename' must be True or False."
+            )
+    if not isinstance(drop_foreign_bid, bool):
+        raise Exception(
+            "'drop_foreign_bid' must be True or False."
+            )
+    if not isinstance(drop_private, bool):
+        raise Exception(
+            "'drop_private' must be True or False."
+            )
+    if not isinstance(subset_account, bool):
+        raise Exception(
+            "'subset_account' must be True or False."
+            )
+    if not isinstance(add_account_group, bool):
+        raise Exception(
+            "'add_account_group' must be True or False."
+            )
+    # INPUT CHECK END
+    df = __convert_foreign_bid(df, drop_foreign_bid, **args)
+    df = __drop_private_entrepreneur(df, drop_private, **args)
+    df = __subset_data(df, subset)
+    df = __modify_account(df, subset_account, add_account_group, **args)
+    df = __rename_columns(df, rename)
+    return df
```

### Comparing `osta-0.6.15/src/osta.egg-info/SOURCES.txt` & `osta-0.6.16/src/osta.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/osta.egg-info/not-zip-safe
 src/osta.egg-info/top_level.txt
 src/osta/resources/data_account.csv
 src/osta/resources/data_financial.csv
 src/osta/resources/data_land.csv
 src/osta/resources/data_municipality.csv
 src/osta/resources/data_service.csv
+src/osta/resources/fields_export.csv
 src/osta/resources/fields_mandatory.csv
 src/osta/resources/fields_optional.csv
 src/osta/resources/fields_pairs.csv
 tests/test_enrich.py
 tests/test_imports.py
 tests/test_resources.py
 tests/test_utils.py
```

### Comparing `osta-0.6.15/tests/test_enrich.py` & `osta-0.6.16/tests/test_enrich.py`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/tests/test_imports.py` & `osta-0.6.16/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/tests/test_resources.py` & `osta-0.6.16/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/tests/test_utils.py` & `osta-0.6.16/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osta-0.6.15/tests/test_wrangle.py` & `osta-0.6.16/tests/test_wrangle.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
-from osta.wrangle import clean, merge
+from osta.wrangle import clean, merge, organize
 import pandas as pd
 import pytest
-from pandas.testing import assert_frame_equal
+from pandas.testing import assert_frame_equal, assert_series_equal
 import pkg_resources
 
 
 def test_check_names_wrong_arguments():
     df = __create_dummy_data()
     # Some tests give warnings...
     with pytest.warns(Warning):
@@ -623,15 +623,14 @@
     df = pd.DataFrame(data)
     df = clean(df, date_format="%Y/%d/%m")
     # Expected names
     data = {"doc_date": ["2013/01/12", "2012/31/12", "2012/20/02"],
             "test": ["0135202-4", "0135202-4", "test"]
             }
     df_expect = pd.DataFrame(data)
-    print(df)
     # Expect that are equal
     assert_frame_equal(df, df_expect)
 
     data = {"doc_date": ["01122013", "3122012", "200212"],
             "test": ["0135202-4", "0135202-4", "test"]
             }
     df = pd.DataFrame(data)
@@ -875,7 +874,251 @@
             }
     df2 = pd.DataFrame(data)
     with pytest.warns(Warning):
         res = merge([df, df2])
     assert res.shape[0] == 6 and res.shape[1] == 3
     df_expect = pd.concat([df, df2]).reset_index(drop=True)
     assert_frame_equal(res, df_expect)
+
+
+# organize
+
+def test_organize_wrong_arguments():
+    df = __create_dummy_data()
+    with pytest.raises(Exception):
+        df = organize()
+    with pytest.raises(Exception):
+        df = organize(pd.DataFrame())
+    with pytest.raises(Exception):
+        df = organize(None)
+    with pytest.raises(Exception):
+        df = organize(1)
+    with pytest.raises(Exception):
+        df = organize(True)
+    with pytest.raises(Exception):
+        df = organize("yes")
+    with pytest.raises(Exception):
+        df = organize(df, subset="yes")
+    with pytest.raises(Exception):
+        df = organize(df, subset=1)
+    with pytest.raises(Exception):
+        df = organize(df, subset=None)
+    with pytest.raises(Exception):
+        df = organize(df, subset=[True, True])
+    with pytest.raises(Exception):
+        df = organize(df, rename="yes")
+    with pytest.raises(Exception):
+        df = organize(df, rename=1)
+    with pytest.raises(Exception):
+        df = organize(df, rename=None)
+    with pytest.raises(Exception):
+        df = organize(df, rename=[True, True])
+    with pytest.raises(Exception):
+        df = organize(df, drop_foreign_bid="yes")
+    with pytest.raises(Exception):
+        df = organize(df, drop_foreign_bid=1)
+    with pytest.raises(Exception):
+        df = organize(df, drop_foreign_bid=None)
+    with pytest.raises(Exception):
+        df = organize(df, drop_foreign_bid=[True, True])
+    with pytest.raises(Exception):
+        df = organize(df, drop_private="yes")
+    with pytest.raises(Exception):
+        df = organize(df, drop_private=1)
+    with pytest.raises(Exception):
+        df = organize(df, drop_private=None)
+    with pytest.raises(Exception):
+        df = organize(df, drop_private=[True, True])
+    with pytest.raises(Exception):
+        df = organize(df, subset_account="yes")
+    with pytest.raises(Exception):
+        df = organize(df, subset_account=1)
+    with pytest.raises(Exception):
+        df = organize(df, subset_account=None)
+    with pytest.raises(Exception):
+        df = organize(df, subset_account=[True, True])
+    with pytest.raises(Exception):
+        df = organize(df, add_account_group="yes")
+    with pytest.raises(Exception):
+        df = organize(df, add_account_group=1)
+    with pytest.raises(Exception):
+        df = organize(df, add_account_group=None)
+    with pytest.raises(Exception):
+        df = organize(df, add_account_group=[True, True])
+    with pytest.raises(Exception):
+        df = organize(df, foreign_bid=True)
+    with pytest.raises(Exception):
+        df = organize(df, foreign_bid=1)
+    with pytest.raises(Exception):
+        df = organize(df, foreign_bid=None)
+    with pytest.raises(Exception):
+        df = organize(df, foreign_bid=["True", "True"])
+    with pytest.raises(Exception):
+        df = organize(df, private_bid=True)
+    with pytest.raises(Exception):
+        df = organize(df, private_bid=1)
+    with pytest.raises(Exception):
+        df = organize(df, private_bid=None)
+    with pytest.raises(Exception):
+        df = organize(df, private_bid=["True", "True"])
+    with pytest.raises(Exception):
+        df = organize(df, language=True)
+    with pytest.raises(Exception):
+        df = organize(df, language="yes")
+    with pytest.raises(Exception):
+        df = organize(df, language=1)
+    with pytest.raises(Exception):
+        df = organize(df, language=None)
+    with pytest.raises(Exception):
+        df = organize(df, language=["True", "True"])
+    with pytest.raises(Exception):
+        df = organize(df, form_col=True)
+    with pytest.raises(Exception):
+        df = organize(df, form_col="yes")
+    with pytest.raises(Exception):
+        df = organize(df, form_col=1)
+    with pytest.raises(Exception):
+        df = organize(df, form_col=["True", "True"])
+    with pytest.raises(Exception):
+        df = organize(df, land_col=True)
+    with pytest.raises(Exception):
+        df = organize(df, land_col="yes")
+    with pytest.raises(Exception):
+        df = organize(df, land_col=1)
+    with pytest.raises(Exception):
+        df = organize(df, land_col=["True", "True"])
+
+
+def test_organize():
+    # Test that subsetting and renaming works
+    df = __create_dummy_data2()
+    columns = df.columns
+    df = organize(df, subset=False, rename=False)
+    columns = [x in df.columns for x in columns]
+    assert all(columns)
+
+    df = __create_dummy_data2()
+    columns = [
+        "Kunnan tai kuntayhtymän nimi",
+        "Kuntanumero",
+        "Kunnan y-tunnus",
+        "Tositenumero",
+        "Tositepäivämäärä",
+        "Toimittajan nimi",
+        "Toimittajan y-tunnus",
+        "Toimittajan maakoodi",
+        "Kokonaissumma euroina",
+        "Palveluluokka",
+        "VAT-tunnus",
+        "Tilin nimi",
+        "Kirjanpidon tilinumero",
+        "Kirjanpidon tiliryhmät"
+        ]
+    df = organize(df)
+    print(df.columns)
+    columns = [x in columns for x in df.columns]
+    assert all(columns)
+
+    # Test that drop foreign BIDs works
+    df = __create_dummy_data2()
+    df = organize(df, rename=False)
+    exp = pd.Series(["0000000-0", "testi", "0000000-1"])
+    assert_series_equal(df["suppl_bid"], exp, check_names=False)
+
+    df = __create_dummy_data2()
+    df = organize(df, rename=False, foreign_bid="ulkomainen")
+    exp = pd.Series(["0000000-0", "testi", "ulkomainen"])
+    assert_series_equal(df["suppl_bid"], exp, check_names=False)
+
+    df = __create_dummy_data2()
+    df = organize(df, rename=False, drop_foreign_bid=False)
+    exp = pd.Series(["0000000-0", "testi", "test"])
+    assert_series_equal(df["suppl_bid"], exp, check_names=False)
+
+    df = __create_dummy_data2()
+    df = organize(df, rename=False, land_col="suppl_land")
+    exp = pd.Series(["0000000-0", "testi", "0000000-1"])
+    assert_series_equal(df["suppl_bid"], exp, check_names=False)
+
+    # Test that drop private info works
+    df = __create_dummy_data2()
+    df = organize(df, rename=False, subset=False)
+    exp = pd.Series(["0000000-0", "testi", "0000000-1"])
+    assert_series_equal(df["suppl_bid"], exp, check_names=False)
+    exp = pd.Series([
+        "Yksityinen elinkeinonharjoittaja", "testi", "test"])
+    assert_series_equal(df["suppl_name"], exp, check_names=False)
+
+    df = __create_dummy_data2()
+    df = organize(
+        df, rename=False, private_bid="yksityinen y-tunnus")
+    exp = pd.Series(["yksityinen y-tunnus", "testi", "0000000-1"])
+    assert_series_equal(df["suppl_bid"], exp, check_names=False)
+
+    df = __create_dummy_data2()
+    df = organize(df, rename=False, drop_private=False)
+    exp = pd.Series(["test", "testi", "0000000-1"])
+    assert_series_equal(df["suppl_bid"], exp, check_names=False)
+    exp = pd.Series(["test", "testi", "test"])
+    assert_series_equal(df["suppl_name"], exp, check_names=False)
+
+    df = __create_dummy_data2()
+    df = organize(df, rename=False, subset=False, form_col="suppl_yhtiömuoto")
+    exp = pd.Series(["0000000-0", "testi", "0000000-1"])
+    assert_series_equal(df["suppl_bid"], exp, check_names=False)
+    exp = pd.Series([
+        "Yksityinen elinkeinonharjoittaja", "testi", "test"])
+    assert_series_equal(df["suppl_name"], exp, check_names=False)
+
+    # Test that account manipulation works
+    df = __create_dummy_data2()
+    df = organize(df, subset_account=False)
+    assert df.shape[0] == 4
+
+    df = __create_dummy_data2()
+    df = organize(df)
+    assert df.shape[0] == 3
+
+    df = __create_dummy_data2()
+    df = organize(df, add_account_group=False)
+    assert "Kirjanpidon tiliryhmät" not in df.columns
+
+    df = __create_dummy_data2()
+    df = organize(df)
+    exp = pd.Series([
+        "Palvelujen ostot", "Aineet, tarvikkeet ja tavarat",
+        "Muut toimintakulut"])
+    assert_series_equal(df["Kirjanpidon tiliryhmät"], exp, check_names=False)
+
+    # Test that language works
+    df = __create_dummy_data2()
+    df = organize(df, language="en", rename=False)
+    exp = pd.Series([
+        "Services", "Materials, supplies and goods",
+        "Other operating expenses"])
+    assert_series_equal(df["Account groups"], exp, check_names=False)
+    exp = pd.Series([
+        "Private person carrying on trade", "testi", "test"])
+    assert_series_equal(df["suppl_name"], exp, check_names=False)
+    return df
+
+
+def __create_dummy_data2():
+    data = {"org_name": ["test", "testi", "test", "test"],
+            "org_code": [1, 2, 3, 3],
+            "org_bid": ["test", "testi", "test", "test"],
+            "suppl_bid": ["test", "testi", "test", "test"],
+            "doc_date": ["02.04.2023", "02.10.2023", "23.06.2022", "123"],
+            "suppl_name": ["test", "testi", "test", "testilainen"],
+            "suppl_yhtiömuoto": [
+                "Yksityinen elinkeinonharjoittaja", "testi", "test",
+                "testilainen"],
+            "price_total": [1.10, 2.04, 3.74, 4],
+            "test3": [True, False, False, True],
+            "doc_id": [1, 2, 3, 4],
+            "account_code": [4400, 4567, 4999, 5000],
+            "service_code": [123, 123, 123, 123],
+            "suppl_vat_number": ["test", "testi", "test", "test"],
+            "suppl_land": ["Suomi", "FIN", "DE", "FI"],
+            }
+    df = pd.DataFrame(data)
+    return df
```

