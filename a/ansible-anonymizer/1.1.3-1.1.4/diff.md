# Comparing `tmp/ansible-anonymizer-1.1.3.tar.gz` & `tmp/ansible-anonymizer-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-anonymizer-1.1.3.tar", last modified: Wed Apr  5 20:49:11 2023, max compression
+gzip compressed data, was "ansible-anonymizer-1.1.4.tar", last modified: Tue Apr 11 15:12:13 2023, max compression
```

## Comparing `ansible-anonymizer-1.1.3.tar` & `ansible-anonymizer-1.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-05 20:49:11.662052 ansible-anonymizer-1.1.3/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      292 2023-03-10 14:59:31.000000 ansible-anonymizer-1.1.3/.editorconfig
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-05 20:49:11.660052 ansible-anonymizer-1.1.3/.github/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      321 2023-03-23 15:13:37.000000 ansible-anonymizer-1.1.3/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-05 20:49:11.660052 ansible-anonymizer-1.1.3/.github/workflows/
--rw-r--r--   0 goneri    (1002) goneri    (1002)      551 2023-03-10 14:59:31.000000 ansible-anonymizer-1.1.3/.github/workflows/tox.yml
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1204 2023-03-10 14:59:31.000000 ansible-anonymizer-1.1.3/.gitignore
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1138 2023-04-05 13:57:02.000000 ansible-anonymizer-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0 goneri    (1002) goneri    (1002)      866 2023-04-05 20:45:20.000000 ansible-anonymizer-1.1.3/CHANGELOG.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)     2478 2023-03-23 15:13:37.000000 ansible-anonymizer-1.1.3/CONTRIBUTING.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)       63 2023-03-10 14:59:31.000000 ansible-anonymizer-1.1.3/HISTORY.rst
--rw-r--r--   0 goneri    (1002) goneri    (1002)      588 2023-03-22 17:41:29.000000 ansible-anonymizer-1.1.3/LICENSE
--rw-r--r--   0 goneri    (1002) goneri    (1002)      168 2023-04-05 18:22:37.000000 ansible-anonymizer-1.1.3/MANIFEST.in
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1554 2023-04-05 20:49:11.662052 ansible-anonymizer-1.1.3/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1110 2023-04-05 13:57:47.000000 ansible-anonymizer-1.1.3/README.rst
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-05 20:49:11.660052 ansible-anonymizer-1.1.3/ansible_anonymizer/
--rw-r--r--   0 goneri    (1002) goneri    (1002)       90 2023-04-05 20:48:17.000000 ansible-anonymizer-1.1.3/ansible_anonymizer/__init__.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)    11207 2023-04-05 20:32:36.000000 ansible-anonymizer-1.1.3/ansible_anonymizer/anonymizer.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)      757 2023-03-31 17:38:17.000000 ansible-anonymizer-1.1.3/ansible_anonymizer/cli.py
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-05 20:49:11.661052 ansible-anonymizer-1.1.3/ansible_anonymizer.egg-info/
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1554 2023-04-05 20:49:11.000000 ansible-anonymizer-1.1.3/ansible_anonymizer.egg-info/PKG-INFO
--rw-r--r--   0 goneri    (1002) goneri    (1002)      566 2023-04-05 20:49:11.000000 ansible-anonymizer-1.1.3/ansible_anonymizer.egg-info/SOURCES.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2023-04-05 20:49:11.000000 ansible-anonymizer-1.1.3/ansible_anonymizer.egg-info/dependency_links.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2023-04-05 20:49:11.000000 ansible-anonymizer-1.1.3/ansible_anonymizer.egg-info/entry_points.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       12 2023-04-05 20:49:11.000000 ansible-anonymizer-1.1.3/ansible_anonymizer.egg-info/requires.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)       19 2023-04-05 20:49:11.000000 ansible-anonymizer-1.1.3/ansible_anonymizer.egg-info/top_level.txt
--rw-r--r--   0 goneri    (1002) goneri    (1002)      910 2023-03-31 17:38:17.000000 ansible-anonymizer-1.1.3/pyproject.toml
--rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2023-04-05 20:49:11.662052 ansible-anonymizer-1.1.3/setup.cfg
-drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-05 20:49:11.661052 ansible-anonymizer-1.1.3/tests/
--rw-r--r--   0 goneri    (1002) goneri    (1002)    12536 2023-04-05 20:32:36.000000 ansible-anonymizer-1.1.3/tests/test_anonymizer.py
--rw-r--r--   0 goneri    (1002) goneri    (1002)     1155 2023-04-05 13:57:03.000000 ansible-anonymizer-1.1.3/tox.ini
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-11 15:12:13.541434 ansible-anonymizer-1.1.4/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      292 2023-03-10 14:59:31.000000 ansible-anonymizer-1.1.4/.editorconfig
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-11 15:12:13.539434 ansible-anonymizer-1.1.4/.github/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      321 2023-03-23 15:13:37.000000 ansible-anonymizer-1.1.4/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-11 15:12:13.539434 ansible-anonymizer-1.1.4/.github/workflows/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      551 2023-03-10 14:59:31.000000 ansible-anonymizer-1.1.4/.github/workflows/tox.yml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1204 2023-03-10 14:59:31.000000 ansible-anonymizer-1.1.4/.gitignore
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1138 2023-04-05 13:57:02.000000 ansible-anonymizer-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      999 2023-04-11 15:11:55.000000 ansible-anonymizer-1.1.4/CHANGELOG.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     2478 2023-03-23 15:13:37.000000 ansible-anonymizer-1.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       63 2023-03-10 14:59:31.000000 ansible-anonymizer-1.1.4/HISTORY.rst
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      588 2023-03-22 17:41:29.000000 ansible-anonymizer-1.1.4/LICENSE
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      168 2023-04-05 18:22:37.000000 ansible-anonymizer-1.1.4/MANIFEST.in
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1554 2023-04-11 15:12:13.541434 ansible-anonymizer-1.1.4/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1110 2023-04-05 13:57:47.000000 ansible-anonymizer-1.1.4/README.rst
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-11 15:12:13.539434 ansible-anonymizer-1.1.4/ansible_anonymizer/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       90 2023-04-11 15:10:03.000000 ansible-anonymizer-1.1.4/ansible_anonymizer/__init__.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    11527 2023-04-11 15:10:03.000000 ansible-anonymizer-1.1.4/ansible_anonymizer/anonymizer.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      757 2023-03-31 17:38:17.000000 ansible-anonymizer-1.1.4/ansible_anonymizer/cli.py
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-11 15:12:13.540434 ansible-anonymizer-1.1.4/ansible_anonymizer.egg-info/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1554 2023-04-11 15:12:13.000000 ansible-anonymizer-1.1.4/ansible_anonymizer.egg-info/PKG-INFO
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      566 2023-04-11 15:12:13.000000 ansible-anonymizer-1.1.4/ansible_anonymizer.egg-info/SOURCES.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)        1 2023-04-11 15:12:13.000000 ansible-anonymizer-1.1.4/ansible_anonymizer.egg-info/dependency_links.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       67 2023-04-11 15:12:13.000000 ansible-anonymizer-1.1.4/ansible_anonymizer.egg-info/entry_points.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       12 2023-04-11 15:12:13.000000 ansible-anonymizer-1.1.4/ansible_anonymizer.egg-info/requires.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       19 2023-04-11 15:12:13.000000 ansible-anonymizer-1.1.4/ansible_anonymizer.egg-info/top_level.txt
+-rw-r--r--   0 goneri    (1002) goneri    (1002)      910 2023-03-31 17:38:17.000000 ansible-anonymizer-1.1.4/pyproject.toml
+-rw-r--r--   0 goneri    (1002) goneri    (1002)       38 2023-04-11 15:12:13.541434 ansible-anonymizer-1.1.4/setup.cfg
+drwxr-xr-x   0 goneri    (1002) goneri    (1002)        0 2023-04-11 15:12:13.540434 ansible-anonymizer-1.1.4/tests/
+-rw-r--r--   0 goneri    (1002) goneri    (1002)    13033 2023-04-11 15:10:03.000000 ansible-anonymizer-1.1.4/tests/test_anonymizer.py
+-rw-r--r--   0 goneri    (1002) goneri    (1002)     1155 2023-04-05 13:57:03.000000 ansible-anonymizer-1.1.4/tox.ini
```

### Comparing `ansible-anonymizer-1.1.3/.github/workflows/tox.yml` & `ansible-anonymizer-1.1.4/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.3/.gitignore` & `ansible-anonymizer-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.3/.pre-commit-config.yaml` & `ansible-anonymizer-1.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.3/CHANGELOG.rst` & `ansible-anonymizer-1.1.4/CHANGELOG.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+Version 1.1.4  (2023-04-08)
+-------------
+
+- is_uuid_string(): do not anonymize UUID strings
+- test_anonymizer: add UUID test cases
+
 Version 1.1.3  (2023-04-05)
 -------------
 
 - is_password_field_name(): ignore the case of the string
 
 Version 1.1.2  (2023-04-05)
 -------------
```

### Comparing `ansible-anonymizer-1.1.3/CONTRIBUTING.rst` & `ansible-anonymizer-1.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.3/LICENSE` & `ansible-anonymizer-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.3/PKG-INFO` & `ansible-anonymizer-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-anonymizer
-Version: 1.1.3
+Version: 1.1.4
 Summary: Ansible Anonymizer
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
 Project-URL: Homepage, https://github.com/ansible/anonymizer
 Keywords: pii,anonymize
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `ansible-anonymizer-1.1.3/README.rst` & `ansible-anonymizer-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.3/ansible_anonymizer/anonymizer.py` & `ansible-anonymizer-1.1.4/ansible_anonymizer/anonymizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,26 @@
     """Check if an unquoted string hold a Jinja2 variable"""
     if re.match(r"^\s*{{\s*.*?\s*}}\s*$", value):
         return True
 
     return False
 
 
+def is_uuid_string(value: str) -> bool:
+    """Check if a given value is a UUID string"""
+    if re.match(
+        r"^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$",
+        value,
+        flags=re.IGNORECASE,
+    ):
+        return True
+
+    return False
+
+
 common_ipv4_networks = [
     ipaddress.IPv4Network("1.0.0.1/32"),
     ipaddress.IPv4Network("1.1.1.1/32"),
     ipaddress.IPv4Network("149.112.112.112/32"),
     ipaddress.IPv4Network("208.67.220.220/32"),
     ipaddress.IPv4Network("208.67.222.222/32"),
     ipaddress.IPv4Network("76.223.122.150/32"),
@@ -162,14 +174,16 @@
     if value[0] == value[-1] and value[0] in ('"', "'"):
         return value[1:-1]
     return value
 
 
 def anonymize_field(value: str, name: str) -> str:
     v = value.strip()
+    if is_uuid_string(v):
+        return value
     if is_password_field_name(name):
         if is_path(v):
             return value
         if is_jinja2_expression(unquote(v)):
             return unquote(v)
         variable_name = str_jinja2_variable_name(name)
         return f"{{{{ { variable_name } }}}}"
```

### Comparing `ansible-anonymizer-1.1.3/ansible_anonymizer/cli.py` & `ansible-anonymizer-1.1.4/ansible_anonymizer/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.3/ansible_anonymizer.egg-info/PKG-INFO` & `ansible-anonymizer-1.1.4/ansible_anonymizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-anonymizer
-Version: 1.1.3
+Version: 1.1.4
 Summary: Ansible Anonymizer
 Author-email: Gonéri Le Bouder <goneri@lebouder.net>
 Project-URL: Homepage, https://github.com/ansible/anonymizer
 Keywords: pii,anonymize
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

### Comparing `ansible-anonymizer-1.1.3/ansible_anonymizer.egg-info/SOURCES.txt` & `ansible-anonymizer-1.1.4/ansible_anonymizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.3/pyproject.toml` & `ansible-anonymizer-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-anonymizer-1.1.3/tests/test_anonymizer.py` & `ansible-anonymizer-1.1.4/tests/test_anonymizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from ansible_anonymizer.anonymizer import hide_secrets
 from ansible_anonymizer.anonymizer import hide_us_phone_numbers
 from ansible_anonymizer.anonymizer import hide_us_ssn
 from ansible_anonymizer.anonymizer import hide_user_name
 from ansible_anonymizer.anonymizer import is_jinja2_expression
 from ansible_anonymizer.anonymizer import is_password_field_name
 from ansible_anonymizer.anonymizer import is_path
+from ansible_anonymizer.anonymizer import is_uuid_string
 from ansible_anonymizer.anonymizer import redact_ip_address
 from ansible_anonymizer.anonymizer import redact_ipv4_address
 from ansible_anonymizer.anonymizer import redact_ipv6_address
 from ansible_anonymizer.anonymizer import unquote
 
 
 def test_is_password_field_name():
@@ -413,7 +414,21 @@
 def test_unquote():
     assert unquote("'a'") == 'a'
     assert unquote('"a"') == 'a'
     assert unquote('"a\'') == '"a\''
     assert unquote('a') == 'a'
     assert unquote("''") == ""
     assert unquote("'") == "'"
+
+
+def test_is_uuid_string():
+    assert is_uuid_string('ce34efc1-f5e3-4b0f-bb2c-5272319589a7') is True
+    assert is_uuid_string('CE34EFC1-F5E3-4B0F-BB2C-5272319589A7') is True
+
+
+def test_anonymize_uuid_field():
+    field = "uuid_field"
+    value = "ce34efc1-f5e3-4b0f-bb2c-5272319589a7"
+    assert anonymize_field(value, field) == value
+
+    value = "CE34EFC1-F5E3-4B0F-BB2C-5272319589A7"
+    assert anonymize_field(value, field) == value
```

### Comparing `ansible-anonymizer-1.1.3/tox.ini` & `ansible-anonymizer-1.1.4/tox.ini`

 * *Files identical despite different names*

