# Comparing `tmp/pheno-utils-0.0.7.tar.gz` & `tmp/pheno-utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.0.7.tar", last modified: Mon Apr 10 21:18:41 2023, max compression
+gzip compressed data, was "pheno-utils-0.0.8.tar", last modified: Tue Apr 11 12:31:04 2023, max compression
```

## Comparing `pheno-utils-0.0.7.tar` & `pheno-utils-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-10 21:18:41.337829 pheno-utils-0.0.7/
--rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.0.7/LICENSE
--rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.0.7/MANIFEST.in
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-10 21:18:41.337496 pheno-utils-0.0.7/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.0.7/README.md
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-10 21:18:41.334323 pheno-utils-0.0.7/pheno_utils/
--rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/__init__.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     8743 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/_modidx.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/age_reference_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2333 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/basic_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2740 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/config.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    12417 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/data_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-10 20:10:59.000000 pheno-utils-0.0.7/pheno_utils/dates_plots.py
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-10 21:18:41.337077 pheno-utils-0.0.7/pheno_utils.egg-info/
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-10 21:18:41.000000 pheno-utils-0.0.7/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      515 2023-04-10 21:18:41.000000 pheno-utils-0.0.7/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-10 21:18:41.000000 pheno-utils-0.0.7/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-10 21:18:41.000000 pheno-utils-0.0.7/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.0.7/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 alondmnt   (501) staff       (20)       99 2023-04-10 21:18:41.000000 pheno-utils-0.0.7/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-10 21:18:41.000000 pheno-utils-0.0.7/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)     1040 2023-04-10 20:10:51.000000 pheno-utils-0.0.7/settings.ini
--rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-10 21:18:41.337969 pheno-utils-0.0.7/setup.cfg
--rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.0.7/setup.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-11 12:31:04.813919 pheno-utils-0.0.8/
+-rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.0.8/LICENSE
+-rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.0.8/MANIFEST.in
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-11 12:31:04.813310 pheno-utils-0.0.8/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.0.8/README.md
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-11 12:31:04.809364 pheno-utils-0.0.8/pheno_utils/
+-rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/__init__.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     8743 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/_modidx.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2333 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/basic_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2740 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/config.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    12655 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/data_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-11 12:26:24.000000 pheno-utils-0.0.8/pheno_utils/dates_plots.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-11 12:31:04.812771 pheno-utils-0.0.8/pheno_utils.egg-info/
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-11 12:31:04.000000 pheno-utils-0.0.8/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      515 2023-04-11 12:31:04.000000 pheno-utils-0.0.8/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-11 12:31:04.000000 pheno-utils-0.0.8/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-11 12:31:04.000000 pheno-utils-0.0.8/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.0.8/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 alondmnt   (501) staff       (20)       99 2023-04-11 12:31:04.000000 pheno-utils-0.0.8/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-11 12:31:04.000000 pheno-utils-0.0.8/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1040 2023-04-11 12:25:58.000000 pheno-utils-0.0.8/settings.ini
+-rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-11 12:31:04.814034 pheno-utils-0.0.8/setup.cfg
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.0.8/setup.py
```

### Comparing `pheno-utils-0.0.7/LICENSE` & `pheno-utils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.7/PKG-INFO` & `pheno-utils-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.0.7/pheno_utils/_modidx.py` & `pheno-utils-0.0.8/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.7/pheno_utils/age_reference_plots.py` & `pheno-utils-0.0.8/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.7/pheno_utils/basic_plots.py` & `pheno-utils-0.0.8/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.7/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.0.8/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.7/pheno_utils/config.py` & `pheno-utils-0.0.8/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.7/pheno_utils/data_loader.py` & `pheno-utils-0.0.8/pheno_utils/data_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,34 +209,39 @@
         age_path = os.path.join(
             self.base_path,
             self.age_sex_dataset,
             self.cohort,
             'events.parquet')
         align_df = self.dfs[list(self.dfs)[0]]
 
-        # TODO: check if research stage is "continuous"
         if ('research_stage' in align_df.columns) or ('research_stage' in align_df.index.names):
             age_df = pd.read_parquet(age_path)
             self.dfs['age_sex'] = align_df.join(
                 age_df[['age_at_research_stage', 'sex']].droplevel('array_index'))\
                 .rename(columns={'age_at_research_stage': 'age'})
-            self.fields += ['age', 'sex']
+        else:
+            # init an empty df
+            self.dfs['age_sex'] = pd.DataFrame(index=align_df.index).assign(age=np.nan, sex=np.nan)
+
+        self.fields += ['age', 'sex']
+        ind = self.dfs['age_sex'].isnull().any(axis=1)
+        if ind.sum() == 0:  # no missing values
             return
 
+        # fill in missing values by computing age from birth date
         date_cols = np.array(['collection_timestamp', 'collection_date', 'sequencing_date'])
         date = date_cols[np.isin(date_cols, align_df.columns)][0]  # prefer first match
 
         age_df = pd.read_parquet(age_path.replace('events', 'population'))
         age_df['birth_date'] = pd.to_datetime(
             age_df['year_of_birth'].astype(str) + '-' + age_df['month_of_birth'].astype(str))
 
-        self.dfs['age_sex'] = align_df[[date]].join(age_df[['sex', 'birth_date']])\
+        self.dfs['age_sex'].loc[ind, :] = align_df.loc[ind, [date]].join(age_df[['sex', 'birth_date']])\
             .assign(age=lambda x: ((x[date].dt.date - x['birth_date'].dt.date).dt.days / 365.25).round(1))\
             .drop(columns=['birth_date'])
-        self.fields += ['age', 'sex']
 
     def __load_dataframes__(self) -> None:
         """
         Load all tables in the dataset dictionary.
         """
         self.dfs = {}
         self.fields = set()
```

### Comparing `pheno-utils-0.0.7/pheno_utils/dates_plots.py` & `pheno-utils-0.0.8/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.7/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.0.8/pheno_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.0.7/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.0.8/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.7/settings.ini` & `pheno-utils-0.0.8/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.0.7
+version = 0.0.8
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
```

### Comparing `pheno-utils-0.0.7/setup.py` & `pheno-utils-0.0.8/setup.py`

 * *Files identical despite different names*

