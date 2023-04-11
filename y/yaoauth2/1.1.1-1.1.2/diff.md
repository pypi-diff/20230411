# Comparing `tmp/yaoauth2-1.1.1.tar.gz` & `tmp/yaoauth2-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaoauth2-1.1.1.tar", max compression
+gzip compressed data, was "yaoauth2-1.1.2.tar", max compression
```

## Comparing `yaoauth2-1.1.1.tar` & `yaoauth2-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      441 2023-02-22 18:13:21.148102 yaoauth2-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      221 2022-01-31 13:39:29.535603 yaoauth2-1.1.1/yaoauth2/__init__.py
--rw-r--r--   0        0        0     1417 2023-02-17 14:46:23.547328 yaoauth2-1.1.1/yaoauth2/config.py
--rw-r--r--   0        0        0     4560 2023-02-22 18:12:38.836441 yaoauth2-1.1.1/yaoauth2/endpoints.py
--rw-r--r--   0        0        0     2605 2023-02-17 14:45:22.224043 yaoauth2-1.1.1/yaoauth2/models.py
--rw-r--r--   0        0        0      190 2022-01-28 13:10:26.040600 yaoauth2-1.1.1/yaoauth2/providers/__init__.py
--rw-r--r--   0        0        0     1003 2023-02-17 14:43:52.501122 yaoauth2-1.1.1/yaoauth2/providers/discord.py
--rw-r--r--   0        0        0      949 2023-02-17 14:43:52.509122 yaoauth2-1.1.1/yaoauth2/providers/google.py
--rw-r--r--   0        0        0     3355 2023-02-17 14:47:59.606239 yaoauth2-1.1.1/yaoauth2/router.py
--rw-r--r--   0        0        0      960 2022-03-18 14:26:06.247978 yaoauth2-1.1.1/yaoauth2/utils.py
--rw-r--r--   0        0        0      684 2023-02-22 18:13:55.581032 yaoauth2-1.1.1/setup.py
--rw-r--r--   0        0        0      390 2023-02-22 18:13:55.581238 yaoauth2-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      446 2023-04-11 07:13:42.024092 yaoauth2-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      221 2022-01-31 13:39:29.535603 yaoauth2-1.1.2/yaoauth2/__init__.py
+-rw-r--r--   0        0        0     1417 2023-02-17 14:46:23.547328 yaoauth2-1.1.2/yaoauth2/config.py
+-rw-r--r--   0        0        0     4560 2023-02-22 18:12:38.836441 yaoauth2-1.1.2/yaoauth2/endpoints.py
+-rw-r--r--   0        0        0     2605 2023-02-17 14:45:22.224043 yaoauth2-1.1.2/yaoauth2/models.py
+-rw-r--r--   0        0        0      190 2022-01-28 13:10:26.040600 yaoauth2-1.1.2/yaoauth2/providers/__init__.py
+-rw-r--r--   0        0        0     1003 2023-02-17 14:43:52.501122 yaoauth2-1.1.2/yaoauth2/providers/discord.py
+-rw-r--r--   0        0        0      949 2023-02-17 14:43:52.509122 yaoauth2-1.1.2/yaoauth2/providers/google.py
+-rw-r--r--   0        0        0     3355 2023-02-17 14:47:59.606239 yaoauth2-1.1.2/yaoauth2/router.py
+-rw-r--r--   0        0        0      960 2022-03-18 14:26:06.247978 yaoauth2-1.1.2/yaoauth2/utils.py
+-rw-r--r--   0        0        0      682 2023-04-11 07:14:04.713726 yaoauth2-1.1.2/setup.py
+-rw-r--r--   0        0        0      388 2023-04-11 07:14:04.714066 yaoauth2-1.1.2/PKG-INFO
```

### Comparing `yaoauth2-1.1.1/yaoauth2/config.py` & `yaoauth2-1.1.2/yaoauth2/config.py`

 * *Files identical despite different names*

### Comparing `yaoauth2-1.1.1/yaoauth2/endpoints.py` & `yaoauth2-1.1.2/yaoauth2/endpoints.py`

 * *Files identical despite different names*

### Comparing `yaoauth2-1.1.1/yaoauth2/models.py` & `yaoauth2-1.1.2/yaoauth2/models.py`

 * *Files identical despite different names*

### Comparing `yaoauth2-1.1.1/yaoauth2/providers/discord.py` & `yaoauth2-1.1.2/yaoauth2/providers/discord.py`

 * *Files identical despite different names*

### Comparing `yaoauth2-1.1.1/yaoauth2/providers/google.py` & `yaoauth2-1.1.2/yaoauth2/providers/google.py`

 * *Files identical despite different names*

### Comparing `yaoauth2-1.1.1/yaoauth2/router.py` & `yaoauth2-1.1.2/yaoauth2/router.py`

 * *Files identical despite different names*

### Comparing `yaoauth2-1.1.1/yaoauth2/utils.py` & `yaoauth2-1.1.2/yaoauth2/utils.py`

 * *Files identical despite different names*

### Comparing `yaoauth2-1.1.1/setup.py` & `yaoauth2-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['yaoauth2', 'yaoauth2.providers']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fastapi>=0.92,<0.93', 'httpx>=0.23,<0.24', 'nxtools>=1.6,<2.0']
+['fastapi>0.92,<1.0', 'httpx>=0.23,<0.24', 'nxtools>=1.6,<2.0']
 
 setup_kwargs = {
     'name': 'yaoauth2',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'Simple OAuth2 client library for FastAPI',
     'long_description': None,
     'author': 'Martin Wacker',
     'author_email': 'martas@imm.cz',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

