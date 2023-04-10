# Comparing `tmp/ldns-explorer-1.2.tar.gz` & `tmp/ldns-explorer-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/CD/Desktop/first/DNS/dist/.tmp-cc0kzenk/ldns-explorer-1.2.tar", last modified: Mon Apr 10 19:41:08 2023, max compression
+gzip compressed data, was "/Users/CD/Desktop/first/DNS/dist/.tmp-26elebgj/ldns-explorer-1.3.tar", last modified: Mon Apr 10 22:26:36 2023, max compression
```

## Comparing `ldns-explorer-1.2.tar` & `ldns-explorer-1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-10 19:41:08.340955 ldns-explorer-1.2/
--rw-r--r--   0 CD         (501) staff       (20)     2238 2023-04-10 19:41:08.340588 ldns-explorer-1.2/PKG-INFO
--rw-r--r--   0 CD         (501) staff       (20)     1978 2023-04-10 19:39:49.000000 ldns-explorer-1.2/README.md
--rw-r--r--   0 CD         (501) staff       (20)      403 2023-04-10 19:37:23.000000 ldns-explorer-1.2/pyproject.toml
--rw-r--r--   0 CD         (501) staff       (20)       38 2023-04-10 19:41:08.341029 ldns-explorer-1.2/setup.cfg
--rw-r--r--   0 CD         (501) staff       (20)      157 2023-03-28 20:00:36.000000 ldns-explorer-1.2/setup.py
-drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-10 19:41:08.333689 ldns-explorer-1.2/src/
--rw-r--r--   0 CD         (501) staff       (20)        0 2023-03-15 19:25:14.000000 ldns-explorer-1.2/src/__init__.py
--rw-r--r--   0 CD         (501) staff       (20)       67 2023-03-24 21:07:54.000000 ldns-explorer-1.2/src/envplay.py
-drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-10 19:41:08.336022 ldns-explorer-1.2/src/ldns_explorer.egg-info/
--rw-r--r--   0 CD         (501) staff       (20)     2238 2023-04-10 19:41:08.000000 ldns-explorer-1.2/src/ldns_explorer.egg-info/PKG-INFO
--rw-r--r--   0 CD         (501) staff       (20)      489 2023-04-10 19:41:08.000000 ldns-explorer-1.2/src/ldns_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 CD         (501) staff       (20)        1 2023-04-10 19:41:08.000000 ldns-explorer-1.2/src/ldns_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 CD         (501) staff       (20)       21 2023-04-10 19:41:08.000000 ldns-explorer-1.2/src/ldns_explorer.egg-info/requires.txt
--rw-r--r--   0 CD         (501) staff       (20)       30 2023-04-10 19:41:08.000000 ldns-explorer-1.2/src/ldns_explorer.egg-info/top_level.txt
-drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-10 19:41:08.339727 ldns-explorer-1.2/src/ldnsexplorer/
--rw-r--r--   0 CD         (501) staff       (20)     9852 2023-04-10 19:40:55.000000 ldns-explorer-1.2/src/ldnsexplorer/DNS_APP.py
--rw-r--r--   0 CD         (501) staff       (20)        0 2023-03-14 21:01:01.000000 ldns-explorer-1.2/src/ldnsexplorer/__init__.py
--rw-r--r--   0 CD         (501) staff       (20)       40 2023-03-28 16:23:49.000000 ldns-explorer-1.2/src/ldnsexplorer/__main__.py
--rw-r--r--   0 CD         (501) staff       (20)      303 2023-02-27 20:24:11.000000 ldns-explorer-1.2/src/ldnsexplorer/find_local_resolver.py
--rw-r--r--   0 CD         (501) staff       (20)     1439 2023-03-14 04:37:46.000000 ldns-explorer-1.2/src/ldnsexplorer/measure_dns.py
--rw-r--r--   0 CD         (501) staff       (20)      352 2023-03-14 04:52:05.000000 ldns-explorer-1.2/src/ldnsexplorer/measure_tcp.py
--rw-r--r--   0 CD         (501) staff       (20)     1584 2023-03-29 02:06:34.000000 ldns-explorer-1.2/src/ldnsexplorer/tcp_client.py
+drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-10 22:26:36.411703 ldns-explorer-1.3/
+-rw-r--r--   0 CD         (501) staff       (20)     2237 2023-04-10 22:26:36.411445 ldns-explorer-1.3/PKG-INFO
+-rw-r--r--   0 CD         (501) staff       (20)     1977 2023-04-10 22:25:52.000000 ldns-explorer-1.3/README.md
+-rw-r--r--   0 CD         (501) staff       (20)      403 2023-04-10 22:26:25.000000 ldns-explorer-1.3/pyproject.toml
+-rw-r--r--   0 CD         (501) staff       (20)       38 2023-04-10 22:26:36.411776 ldns-explorer-1.3/setup.cfg
+-rw-r--r--   0 CD         (501) staff       (20)      157 2023-03-28 20:00:36.000000 ldns-explorer-1.3/setup.py
+drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-10 22:26:36.406520 ldns-explorer-1.3/src/
+-rw-r--r--   0 CD         (501) staff       (20)        0 2023-03-15 19:25:14.000000 ldns-explorer-1.3/src/__init__.py
+-rw-r--r--   0 CD         (501) staff       (20)       67 2023-03-24 21:07:54.000000 ldns-explorer-1.3/src/envplay.py
+drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-10 22:26:36.407840 ldns-explorer-1.3/src/ldns_explorer.egg-info/
+-rw-r--r--   0 CD         (501) staff       (20)     2237 2023-04-10 22:26:36.000000 ldns-explorer-1.3/src/ldns_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 CD         (501) staff       (20)      489 2023-04-10 22:26:36.000000 ldns-explorer-1.3/src/ldns_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 CD         (501) staff       (20)        1 2023-04-10 22:26:36.000000 ldns-explorer-1.3/src/ldns_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 CD         (501) staff       (20)       21 2023-04-10 22:26:36.000000 ldns-explorer-1.3/src/ldns_explorer.egg-info/requires.txt
+-rw-r--r--   0 CD         (501) staff       (20)       30 2023-04-10 22:26:36.000000 ldns-explorer-1.3/src/ldns_explorer.egg-info/top_level.txt
+drwxr-xr-x   0 CD         (501) staff       (20)        0 2023-04-10 22:26:36.410914 ldns-explorer-1.3/src/ldnsexplorer/
+-rw-r--r--   0 CD         (501) staff       (20)     9852 2023-04-10 19:40:55.000000 ldns-explorer-1.3/src/ldnsexplorer/DNS_APP.py
+-rw-r--r--   0 CD         (501) staff       (20)        0 2023-03-14 21:01:01.000000 ldns-explorer-1.3/src/ldnsexplorer/__init__.py
+-rw-r--r--   0 CD         (501) staff       (20)       40 2023-03-28 16:23:49.000000 ldns-explorer-1.3/src/ldnsexplorer/__main__.py
+-rw-r--r--   0 CD         (501) staff       (20)      303 2023-02-27 20:24:11.000000 ldns-explorer-1.3/src/ldnsexplorer/find_local_resolver.py
+-rw-r--r--   0 CD         (501) staff       (20)     1439 2023-03-14 04:37:46.000000 ldns-explorer-1.3/src/ldnsexplorer/measure_dns.py
+-rw-r--r--   0 CD         (501) staff       (20)      352 2023-03-14 04:52:05.000000 ldns-explorer-1.3/src/ldnsexplorer/measure_tcp.py
+-rw-r--r--   0 CD         (501) staff       (20)     1584 2023-03-29 02:06:34.000000 ldns-explorer-1.3/src/ldnsexplorer/tcp_client.py
```

### Comparing `ldns-explorer-1.2/PKG-INFO` & `ldns-explorer-1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldns-explorer
-Version: 1.2
+Version: 1.3
 Summary: A public DNS resolver explorer
 Author: cwru
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
@@ -58,17 +58,17 @@
 1.1.1.1
 ```
 
 
 ## Disclaimer
 
 The purpose of this project is twofold. On one hand, we hope it will help Internet
-users choose a DNS resolver that would improve their own Web browsing experience.  
-On the other hand, we would like to obtain general insights about performance 
+users choose a DNS resolver that would improve their own Web browsing experience. On the 
+other hand, we would like to obtain general insights about performance 
 of DNS resolution infrastructures, which may lead to improvements of the Internet 
 for everybody. For the latter purpose, the DNS Explorer will send the result 
 of the measurement to us. No personally identifiable information is collected 
 or accessed by the application -- only the public IP address and the performance metrics. You can disable this 
 functionality by typing `NO` to the corresponding prompt during the application 
-execution; however, we hope you choose to participate in this crowdsources data collection 
+execution; however, we hope you choose to participate in this crowdsourced data collection 
 in recognition of our effort in creating this application.
```

### Comparing `ldns-explorer-1.2/README.md` & `ldns-explorer-1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 1.1.1.1
 ```
 
 
 ## Disclaimer
 
 The purpose of this project is twofold. On one hand, we hope it will help Internet
-users choose a DNS resolver that would improve their own Web browsing experience.  
-On the other hand, we would like to obtain general insights about performance 
+users choose a DNS resolver that would improve their own Web browsing experience. On the 
+other hand, we would like to obtain general insights about performance 
 of DNS resolution infrastructures, which may lead to improvements of the Internet 
 for everybody. For the latter purpose, the DNS Explorer will send the result 
 of the measurement to us. No personally identifiable information is collected 
 or accessed by the application -- only the public IP address and the performance metrics. You can disable this 
 functionality by typing `NO` to the corresponding prompt during the application 
-execution; however, we hope you choose to participate in this crowdsources data collection 
+execution; however, we hope you choose to participate in this crowdsourced data collection 
 in recognition of our effort in creating this application.
```

### Comparing `ldns-explorer-1.2/src/ldns_explorer.egg-info/PKG-INFO` & `ldns-explorer-1.3/src/ldns_explorer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldns-explorer
-Version: 1.2
+Version: 1.3
 Summary: A public DNS resolver explorer
 Author: cwru
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
@@ -58,17 +58,17 @@
 1.1.1.1
 ```
 
 
 ## Disclaimer
 
 The purpose of this project is twofold. On one hand, we hope it will help Internet
-users choose a DNS resolver that would improve their own Web browsing experience.  
-On the other hand, we would like to obtain general insights about performance 
+users choose a DNS resolver that would improve their own Web browsing experience. On the 
+other hand, we would like to obtain general insights about performance 
 of DNS resolution infrastructures, which may lead to improvements of the Internet 
 for everybody. For the latter purpose, the DNS Explorer will send the result 
 of the measurement to us. No personally identifiable information is collected 
 or accessed by the application -- only the public IP address and the performance metrics. You can disable this 
 functionality by typing `NO` to the corresponding prompt during the application 
-execution; however, we hope you choose to participate in this crowdsources data collection 
+execution; however, we hope you choose to participate in this crowdsourced data collection 
 in recognition of our effort in creating this application.
```

### Comparing `ldns-explorer-1.2/src/ldnsexplorer/DNS_APP.py` & `ldns-explorer-1.3/src/ldnsexplorer/DNS_APP.py`

 * *Files identical despite different names*

### Comparing `ldns-explorer-1.2/src/ldnsexplorer/measure_dns.py` & `ldns-explorer-1.3/src/ldnsexplorer/measure_dns.py`

 * *Files identical despite different names*

### Comparing `ldns-explorer-1.2/src/ldnsexplorer/tcp_client.py` & `ldns-explorer-1.3/src/ldnsexplorer/tcp_client.py`

 * *Files identical despite different names*

