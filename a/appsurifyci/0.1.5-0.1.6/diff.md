# Comparing `tmp/appsurifyci-0.1.5.tar.gz` & `tmp/appsurifyci-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appsurifyci-0.1.5.tar", last modified: Wed Mar 15 21:25:43 2023, max compression
+gzip compressed data, was "appsurifyci-0.1.6.tar", last modified: Tue Apr 11 09:33:51 2023, max compression
```

## Comparing `appsurifyci-0.1.5.tar` & `appsurifyci-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-03-15 21:25:43.959269 appsurifyci-0.1.5/
--rw-rw-rw-   0        0        0     2021 2022-11-03 08:45:50.000000 appsurifyci-0.1.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1060 2021-03-19 06:30:43.000000 appsurifyci-0.1.5/LICENCE.txt
--rw-rw-rw-   0        0        0       32 2021-03-19 06:30:43.000000 appsurifyci-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6077 2023-03-15 21:25:43.957736 appsurifyci-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3468 2022-05-18 03:22:21.000000 appsurifyci-0.1.5/README.md
--rw-rw-rw-   0        0        0        8 2021-03-19 06:30:43.000000 appsurifyci-0.1.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-03-15 21:25:43.939862 appsurifyci-0.1.5/appsurifyci/
--rw-rw-rw-   0        0        0    38247 2022-12-16 20:07:42.000000 appsurifyci-0.1.5/appsurifyci/GitToAppsurify.py
--rw-rw-rw-   0        0        0    37851 2022-10-28 20:12:12.000000 appsurifyci-0.1.5/appsurifyci/GitToAppsurifyDev.py
--rw-rw-rw-   0        0        0   124785 2023-03-15 20:06:23.000000 appsurifyci-0.1.5/appsurifyci/RunTestsWithAppsurify3.py
--rw-rw-rw-   0        0        0   103616 2022-11-16 08:17:51.000000 appsurifyci-0.1.5/appsurifyci/RunTestsWithAppsurifyDev.py
--rw-rw-rw-   0        0        0        0 2021-03-19 06:30:43.000000 appsurifyci-0.1.5/appsurifyci/__init__.py
--rw-rw-rw-   0        0        0     6159 2023-03-15 20:06:40.000000 appsurifyci-0.1.5/appsurifyci/appsurifytests.txt
--rw-rw-rw-   0        0        0      286 2023-03-15 19:43:54.000000 appsurifyci-0.1.5/appsurifyci/testpython.py
--rw-rw-rw-   0        0        0      396 2022-08-12 01:27:20.000000 appsurifyci-0.1.5/appsurifyci/trxcpnvert.py
-drwxrwxrwx   0        0        0        0 2023-03-15 21:25:43.957736 appsurifyci-0.1.5/appsurifyci.egg-info/
--rw-rw-rw-   0        0        0     6077 2023-03-15 21:25:43.000000 appsurifyci-0.1.5/appsurifyci.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2023-03-15 21:25:43.000000 appsurifyci-0.1.5/appsurifyci.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-15 21:25:43.000000 appsurifyci-0.1.5/appsurifyci.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-03-15 21:25:43.000000 appsurifyci-0.1.5/appsurifyci.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-03-15 21:25:43.000000 appsurifyci-0.1.5/appsurifyci.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-15 21:25:43.000000 appsurifyci-0.1.5/appsurifyci.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-15 21:25:43.959780 appsurifyci-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1011 2023-03-15 21:24:50.000000 appsurifyci-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:33:51.713268 appsurifyci-0.1.6/
+-rw-rw-rw-   0        0        0     2021 2022-11-03 08:45:50.000000 appsurifyci-0.1.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1060 2021-03-19 06:30:43.000000 appsurifyci-0.1.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       32 2021-03-19 06:30:43.000000 appsurifyci-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6077 2023-04-11 09:33:51.713268 appsurifyci-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3468 2022-05-18 03:22:21.000000 appsurifyci-0.1.6/README.md
+-rw-rw-rw-   0        0        0        8 2021-03-19 06:30:43.000000 appsurifyci-0.1.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 09:33:51.689413 appsurifyci-0.1.6/appsurifyci/
+-rw-rw-rw-   0        0        0    38529 2023-04-11 09:32:22.000000 appsurifyci-0.1.6/appsurifyci/GitToAppsurify.py
+-rw-rw-rw-   0        0        0    37851 2022-10-28 20:12:12.000000 appsurifyci-0.1.6/appsurifyci/GitToAppsurifyDev.py
+-rw-rw-rw-   0        0        0   124785 2023-03-15 20:06:23.000000 appsurifyci-0.1.6/appsurifyci/RunTestsWithAppsurify3.py
+-rw-rw-rw-   0        0        0   103616 2022-11-16 08:17:51.000000 appsurifyci-0.1.6/appsurifyci/RunTestsWithAppsurifyDev.py
+-rw-rw-rw-   0        0        0        0 2021-03-19 06:30:43.000000 appsurifyci-0.1.6/appsurifyci/__init__.py
+-rw-rw-rw-   0        0        0     6159 2023-03-15 20:06:40.000000 appsurifyci-0.1.6/appsurifyci/appsurifytests.txt
+-rw-rw-rw-   0        0        0      286 2023-03-15 19:43:54.000000 appsurifyci-0.1.6/appsurifyci/testpython.py
+-rw-rw-rw-   0        0        0      396 2022-08-12 01:27:20.000000 appsurifyci-0.1.6/appsurifyci/trxcpnvert.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:33:51.712269 appsurifyci-0.1.6/appsurifyci.egg-info/
+-rw-rw-rw-   0        0        0     6077 2023-04-11 09:33:51.000000 appsurifyci-0.1.6/appsurifyci.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2023-04-11 09:33:51.000000 appsurifyci-0.1.6/appsurifyci.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 09:33:51.000000 appsurifyci-0.1.6/appsurifyci.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-04-11 09:33:51.000000 appsurifyci-0.1.6/appsurifyci.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-04-11 09:33:51.000000 appsurifyci-0.1.6/appsurifyci.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-11 09:33:51.000000 appsurifyci-0.1.6/appsurifyci.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 09:33:51.714315 appsurifyci-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1011 2023-04-11 09:33:11.000000 appsurifyci-0.1.6/setup.py
```

### Comparing `appsurifyci-0.1.5/CHANGELOG.txt` & `appsurifyci-0.1.6/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.5/LICENCE.txt` & `appsurifyci-0.1.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.5/PKG-INFO` & `appsurifyci-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appsurifyci
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package used to run tests using Appsurify
 Home-page: https://appsurify.com
 Author: James Farrier
 Author-email: jamesfarrier@appsurify.com
 License: MIT
 Keywords: appsurify
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `appsurifyci-0.1.5/README.md` & `appsurifyci-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.5/appsurifyci/GitToAppsurify.py` & `appsurifyci-0.1.6/appsurifyci/GitToAppsurify.py`

 * *Files 2% similar despite different names*

```diff
@@ -705,31 +705,28 @@
     return result
 
 
 def get_project_id(base_url, project_name, token):
     url = base_url + '/api/ssh_v2/hook/fetch/?project_name={}'.format(project_name)
     headers = {"Content-Type": "application/json",
                 "token": token}
-
     session = Session()
     session.mount('http://', HTTPAdapter(max_retries=3))
     session.mount('https://', HTTPAdapter(max_retries=3))
 
     resp = session.get(url=url, headers=headers, verify=False, allow_redirects=True)
-
     if resp.status_code == 200:
         return resp.json()
-
     if resp.status_code == 401:
         logging.debug('Could not verify your token, please check it and try again.')
         # sys.exit(1)
         raise Exception('Could not verify your token, please check it and try again.')
 
     if resp.status_code != 200:
-        logging.debug('Can\'t not get a connection to the server, please check your url or token and try again.')
+        logging.debug('Can\'t not get a connection to the server, please check your url or token and try again. Http status {}'.format(resp.status_code))
         # sys.exit(1)
         raise Exception('Can\'t not get a connection to the server, please check your url or token and try again.')
 
 def get_commit_branch(sha):
     branch_list = list()
     output = execute(COMMAND_COMMIT_BRANCH.format(sha))
 
@@ -1167,39 +1164,42 @@
                     help='Write data of commits to json file')
 parser.add_argument('--repo_name', type=str, required=False, default='',
                     help='Define repository name')
 parser.add_argument('--auto_repo_name', action='store_true', default=False,
                     help='Use Git remote as repository name.')
 
 args = parser.parse_args()
-
 base_url = args.url.rstrip('/')
 project = args.project
 token = args.token
 start = args.start
 number = args.number if args.number else 100
 branch = args.branch
 blame = args.blame
 debug = args.debug
+if debug:
+    logging.info('Setting debug')
+    logging.getLogger().setLevel(logging.DEBUG)
+    for handler in logging.getLogger().handlers:
+        handler.setLevel(logging.DEBUG)
 debug = True
 
 repo_name = args.repo_name
 auto_repo_name = args.auto_repo_name
-
 if auto_repo_name:
     REPOSITORY_NAME = get_repo_name()
 else:
     REPOSITORY_NAME = repo_name
-
+logging.debug('Finding project id')
 
 try:
     project_id_data = get_project_id(base_url=base_url, project_name=project, token=token)
 except Exception as exc:
     sys.exit(1)
-
+logging.debug('Project id set')
 
 if 'project_id' in project_id_data:
     project_id = project_id_data['project_id']
     url = base_url + '/api/ssh_v2/hook/{}/'.format(project_id)
 elif 'error' in project_id_data:
     logging.debug('Project not found')
     sys.exit(1)
```

### Comparing `appsurifyci-0.1.5/appsurifyci/GitToAppsurifyDev.py` & `appsurifyci-0.1.6/appsurifyci/GitToAppsurifyDev.py`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.5/appsurifyci/RunTestsWithAppsurify3.py` & `appsurifyci-0.1.6/appsurifyci/RunTestsWithAppsurify3.py`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.5/appsurifyci/RunTestsWithAppsurifyDev.py` & `appsurifyci-0.1.6/appsurifyci/RunTestsWithAppsurifyDev.py`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.5/appsurifyci/appsurifytests.txt` & `appsurifyci-0.1.6/appsurifyci/appsurifytests.txt`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.5/appsurifyci.egg-info/PKG-INFO` & `appsurifyci-0.1.6/appsurifyci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appsurifyci
-Version: 0.1.5
+Version: 0.1.6
 Summary: Package used to run tests using Appsurify
 Home-page: https://appsurify.com
 Author: James Farrier
 Author-email: jamesfarrier@appsurify.com
 License: MIT
 Keywords: appsurify
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `appsurifyci-0.1.5/appsurifyci.egg-info/SOURCES.txt` & `appsurifyci-0.1.6/appsurifyci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appsurifyci-0.1.5/setup.py` & `appsurifyci-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='appsurifyci',
-  version='0.1.5',
+  version='0.1.6',
   description='Package used to run tests using Appsurify',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://appsurify.com',  
   author='James Farrier',
   author_email='jamesfarrier@appsurify.com',
   license='MIT',
```

