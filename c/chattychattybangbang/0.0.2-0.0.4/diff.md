# Comparing `tmp/chattychattybangbang-0.0.2.tar.gz` & `tmp/chattychattybangbang-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chattychattybangbang-0.0.2.tar", last modified: Tue Apr 11 02:16:49 2023, max compression
+gzip compressed data, was "chattychattybangbang-0.0.4.tar", last modified: Tue Apr 11 15:47:56 2023, max compression
```

## Comparing `chattychattybangbang-0.0.2.tar` & `chattychattybangbang-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:16:49.063090 chattychattybangbang-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 02:16:27.000000 chattychattybangbang-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-11 02:16:49.063090 chattychattybangbang-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-11 02:16:27.000000 chattychattybangbang-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:16:49.063090 chattychattybangbang-0.0.2/chattychattybangbang/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 02:16:27.000000 chattychattybangbang-0.0.2/chattychattybangbang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-11 02:16:27.000000 chattychattybangbang-0.0.2/chattychattybangbang/castigateuntilvalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-11 02:16:27.000000 chattychattybangbang-0.0.2/chattychattybangbang/castigateuntilvaluesare.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 02:16:27.000000 chattychattybangbang-0.0.2/chattychattybangbang/castigators.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 02:16:27.000000 chattychattybangbang-0.0.2/chattychattybangbang/jsonutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-11 02:16:27.000000 chattychattybangbang-0.0.2/chattychattybangbang/openaicredentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-11 02:16:27.000000 chattychattybangbang-0.0.2/chattychattybangbang/openutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-11 02:16:27.000000 chattychattybangbang-0.0.2/chattychattybangbang/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 02:16:27.000000 chattychattybangbang-0.0.2/chattychattybangbang/whereami.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:16:49.063090 chattychattybangbang-0.0.2/chattychattybangbang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-11 02:16:49.000000 chattychattybangbang-0.0.2/chattychattybangbang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-11 02:16:49.000000 chattychattybangbang-0.0.2/chattychattybangbang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:16:49.000000 chattychattybangbang-0.0.2/chattychattybangbang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 02:16:49.000000 chattychattybangbang-0.0.2/chattychattybangbang.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 02:16:49.000000 chattychattybangbang-0.0.2/chattychattybangbang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 02:16:49.000000 chattychattybangbang-0.0.2/chattychattybangbang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:16:49.063090 chattychattybangbang-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-11 02:16:27.000000 chattychattybangbang-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:47:56.190847 chattychattybangbang-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-11 15:47:56.190847 chattychattybangbang-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:47:56.190847 chattychattybangbang-0.0.4/chattychattybangbang/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/castigateuntilvalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/castigateuntilvaluesare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/castigators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/jsonutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/openaicredentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/openutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/chattychattybangbang/whereami.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:47:56.190847 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-11 15:47:56.000000 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-11 15:47:56.000000 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:47:56.000000 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-11 15:47:56.000000 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-11 15:47:56.000000 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 15:47:56.000000 chattychattybangbang-0.0.4/chattychattybangbang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:47:56.190847 chattychattybangbang-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-11 15:47:25.000000 chattychattybangbang-0.0.4/setup.py
```

### Comparing `chattychattybangbang-0.0.2/LICENSE` & `chattychattybangbang-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chattychattybangbang-0.0.2/chattychattybangbang/castigateuntilvalid.py` & `chattychattybangbang-0.0.4/chattychattybangbang/castigateuntilvalid.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from chattychattybangbang.openaicredentials import set_credentials
-from chattychattybangbang.validators import default_validator
+from chattychattybangbang.validators import default_validator, validate_numeric_dict
 from chattychattybangbang.jsonutil import json_or_none
 from chattychattybangbang.castigators import default_castigator
 from chattychattybangbang.openutil import ask_gpt
 
 
 DEFAULT_MAX_RETRIES = 3
 
 
-def castigate_until_valid(question:str, validator=None, castigator=None, max_retries=DEFAULT_MAX_RETRIES):
+def castigate_until_valid(question:str, validator=None, castigator=None, max_retries:int=DEFAULT_MAX_RETRIES):
+    """
+    :param question:
+    :param validator:     Function taking dict --> bool
+    :param castigator:    Function taking castigator(question, response) --> str
+    :param max_retries:
+    :return:
+    """
     if validator is None:
         validator = default_validator
     if castigator is None:
         castigator = default_castigator
 
     retries = 0
 
@@ -28,14 +35,17 @@
 
     if retries == max_retries:
         return None
     else:
         return parsed_response
 
 
+def castigate_until_numeric_dict(question:str, castigator=None, max_retries=DEFAULT_MAX_RETRIES):
+    return castigate_until_valid(question=question, validator=validate_numeric_dict, max_retries=max_retries)
+
 
 if __name__=='__main__':
     question = """
       I would like you to create a dictionary by choosing three tickers from companies
       that were in the sp500 index in 2011 and returning a dictionary with keys given by
       the tickers and values equal to a text description of the colors of the companies
       in question.
```

### Comparing `chattychattybangbang-0.0.2/chattychattybangbang/castigateuntilvaluesare.py` & `chattychattybangbang-0.0.4/chattychattybangbang/castigateuntilvaluesare.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 from chattychattybangbang.castigateuntilvalid import castigate_until_valid
 from chattychattybangbang.validators import validate_yes_or_no
 
 DEFAULT_MAX_RETRIES = 3
+DEFAULT_N_CHECK = 5
 
 
-def values_isa_validator(parsed_response: dict, value_description:str, max_retries=DEFAULT_MAX_RETRIES):
+def values_isa_validator(parsed_response: dict, value_description:str,
+                         max_retries=DEFAULT_MAX_RETRIES, n_check=DEFAULT_N_CHECK):
     """ For each value in a dictionary, ask ChatGPT if it meets value_description
         Short-circuit
     :param value_description:  'is a president'
+    :param n_check:            How many to check
     :return:
     """
+    n_checked = 0
     for k, v in parsed_response.items():
         validation_question = 'Please answer the following as a yes or no question only, returning a single word please. Is ' + str(
             v) + ' ' + value_description + ' ?'
         yes_or_no_dict = castigate_until_valid(question=validation_question,
                                           validator=validate_yes_or_no,
                                           max_retries=max_retries)
         if yes_or_no_dict is None:
             return False
         else:
             yes_or_no_values = list(yes_or_no_dict.values())[0]
             if not isinstance(yes_or_no_values, str) or (('no' in yes_or_no_values.lower()) and ('yes' not in yes_or_no_values.lower())):
                 return False
+            else:
+                n_checked+=1
+                if n_checked>=n_check:
+                    break
     return True
 
 
-def castigate_until_values_are(question:str, value_description:str, castigator=None, max_retries=DEFAULT_MAX_RETRIES):
+def castigate_until_values_are(question:str, value_description:str,
+                               castigator=None, max_retries=DEFAULT_MAX_RETRIES,
+                               n_check=5):
     """ Retry until we get a dict whose values are 'value_description'
     :param question:   'Please provide a dictionary length 3 where
     :param value_description:  'is a color'
     :param castigator:
     :param max_retries:
     :return:
     """
     def _validator(parsed_response):
-         return values_isa_validator(parsed_response=parsed_response, value_description=value_description)
+         return values_isa_validator(parsed_response=parsed_response,
+                                     value_description=value_description,
+                                     n_check=n_check)
 
     return castigate_until_valid(question=question,
                                 validator=_validator,
                                   castigator=castigator,
                                 max_retries=max_retries)
```

### Comparing `chattychattybangbang-0.0.2/chattychattybangbang.egg-info/SOURCES.txt` & `chattychattybangbang-0.0.4/chattychattybangbang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chattychattybangbang-0.0.2/setup.py` & `chattychattybangbang-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="chattychattybangbang",
-    version="0.0.2",
+    version="0.0.4",
     description="chat utilities",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/chattychattybangbang/chattychattybangbang",
     author="chattychattybangbang",
     author_email="pcotton@intechinvestments.com",
     license="MIT",
```

