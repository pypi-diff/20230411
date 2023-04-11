# Comparing `tmp/certbot-dns-e2econfig-0.4.8.tar.gz` & `tmp/certbot-dns-e2econfig-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-e2econfig-0.4.8.tar", last modified: Thu Apr  6 09:36:33 2023, max compression
+gzip compressed data, was "certbot-dns-e2econfig-0.4.9.tar", last modified: Tue Apr 11 06:11:29 2023, max compression
```

## Comparing `certbot-dns-e2econfig-0.4.8.tar` & `certbot-dns-e2econfig-0.4.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 abhaybhati   (501) staff       (20)        0 2023-04-06 09:36:33.557247 certbot-dns-e2econfig-0.4.8/
--rw-r--r--   0 abhaybhati   (501) staff       (20)    10786 2023-04-03 06:46:44.000000 certbot-dns-e2econfig-0.4.8/LICENSE.txt
--rw-r--r--   0 abhaybhati   (501) staff       (20)     7200 2023-04-06 09:36:33.557337 certbot-dns-e2econfig-0.4.8/PKG-INFO
--rw-r--r--   0 abhaybhati   (501) staff       (20)     4898 2023-04-03 06:46:44.000000 certbot-dns-e2econfig-0.4.8/README.rst
-drwxr-xr-x   0 abhaybhati   (501) staff       (20)        0 2023-04-06 09:36:33.556335 certbot-dns-e2econfig-0.4.8/certbot_dns_e2econfig/
--rw-r--r--   0 abhaybhati   (501) staff       (20)     3271 2023-04-05 12:55:09.000000 certbot-dns-e2econfig-0.4.8/certbot_dns_e2econfig/__init__.py
--rw-r--r--   0 abhaybhati   (501) staff       (20)     8485 2023-04-06 09:35:36.000000 certbot-dns-e2econfig-0.4.8/certbot_dns_e2econfig/dns_e2econfig.py
-drwxr-xr-x   0 abhaybhati   (501) staff       (20)        0 2023-04-06 09:36:33.557160 certbot-dns-e2econfig-0.4.8/certbot_dns_e2econfig.egg-info/
--rw-r--r--   0 abhaybhati   (501) staff       (20)     7200 2023-04-06 09:36:33.000000 certbot-dns-e2econfig-0.4.8/certbot_dns_e2econfig.egg-info/PKG-INFO
--rw-r--r--   0 abhaybhati   (501) staff       (20)      386 2023-04-06 09:36:33.000000 certbot-dns-e2econfig-0.4.8/certbot_dns_e2econfig.egg-info/SOURCES.txt
--rw-r--r--   0 abhaybhati   (501) staff       (20)        1 2023-04-06 09:36:33.000000 certbot-dns-e2econfig-0.4.8/certbot_dns_e2econfig.egg-info/dependency_links.txt
--rw-r--r--   0 abhaybhati   (501) staff       (20)       85 2023-04-06 09:36:33.000000 certbot-dns-e2econfig-0.4.8/certbot_dns_e2econfig.egg-info/entry_points.txt
--rw-r--r--   0 abhaybhati   (501) staff       (20)       79 2023-04-06 09:36:33.000000 certbot-dns-e2econfig-0.4.8/certbot_dns_e2econfig.egg-info/requires.txt
--rw-r--r--   0 abhaybhati   (501) staff       (20)       22 2023-04-06 09:36:33.000000 certbot-dns-e2econfig-0.4.8/certbot_dns_e2econfig.egg-info/top_level.txt
--rw-r--r--   0 abhaybhati   (501) staff       (20)       67 2023-04-06 09:36:33.557545 certbot-dns-e2econfig-0.4.8/setup.cfg
--rw-r--r--   0 abhaybhati   (501) staff       (20)     1994 2023-04-06 09:35:42.000000 certbot-dns-e2econfig-0.4.8/setup.py
+drwxr-xr-x   0 abhaybhati   (501) staff       (20)        0 2023-04-11 06:11:29.780796 certbot-dns-e2econfig-0.4.9/
+-rw-r--r--   0 abhaybhati   (501) staff       (20)    10786 2023-04-03 06:46:44.000000 certbot-dns-e2econfig-0.4.9/LICENSE.txt
+-rw-r--r--   0 abhaybhati   (501) staff       (20)     7200 2023-04-11 06:11:29.780889 certbot-dns-e2econfig-0.4.9/PKG-INFO
+-rw-r--r--   0 abhaybhati   (501) staff       (20)     4898 2023-04-03 06:46:44.000000 certbot-dns-e2econfig-0.4.9/README.rst
+drwxr-xr-x   0 abhaybhati   (501) staff       (20)        0 2023-04-11 06:11:29.779958 certbot-dns-e2econfig-0.4.9/certbot_dns_e2econfig/
+-rw-r--r--   0 abhaybhati   (501) staff       (20)     3271 2023-04-05 12:55:09.000000 certbot-dns-e2econfig-0.4.9/certbot_dns_e2econfig/__init__.py
+-rw-r--r--   0 abhaybhati   (501) staff       (20)     8580 2023-04-11 06:09:20.000000 certbot-dns-e2econfig-0.4.9/certbot_dns_e2econfig/dns_e2econfig.py
+drwxr-xr-x   0 abhaybhati   (501) staff       (20)        0 2023-04-11 06:11:29.780688 certbot-dns-e2econfig-0.4.9/certbot_dns_e2econfig.egg-info/
+-rw-r--r--   0 abhaybhati   (501) staff       (20)     7200 2023-04-11 06:11:29.000000 certbot-dns-e2econfig-0.4.9/certbot_dns_e2econfig.egg-info/PKG-INFO
+-rw-r--r--   0 abhaybhati   (501) staff       (20)      386 2023-04-11 06:11:29.000000 certbot-dns-e2econfig-0.4.9/certbot_dns_e2econfig.egg-info/SOURCES.txt
+-rw-r--r--   0 abhaybhati   (501) staff       (20)        1 2023-04-11 06:11:29.000000 certbot-dns-e2econfig-0.4.9/certbot_dns_e2econfig.egg-info/dependency_links.txt
+-rw-r--r--   0 abhaybhati   (501) staff       (20)       85 2023-04-11 06:11:29.000000 certbot-dns-e2econfig-0.4.9/certbot_dns_e2econfig.egg-info/entry_points.txt
+-rw-r--r--   0 abhaybhati   (501) staff       (20)       79 2023-04-11 06:11:29.000000 certbot-dns-e2econfig-0.4.9/certbot_dns_e2econfig.egg-info/requires.txt
+-rw-r--r--   0 abhaybhati   (501) staff       (20)       22 2023-04-11 06:11:29.000000 certbot-dns-e2econfig-0.4.9/certbot_dns_e2econfig.egg-info/top_level.txt
+-rw-r--r--   0 abhaybhati   (501) staff       (20)       67 2023-04-11 06:11:29.781116 certbot-dns-e2econfig-0.4.9/setup.cfg
+-rw-r--r--   0 abhaybhati   (501) staff       (20)     1994 2023-04-11 06:09:44.000000 certbot-dns-e2econfig-0.4.9/setup.py
```

### Comparing `certbot-dns-e2econfig-0.4.8/LICENSE.txt` & `certbot-dns-e2econfig-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-e2econfig-0.4.8/PKG-INFO` & `certbot-dns-e2econfig-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-e2econfig
-Version: 0.4.8
+Version: 0.4.9
 Summary: E2E DNS Authenticator plugin for Certbot
 Home-page: UNKNOWN
 Author: Abhay Bhati
 Author-email: abhaybhati987@gmail.com
 License: Apache License 2.0
 Description: certbot-dns-ispconfig
         =====================
```

### Comparing `certbot-dns-e2econfig-0.4.8/README.rst` & `certbot-dns-e2econfig-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-e2econfig-0.4.8/certbot_dns_e2econfig/__init__.py` & `certbot-dns-e2econfig-0.4.9/certbot_dns_e2econfig/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-e2econfig-0.4.8/certbot_dns_e2econfig/dns_e2econfig.py` & `certbot-dns-e2econfig-0.4.9/certbot_dns_e2econfig/dns_e2econfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,18 @@
             hint = 'Did you provide a valid API token?'  
             
             logger.debug('Error finding domain using the e2e_client API')
             raise errors.PluginError('Error finding domain using the e2e_client API: {0}'
                                      .format(e))
 
         try:
+            domain = self._find_managed_zone_id(domain_name=domain, zone_name=domain, record_name=record_name, record_ttl=record_ttl, record_type='TXT', content=record_content, api_key=self.api_key, api_token=self.api_token)
+            if not domain.endswith('.'):
+                domain += '.'
             Domain(domain_name=domain, zone_name=domain, record_name=record_name, record_ttl=record_ttl, record_type='TXT', content=record_content, api_key=self.api_key, api_token=self.api_token).check_domain_valid()
-            self._find_managed_zone_id(domain_name=domain, zone_name=domain, record_name=record_name, record_ttl=record_ttl, record_type='TXT', content=record_content, api_key=self.api_key, api_token=self.api_token)
         except DomainException as e: 
             hint = 'Did you provide a correct Domain Name?'  
             
             logger.debug('Error finding domain using the e2e_client API')
             raise errors.PluginError('Error finding domain using the e2e_client API: {0}'
                                      .format(e)) 
 
@@ -177,11 +179,11 @@
             # get the zone id
                 logger.debug("looking for zone: %s", zone_name)
                 matches = [domain for domain in domains if domain['domain_name'] == zone_name]
 
                 if matches:
                     domain = matches[0]
                     logger.debug('Found base domain for %s using name %s', domain_name, zone_name)
-                    return domain      
+                    return domain['domain_name']
```

### Comparing `certbot-dns-e2econfig-0.4.8/certbot_dns_e2econfig.egg-info/PKG-INFO` & `certbot-dns-e2econfig-0.4.9/certbot_dns_e2econfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-e2econfig
-Version: 0.4.8
+Version: 0.4.9
 Summary: E2E DNS Authenticator plugin for Certbot
 Home-page: UNKNOWN
 Author: Abhay Bhati
 Author-email: abhaybhati987@gmail.com
 License: Apache License 2.0
 Description: certbot-dns-ispconfig
         =====================
```

### Comparing `certbot-dns-e2econfig-0.4.8/setup.py` & `certbot-dns-e2econfig-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from setuptools import find_packages
 
-version = "0.4.8"
+version = "0.4.9"
 install_requires = [
     "acme>=0.29.0",
     "certbot>=0.34.0",
     "setuptools",
     "requests",
     "mock",
     "requests-mock",
```

