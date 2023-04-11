# Comparing `tmp/perun.proxy.utils-1.0.0.tar.gz` & `tmp/perun.proxy.utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun.proxy.utils-1.0.0.tar", last modified: Fri Mar 31 13:20:00 2023, max compression
+gzip compressed data, was "perun.proxy.utils-1.1.0.tar", last modified: Tue Apr 11 08:13:36 2023, max compression
```

## Comparing `perun.proxy.utils-1.0.0.tar` & `perun.proxy.utils-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 13:20:00.744875 perun.proxy.utils-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-03-31 13:01:55.000000 perun.proxy.utils-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      268 2023-03-31 13:20:00.744875 perun.proxy.utils-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1736 2023-03-31 13:01:55.000000 perun.proxy.utils-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 13:20:00.744875 perun.proxy.utils-1.0.0/perun/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 13:20:00.744875 perun.proxy.utils-1.0.0/perun/proxy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 13:20:00.744875 perun.proxy.utils-1.0.0/perun/proxy/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 13:01:55.000000 perun.proxy.utils-1.0.0/perun/proxy/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-03-31 13:01:55.000000 perun.proxy.utils-1.0.0/perun/proxy/utils/metadata_expiration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 13:20:00.744875 perun.proxy.utils-1.0.0/perun/proxy/utils/nagios/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 13:01:55.000000 perun.proxy.utils-1.0.0/perun/proxy/utils/nagios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    72133 2023-03-31 13:01:55.000000 perun.proxy.utils-1.0.0/perun/proxy/utils/nagios/check_mongodb.py
--rwxrwxrwx   0 root         (0) root         (0)     2322 2023-03-31 13:01:55.000000 perun.proxy.utils-1.0.0/perun/proxy/utils/print_docker_versions.py
--rw-rw-rw-   0 root         (0) root         (0)     3038 2023-03-31 13:01:55.000000 perun.proxy.utils-1.0.0/perun/proxy/utils/run_version_script.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-03-31 13:01:55.000000 perun.proxy.utils-1.0.0/perun/proxy/utils/separate_oidc_logs.py
--rwxrwxrwx   0 root         (0) root         (0)     2238 2023-03-31 13:01:55.000000 perun.proxy.utils-1.0.0/perun/proxy/utils/separate_ssp_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 13:20:00.744875 perun.proxy.utils-1.0.0/perun.proxy.utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      268 2023-03-31 13:20:00.000000 perun.proxy.utils-1.0.0/perun.proxy.utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      552 2023-03-31 13:20:00.000000 perun.proxy.utils-1.0.0/perun.proxy.utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 13:20:00.000000 perun.proxy.utils-1.0.0/perun.proxy.utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-03-31 13:20:00.000000 perun.proxy.utils-1.0.0/perun.proxy.utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-31 13:20:00.000000 perun.proxy.utils-1.0.0/perun.proxy.utils.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-03-31 13:20:00.744875 perun.proxy.utils-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-03-31 13:01:55.000000 perun.proxy.utils-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:13:36.377790 perun.proxy.utils-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-03-31 13:01:55.000000 perun.proxy.utils-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      268 2023-04-11 08:13:36.377790 perun.proxy.utils-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2273 2023-03-31 13:21:34.000000 perun.proxy.utils-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:13:36.045782 perun.proxy.utils-1.1.0/perun/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:13:36.045782 perun.proxy.utils-1.1.0/perun/proxy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:13:36.249787 perun.proxy.utils-1.1.0/perun/proxy/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 13:01:55.000000 perun.proxy.utils-1.1.0/perun/proxy/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-03-31 13:01:55.000000 perun.proxy.utils-1.1.0/perun/proxy/utils/metadata_expiration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:13:36.365790 perun.proxy.utils-1.1.0/perun/proxy/utils/nagios/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 13:01:55.000000 perun.proxy.utils-1.1.0/perun/proxy/utils/nagios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    72133 2023-03-31 13:01:55.000000 perun.proxy.utils-1.1.0/perun/proxy/utils/nagios/check_mongodb.py
+-rwxrwxrwx   0 root         (0) root         (0)    18134 2023-03-31 13:21:34.000000 perun.proxy.utils-1.1.0/perun/proxy/utils/nagios/check_saml.py
+-rw-rw-rw-   0 root         (0) root         (0)     3193 2023-03-31 14:17:55.000000 perun.proxy.utils-1.1.0/perun/proxy/utils/nagios/check_user_logins.py
+-rwxrwxrwx   0 root         (0) root         (0)     2322 2023-03-31 13:01:55.000000 perun.proxy.utils-1.1.0/perun/proxy/utils/print_docker_versions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3038 2023-03-31 13:01:55.000000 perun.proxy.utils-1.1.0/perun/proxy/utils/run_version_script.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-03-31 13:01:55.000000 perun.proxy.utils-1.1.0/perun/proxy/utils/separate_oidc_logs.py
+-rwxrwxrwx   0 root         (0) root         (0)     2238 2023-03-31 13:01:55.000000 perun.proxy.utils-1.1.0/perun/proxy/utils/separate_ssp_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:13:36.053782 perun.proxy.utils-1.1.0/perun.proxy.utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-04-11 08:13:35.000000 perun.proxy.utils-1.1.0/perun.proxy.utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      637 2023-04-11 08:13:35.000000 perun.proxy.utils-1.1.0/perun.proxy.utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 08:13:35.000000 perun.proxy.utils-1.1.0/perun.proxy.utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2023-04-11 08:13:35.000000 perun.proxy.utils-1.1.0/perun.proxy.utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-11 08:13:35.000000 perun.proxy.utils-1.1.0/perun.proxy.utils.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-11 08:13:36.381790 perun.proxy.utils-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-03-31 13:01:55.000000 perun.proxy.utils-1.1.0/setup.py
```

### Comparing `perun.proxy.utils-1.0.0/LICENSE` & `perun.proxy.utils-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.0.0/README.md` & `perun.proxy.utils-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # ProxyIdP scripts
 
-All nagios scripts are located under `nagios` directory.
-
-## List scripts
+## Scripts
 
 ### separate_ssp_script.py
 
 - Script for remove all logs from test accounts from SimpleSAMLlogs
 
 - Params:
   - 1 - The file name
@@ -39,15 +37,44 @@
 - This scripts runs the print_docker_version.py script on the given machines. The collected versions are then printed as a MD table to the stdout
 
 - Options:
   - -e,--exclude NAMES - space delimited string of container names to exclude from the listing
 - Params:
   - 1... - machines to run the script on in the form of user@adress, the user needs root privileges to execute the script
 
+## Nagios probes
+
+All nagios scripts are located under `nagios` directory.
+
 ### check_mongodb.py
 
 - nagios monitoring probe for mongodb
 
 - connect, connections, replication_lag, replset_state monitoring options are tested (some possible options may not work since there are constructs which are not supported by latest mongodb versions)
 
-- For usage run:
+- for usage run:
   `python3 check_mongodb.py --help`
+
+### check_saml.py
+
+- SAML authentication check
+
+- for usage run:
+  `python3 check_saml.py --help`
+
+### check_user_logins.py
+
+- check users which login in repeatedly more often than a specified threshold (logins per seconds)
+
+- for usage run:
+  `python3 check_user_logins.py --help`
+
+- example:
+
+```
+python3 check_user_logins.py
+    -p /var/log/proxyaai/simplesamlphp/simplesamlphp/simplesamlphp.log
+    -l 5
+    -s 60
+    -r "^(?P<datetime>.{20}).*audit-login.* (?P<userid>[0-9]+)@muni\.cz$"
+    -d "%b %d %Y %H:%M:%S"
+```
```

### Comparing `perun.proxy.utils-1.0.0/perun/proxy/utils/nagios/check_mongodb.py` & `perun.proxy.utils-1.1.0/perun/proxy/utils/nagios/check_mongodb.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.0.0/perun/proxy/utils/print_docker_versions.py` & `perun.proxy.utils-1.1.0/perun/proxy/utils/print_docker_versions.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.0.0/perun/proxy/utils/run_version_script.py` & `perun.proxy.utils-1.1.0/perun/proxy/utils/run_version_script.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.0.0/perun/proxy/utils/separate_oidc_logs.py` & `perun.proxy.utils-1.1.0/perun/proxy/utils/separate_oidc_logs.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-1.0.0/perun/proxy/utils/separate_ssp_logs.py` & `perun.proxy.utils-1.1.0/perun/proxy/utils/separate_ssp_logs.py`

 * *Files identical despite different names*

