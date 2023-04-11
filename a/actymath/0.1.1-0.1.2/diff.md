# Comparing `tmp/actymath-0.1.1.tar.gz` & `tmp/actymath-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actymath-0.1.1.tar", max compression
+gzip compressed data, was "actymath-0.1.2.tar", max compression
```

## Comparing `actymath-0.1.1.tar` & `actymath-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1062 2021-05-04 15:05:39.583555 actymath-0.1.1/LICENSE
--rw-r--r--   0        0        0     2111 2021-05-04 15:43:34.438481 actymath-0.1.1/README.md
--rw-r--r--   0        0        0       84 2021-05-04 15:05:39.583846 actymath-0.1.1/actymath/__init__.py
--rw-r--r--   0        0        0     3205 2021-05-04 15:05:39.584029 actymath-0.1.1/actymath/calc.py
--rw-r--r--   0        0        0      457 2021-05-04 15:05:39.584227 actymath-0.1.1/actymath/columns/__init__.py
--rw-r--r--   0        0        0     2832 2021-05-04 15:05:39.584363 actymath-0.1.1/actymath/columns/base.py
--rw-r--r--   0        0        0     2074 2021-05-04 15:05:39.584500 actymath-0.1.1/actymath/columns/commutation.py
--rw-r--r--   0        0        0      545 2021-05-04 15:05:39.584646 actymath-0.1.1/actymath/columns/interest_rates.py
--rw-r--r--   0        0        0     2746 2021-05-04 15:05:39.584789 actymath-0.1.1/actymath/columns/mortality.py
--rw-r--r--   0        0        0     7087 2021-05-04 15:05:39.584924 actymath-0.1.1/actymath/columns/term.py
--rw-r--r--   0        0        0      689 2021-05-04 15:05:39.585035 actymath-0.1.1/actymath/columns/timeline.py
--rw-r--r--   0        0        0     2689 2021-05-04 15:05:39.585161 actymath-0.1.1/actymath/columns/whole_of_life.py
--rw-r--r--   0        0        0       41 2021-05-04 15:05:39.585257 actymath-0.1.1/actymath/exceptions.py
--rw-r--r--   0        0        0     1393 2021-05-04 15:05:39.585371 actymath-0.1.1/actymath/indexers.py
--rw-r--r--   0        0        0     3625 2021-05-04 15:05:39.585577 actymath-0.1.1/actymath/table_data/a1967-70.csv
--rw-r--r--   0        0        0     3094 2021-05-04 15:05:39.585713 actymath-0.1.1/actymath/table_data/a1967-70_exam.csv
--rw-r--r--   0        0        0     2710 2021-05-04 15:05:39.585857 actymath-0.1.1/actymath/table_data/amc00.csv
--rw-r--r--   0        0        0     1279 2021-05-04 15:05:39.585998 actymath-0.1.1/actymath/table_data/test.csv
--rw-r--r--   0        0        0       88 2021-05-04 15:05:39.586111 actymath-0.1.1/actymath/table_data/test_lx.csv
--rw-r--r--   0        0        0     6687 2021-05-04 15:05:39.586277 actymath-0.1.1/actymath/tables.py
--rw-r--r--   0        0        0      731 2021-05-04 15:58:36.693773 actymath-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2955 2021-05-04 15:58:39.366675 actymath-0.1.1/setup.py
--rw-r--r--   0        0        0     2818 2021-05-04 15:58:39.366913 actymath-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-11 17:09:38.439250 actymath-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2155 2023-04-11 17:09:38.439385 actymath-0.1.2/README.md
+-rw-r--r--   0        0        0       84 2023-04-11 17:09:38.439539 actymath-0.1.2/actymath/__init__.py
+-rw-r--r--   0        0        0     3205 2023-04-11 17:09:38.439669 actymath-0.1.2/actymath/calc.py
+-rw-r--r--   0        0        0      457 2023-04-11 17:09:38.439845 actymath-0.1.2/actymath/columns/__init__.py
+-rw-r--r--   0        0        0     2832 2023-04-11 17:09:38.439973 actymath-0.1.2/actymath/columns/base.py
+-rw-r--r--   0        0        0     2074 2023-04-11 17:09:38.440089 actymath-0.1.2/actymath/columns/commutation.py
+-rw-r--r--   0        0        0      545 2023-04-11 17:09:38.440193 actymath-0.1.2/actymath/columns/interest_rates.py
+-rw-r--r--   0        0        0     2746 2023-04-11 17:09:38.440314 actymath-0.1.2/actymath/columns/mortality.py
+-rw-r--r--   0        0        0     7087 2023-04-11 17:09:38.440423 actymath-0.1.2/actymath/columns/term.py
+-rw-r--r--   0        0        0      689 2023-04-11 17:09:38.440523 actymath-0.1.2/actymath/columns/timeline.py
+-rw-r--r--   0        0        0     2689 2023-04-11 17:09:38.440663 actymath-0.1.2/actymath/columns/whole_of_life.py
+-rw-r--r--   0        0        0       41 2023-04-11 17:09:38.440775 actymath-0.1.2/actymath/exceptions.py
+-rw-r--r--   0        0        0     1399 2023-04-11 17:33:48.998331 actymath-0.1.2/actymath/indexers.py
+-rw-r--r--   0        0        0     3625 2023-04-11 17:09:38.441087 actymath-0.1.2/actymath/table_data/a1967-70.csv
+-rw-r--r--   0        0        0     3094 2023-04-11 17:09:38.441220 actymath-0.1.2/actymath/table_data/a1967-70_exam.csv
+-rw-r--r--   0        0        0     2710 2023-04-11 17:09:38.441335 actymath-0.1.2/actymath/table_data/amc00.csv
+-rw-r--r--   0        0        0     1279 2023-04-11 17:09:38.441452 actymath-0.1.2/actymath/table_data/test.csv
+-rw-r--r--   0        0        0       88 2023-04-11 17:09:38.441551 actymath-0.1.2/actymath/table_data/test_lx.csv
+-rw-r--r--   0        0        0     6687 2023-04-11 17:09:38.441763 actymath-0.1.2/actymath/tables.py
+-rw-r--r--   0        0        0      751 2023-04-11 17:33:54.189540 actymath-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 actymath-0.1.2/PKG-INFO
```

### Comparing `actymath-0.1.1/LICENSE` & `actymath-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/README.md` & `actymath-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 Install using pip
 
     pip install actymath
 
 ### Getting started
 
-This [getting started notebook](notebooks/01_getting_started.ipynb) illustrates how to use the package with a simple example.
+This [getting started notebook](https://github.com/ttamg/actymath/blob/main/notebooks/01_getting_started.ipynb) illustrates how to use the package with a simple example.
 
 ### Actuarial formula
 
 The formula definitions are called **columns** in this package as they spawn columns in a pandas DataFrame.
 
 These formulae can be explored in the [actymath/columns directory](https://github.com/ttamg/actymath/tree/main/actymath/columns).
```

### Comparing `actymath-0.1.1/actymath/calc.py` & `actymath-0.1.2/actymath/calc.py`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/actymath/columns/base.py` & `actymath-0.1.2/actymath/columns/base.py`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/actymath/columns/commutation.py` & `actymath-0.1.2/actymath/columns/commutation.py`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/actymath/columns/interest_rates.py` & `actymath-0.1.2/actymath/columns/interest_rates.py`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/actymath/columns/mortality.py` & `actymath-0.1.2/actymath/columns/mortality.py`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/actymath/columns/term.py` & `actymath-0.1.2/actymath/columns/term.py`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/actymath/columns/timeline.py` & `actymath-0.1.2/actymath/columns/timeline.py`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/actymath/columns/whole_of_life.py` & `actymath-0.1.2/actymath/columns/whole_of_life.py`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/actymath/indexers.py` & `actymath-0.1.2/actymath/indexers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     This will return a slice from current index to the end.
 
     Usage example:
     indexer = SliceToEnd()
     dataframe['column'].rolling(indexer).sum()
     """
 
-    def get_window_bounds(self, num_values, min_periods, center, closed):
+    def get_window_bounds(self, num_values, min_periods, center, closed, step):
         start = np.arange(num_values, dtype=np.int64)
         end = np.full(num_values, num_values, dtype=np.int64)
         return start, end
 
 
 class SliceNIndexer(BaseIndexer):
     """
```

### Comparing `actymath-0.1.1/actymath/table_data/a1967-70.csv` & `actymath-0.1.2/actymath/table_data/a1967-70.csv`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/actymath/table_data/a1967-70_exam.csv` & `actymath-0.1.2/actymath/table_data/a1967-70_exam.csv`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/actymath/table_data/amc00.csv` & `actymath-0.1.2/actymath/table_data/amc00.csv`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/actymath/table_data/test.csv` & `actymath-0.1.2/actymath/table_data/test.csv`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/actymath/tables.py` & `actymath-0.1.2/actymath/tables.py`

 * *Files identical despite different names*

### Comparing `actymath-0.1.1/pyproject.toml` & `actymath-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "actymath"
-version = "0.1.1"
+version = "0.1.2"
 description = "Actuarial Math and commutation functions for life insurance product - with a Pandas backend"
 authors = ["Matt Gosden <mdgosden@gmail.com>"]
-license= "MIT"
-readme='README.md'
+license = "MIT"
+readme = 'README.md'
 homepage = "https://github.com/ttamg/actymath"
 repository = "https://github.com/ttamg/actymath"
-exclude=["notebooks"]
-keywords=["actuarial", "pandas", "insurance"]
+exclude = ["notebooks"]
+keywords = ["actuarial", "pandas", "insurance"]
 
 [tool.poetry.dependencies]
 python = ">=3.8 <4.0"
-pandas = "^1.1.5"
+pandas = "^2.0.0"
 parse = "^1.19.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.3.0"
+pylint = "^2.17.2"
+black = "^23.3.0"
+pytest-randomly = "^3.12.0"
 jupyter = "^1.0.0"
-pylint = "^2.8.2"
-black = "^21.4b2"
-nb-black = "^1.0.7"
-pytest-randomly = "^3.7.0"
+ipykernel = "^6.22.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `actymath-0.1.1/PKG-INFO` & `actymath-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: actymath
-Version: 0.1.1
+Version: 0.1.2
 Summary: Actuarial Math and commutation functions for life insurance product - with a Pandas backend
 Home-page: https://github.com/ttamg/actymath
 License: MIT
 Keywords: actuarial,pandas,insurance
 Author: Matt Gosden
 Author-email: mdgosden@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: pandas (>=1.1.5,<2.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: parse (>=1.19.0,<2.0.0)
 Project-URL: Repository, https://github.com/ttamg/actymath
 Description-Content-Type: text/markdown
 
 # actymath
 
 Actuarial formulae and commutation functions for life insurance products (with a fast Pandas backend)
@@ -39,15 +41,15 @@
 
 Install using pip
 
     pip install actymath
 
 ### Getting started
 
-This [getting started notebook](notebooks/01_getting_started.ipynb) illustrates how to use the package with a simple example.
+This [getting started notebook](https://github.com/ttamg/actymath/blob/main/notebooks/01_getting_started.ipynb) illustrates how to use the package with a simple example.
 
 ### Actuarial formula
 
 The formula definitions are called **columns** in this package as they spawn columns in a pandas DataFrame.
 
 These formulae can be explored in the [actymath/columns directory](https://github.com/ttamg/actymath/tree/main/actymath/columns).
```

