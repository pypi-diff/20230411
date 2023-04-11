# Comparing `tmp/ffiec-data-connect-0.2.6.tar.gz` & `tmp/ffiec-data-connect-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffiec-data-connect-0.2.6.tar", last modified: Sat Apr  8 01:39:18 2023, max compression
+gzip compressed data, was "ffiec-data-connect-0.2.7.tar", last modified: Tue Apr 11 01:57:13 2023, max compression
```

## Comparing `ffiec-data-connect-0.2.6.tar` & `ffiec-data-connect-0.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-08 01:39:18.905857 ffiec-data-connect-0.2.6/
--rw-r--r--   0 michael    (501) staff       (20)     1072 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.6/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     3217 2023-04-08 01:39:18.905937 ffiec-data-connect-0.2.6/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     2608 2023-04-08 01:26:10.000000 ffiec-data-connect-0.2.6/README.md
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.6/pyproject.toml
--rw-r--r--   0 michael    (501) staff       (20)      107 2023-04-08 01:39:18.906209 ffiec-data-connect-0.2.6/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1082 2023-04-08 01:38:43.000000 ffiec-data-connect-0.2.6/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-08 01:39:18.902027 ffiec-data-connect-0.2.6/src/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-08 01:39:18.904719 ffiec-data-connect-0.2.6/src/ffiec_data_connect/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.6/src/ffiec_data_connect/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      384 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.6/src/ffiec_data_connect/constants.py
--rw-r--r--   0 michael    (501) staff       (20)     7130 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.6/src/ffiec_data_connect/credentials.py
--rw-r--r--   0 michael    (501) staff       (20)     3805 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.6/src/ffiec_data_connect/datahelpers.py
--rw-r--r--   0 michael    (501) staff       (20)      106 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.6/src/ffiec_data_connect/exceptions.py
--rw-r--r--   0 michael    (501) staff       (20)     8585 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.6/src/ffiec_data_connect/ffiec_connection.py
--rw-r--r--   0 michael    (501) staff       (20)    23458 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.6/src/ffiec_data_connect/methods.py
--rw-r--r--   0 michael    (501) staff       (20)     4085 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.6/src/ffiec_data_connect/xbrl_processor.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-08 01:39:18.905703 ffiec-data-connect-0.2.6/src/ffiec_data_connect.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     3217 2023-04-08 01:39:18.000000 ffiec-data-connect-0.2.6/src/ffiec_data_connect.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      586 2023-04-08 01:39:18.000000 ffiec-data-connect-0.2.6/src/ffiec_data_connect.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-08 01:39:18.000000 ffiec-data-connect-0.2.6/src/ffiec_data_connect.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       31 2023-04-08 01:39:18.000000 ffiec-data-connect-0.2.6/src/ffiec_data_connect.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       19 2023-04-08 01:39:18.000000 ffiec-data-connect-0.2.6/src/ffiec_data_connect.egg-info/top_level.txt
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-11 01:57:13.041313 ffiec-data-connect-0.2.7/
+-rw-r--r--   0 michael    (501) staff       (20)     1072 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.7/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     3217 2023-04-11 01:57:13.041398 ffiec-data-connect-0.2.7/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     2608 2023-04-08 01:26:10.000000 ffiec-data-connect-0.2.7/README.md
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.7/pyproject.toml
+-rw-r--r--   0 michael    (501) staff       (20)      107 2023-04-11 01:57:13.041689 ffiec-data-connect-0.2.7/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1082 2023-04-11 01:56:33.000000 ffiec-data-connect-0.2.7/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-11 01:57:13.037464 ffiec-data-connect-0.2.7/src/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-11 01:57:13.039958 ffiec-data-connect-0.2.7/src/ffiec_data_connect/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.7/src/ffiec_data_connect/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      384 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.7/src/ffiec_data_connect/constants.py
+-rw-r--r--   0 michael    (501) staff       (20)     7130 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.7/src/ffiec_data_connect/credentials.py
+-rw-r--r--   0 michael    (501) staff       (20)     3805 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.7/src/ffiec_data_connect/datahelpers.py
+-rw-r--r--   0 michael    (501) staff       (20)      106 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.7/src/ffiec_data_connect/exceptions.py
+-rw-r--r--   0 michael    (501) staff       (20)     8585 2023-03-24 20:50:39.000000 ffiec-data-connect-0.2.7/src/ffiec_data_connect/ffiec_connection.py
+-rw-r--r--   0 michael    (501) staff       (20)    23948 2023-04-11 01:55:32.000000 ffiec-data-connect-0.2.7/src/ffiec_data_connect/methods.py
+-rw-r--r--   0 michael    (501) staff       (20)     4523 2023-04-11 01:56:01.000000 ffiec-data-connect-0.2.7/src/ffiec_data_connect/xbrl_processor.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-11 01:57:13.041139 ffiec-data-connect-0.2.7/src/ffiec_data_connect.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     3217 2023-04-11 01:57:13.000000 ffiec-data-connect-0.2.7/src/ffiec_data_connect.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      586 2023-04-11 01:57:13.000000 ffiec-data-connect-0.2.7/src/ffiec_data_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-11 01:57:13.000000 ffiec-data-connect-0.2.7/src/ffiec_data_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       31 2023-04-11 01:57:13.000000 ffiec-data-connect-0.2.7/src/ffiec_data_connect.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       19 2023-04-11 01:57:13.000000 ffiec-data-connect-0.2.7/src/ffiec_data_connect.egg-info/top_level.txt
```

### Comparing `ffiec-data-connect-0.2.6/LICENSE.txt` & `ffiec-data-connect-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ffiec-data-connect-0.2.6/PKG-INFO` & `ffiec-data-connect-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffiec-data-connect
-Version: 0.2.6
+Version: 0.2.7
 Summary: Wrapper for the FFIEC's Webservice API
 Home-page: https://github.com/call-report/ffiec-data-connect
 Author: Michael Handelman
 Author-email: m@mikeh.dev
 License: MIT
 Project-URL: Documentation, https://ffiec-data-connect.readthedocs.io/en/latest/
 Project-URL: Repo, https://github.com/call-report/ffiec-data-connect
```

### Comparing `ffiec-data-connect-0.2.6/README.md` & `ffiec-data-connect-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ffiec-data-connect-0.2.6/setup.py` & `ffiec-data-connect-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ffiec-data-connect',
     python_requires='>3.9.0',
-    version='0.2.6',
+    version='0.2.7',
     license='MIT',
     description="Wrapper for the FFIEC's Webservice API",
     readme='README.md',
     long_description=long_description,
     project_urls={
     'Documentation': 'https://ffiec-data-connect.readthedocs.io/en/latest/',
     'Repo': 'https://github.com/call-report/ffiec-data-connect',
```

### Comparing `ffiec-data-connect-0.2.6/src/ffiec_data_connect/credentials.py` & `ffiec-data-connect-0.2.7/src/ffiec_data_connect/credentials.py`

 * *Files identical despite different names*

### Comparing `ffiec-data-connect-0.2.6/src/ffiec_data_connect/datahelpers.py` & `ffiec-data-connect-0.2.7/src/ffiec_data_connect/datahelpers.py`

 * *Files identical despite different names*

### Comparing `ffiec-data-connect-0.2.6/src/ffiec_data_connect/ffiec_connection.py` & `ffiec-data-connect-0.2.7/src/ffiec_data_connect/ffiec_connection.py`

 * *Files identical despite different names*

### Comparing `ffiec-data-connect-0.2.6/src/ffiec_data_connect/methods.py` & `ffiec-data-connect-0.2.7/src/ffiec_data_connect/methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,34 +20,51 @@
 yyyymmddRegex = r"^[0-9]{4}[0-9]{2}[0-9]{2}$"
 yyyymmddDashRegex = r"^[0-9]{4}-[0-9]{2}-[0-9]{2}$"
 mmddyyyyRegex = r"^[0-9]{1,2}/[0-9]{1,2}/[0-9]{4}$"
 
 validRegexList = [quarterStringRegex, yyyymmddRegex, yyyymmddDashRegex, mmddyyyyRegex]
 
 
+def _create_ffiec_date_from_datetime(indate: datetime) -> str:
+    """Converts a datetime object to a FFIEC-formatted date
+
+    Args:
+        indate (datetime): the date to convert
+
+    Returns:
+        str: the date in FFIEC format
+    """
+    month_str = str(indate.month)
+    day_str = str(indate.day)
+    year_str = str(indate.year)
+    
+    mmddyyyy = month_str + "/" + day_str + "/" + year_str
+    
+    return mmddyyyy
+
 def _convert_any_date_to_ffiec_format(indate: str or datetime) -> str:
     """Converts a string-based date or python datetime object to a FFIEC-formatted date
  
     Args:
         date (str or datetime): the date to convert. This can be a string in the format of "YYYY-MM-DD", "YYYYMMDD", "MM/DD/YYYY", or a python datetime object
 
     Returns:
         str: the date in FFIEC format
     """
     
     if isinstance(indate, datetime):
-        return indate.strftime("%-m/%-d/%Y")
+        return _create_ffiec_date_from_datetime(indate)
     elif isinstance(indate, str):
         # does the date have two slashes?
         if indate.count("-") == 2:
-            return datetime.strptime(indate, "%Y-%m-%d").strftime("%-m/%-d/%Y")
+            return _create_ffiec_date_from_datetime(datetime.strptime(indate, "%Y-%m-%d"))
         elif indate.count("/") == 2:
-            return datetime.strptime(indate, "%m/%d/%Y").strftime("%-m/%-d/%Y")
+            return _create_ffiec_date_from_datetime(datetime.strptime(indate, "%m/%d/%Y"))
         elif len(indate) == 8:
-            return datetime.strptime(indate, "%Y%m%d").strftime("%-m/%-d/%Y")    
+            return _create_ffiec_date_from_datetime(datetime.strptime(indate, "%Y%m%d"))  
     else:
         # raise an error if we don't have a valid date
         raise(ValueError("Invalid date format. Must be a string in the format of 'YYYY-MM-DD', 'YYYYMMDD', 'MM/DD/YYYY', or a python datetime object"))
     
 def _convert_quarter_to_date(reporting_period: str) -> datetime:
     
     """Converts date in the format of #QYYYY to a datetime object
@@ -114,18 +131,18 @@
         return any(re.search(regex, reporting_period) for regex in validRegexList)
     else:
         return False # we don't know what to do with this type of input, so return false
     
     
 def _return_ffiec_reporting_date(indate: datetime or str) -> str:
     if isinstance(indate, datetime):
-        return indate.strftime("%-m/%-d/%Y")
+        return _create_ffiec_date_from_datetime(indate)
     elif isinstance(indate, str):
         if indate[1] == "Q":
-            return _convert_quarter_to_date(indate).strftime("%-m/%-d/%Y")
+            return _create_ffiec_date_from_datetime(_convert_quarter_to_date(indate))
         else:
             ffiec_date =  _convert_any_date_to_ffiec_format(indate)
             ffiec_date_month = ffiec_date.split("/")[0]
             ffiec_date_date = ffiec_date.split("/")[1]
             
             if (ffiec_date_month == "3" or ffiec_date_month == "03") and ffiec_date_date == "31":
                 return ffiec_date
```

### Comparing `ffiec-data-connect-0.2.6/src/ffiec_data_connect/xbrl_processor.py` & `ffiec-data-connect-0.2.7/src/ffiec_data_connect/xbrl_processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,14 +54,32 @@
             new_dict.update({'data_type':row['data_type']})
             new_dict.update({'str_data':None})
 
         ret_data.append(new_dict)
     
     return ret_data
 
+
+def _create_ffiec_date_from_datetime(indate: datetime) -> str:
+    """Converts a datetime object to a FFIEC-formatted date
+
+    Args:
+        indate (datetime): the date to convert
+
+    Returns:
+        str: the date in FFIEC format
+    """
+    month_str = str(indate.month)
+    day_str = str(indate.day)
+    year_str = str(indate.year)
+    
+    mmddyyyy = month_str + "/" + day_str + "/" + year_str
+    
+    return mmddyyyy
+
 def _process_xbrl_item(name, items, date_format):
     # incoming is a data dictionary
     results = []
     if type(items) != list:
         items = [items]
     for j,item in enumerate(items):
         context = item.get('@contextRef')
@@ -71,15 +89,15 @@
         rssd = context.split('_')[1]
         #date = int(context.split('_')[2].replace("-",''))
 
         quarter = re_date.findall(context)[0]
 
         # transform the date to the requested date format
         if date_format == 'string_original':
-            quarter = datetime.strptime(quarter, '%Y-%m-%d').strftime('%-m/%-d/%Y')
+            quarter = _create_ffiec_date_from_datetime(datetime.strptime(quarter, '%Y-%m-%d'))
         elif date_format == 'string_yyyymmdd':
             quarter = datetime.strptime(quarter, '%Y-%m-%d').strftime('%Y%m%d')
         elif date_format == 'python_format':
             quarter = datetime.strptime(quarter, '%Y-%m-%d')
         
         data_type = None
```

### Comparing `ffiec-data-connect-0.2.6/src/ffiec_data_connect.egg-info/PKG-INFO` & `ffiec-data-connect-0.2.7/src/ffiec_data_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffiec-data-connect
-Version: 0.2.6
+Version: 0.2.7
 Summary: Wrapper for the FFIEC's Webservice API
 Home-page: https://github.com/call-report/ffiec-data-connect
 Author: Michael Handelman
 Author-email: m@mikeh.dev
 License: MIT
 Project-URL: Documentation, https://ffiec-data-connect.readthedocs.io/en/latest/
 Project-URL: Repo, https://github.com/call-report/ffiec-data-connect
```

### Comparing `ffiec-data-connect-0.2.6/src/ffiec_data_connect.egg-info/SOURCES.txt` & `ffiec-data-connect-0.2.7/src/ffiec_data_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

