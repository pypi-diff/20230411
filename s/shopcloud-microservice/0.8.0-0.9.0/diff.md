# Comparing `tmp/shopcloud-microservice-0.8.0.tar.gz` & `tmp/shopcloud-microservice-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopcloud-microservice-0.8.0.tar", last modified: Sun Mar  5 08:23:53 2023, max compression
+gzip compressed data, was "shopcloud-microservice-0.9.0.tar", last modified: Mon Mar  6 06:51:10 2023, max compression
```

## Comparing `shopcloud-microservice-0.8.0.tar` & `shopcloud-microservice-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 08:23:52.995983 shopcloud-microservice-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-05 08:23:28.000000 shopcloud-microservice-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-05 08:23:52.995983 shopcloud-microservice-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-05 08:23:28.000000 shopcloud-microservice-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-05 08:23:28.000000 shopcloud-microservice-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 08:23:52.995983 shopcloud-microservice-0.8.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-05 08:23:28.000000 shopcloud-microservice-0.8.0/scripts/microservice
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 08:23:52.995983 shopcloud-microservice-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-05 08:23:28.000000 shopcloud-microservice-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 08:23:52.995983 shopcloud-microservice-0.8.0/shopcloud_microservice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 08:23:28.000000 shopcloud-microservice-0.8.0/shopcloud_microservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-05 08:23:28.000000 shopcloud-microservice-0.8.0/shopcloud_microservice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-05 08:23:28.000000 shopcloud-microservice-0.8.0/shopcloud_microservice/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-05 08:23:28.000000 shopcloud-microservice-0.8.0/shopcloud_microservice/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-05 08:23:28.000000 shopcloud-microservice-0.8.0/shopcloud_microservice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-05 08:23:28.000000 shopcloud-microservice-0.8.0/shopcloud_microservice/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-03-05 08:23:28.000000 shopcloud-microservice-0.8.0/shopcloud_microservice/security.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-03-05 08:23:28.000000 shopcloud-microservice-0.8.0/shopcloud_microservice/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 08:23:52.995983 shopcloud-microservice-0.8.0/shopcloud_microservice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-05 08:23:52.000000 shopcloud-microservice-0.8.0/shopcloud_microservice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-05 08:23:52.000000 shopcloud-microservice-0.8.0/shopcloud_microservice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 08:23:52.000000 shopcloud-microservice-0.8.0/shopcloud_microservice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-05 08:23:52.000000 shopcloud-microservice-0.8.0/shopcloud_microservice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-05 08:23:52.000000 shopcloud-microservice-0.8.0/shopcloud_microservice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 06:51:10.976120 shopcloud-microservice-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-06 06:51:10.976120 shopcloud-microservice-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 06:51:10.972120 shopcloud-microservice-0.9.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/scripts/microservice
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 06:51:10.976120 shopcloud-microservice-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 06:51:10.972120 shopcloud-microservice-0.9.0/shopcloud_microservice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/shopcloud_microservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/shopcloud_microservice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/shopcloud_microservice/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/shopcloud_microservice/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/shopcloud_microservice/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/shopcloud_microservice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/shopcloud_microservice/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/shopcloud_microservice/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-03-06 06:50:47.000000 shopcloud-microservice-0.9.0/shopcloud_microservice/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 06:51:10.976120 shopcloud-microservice-0.9.0/shopcloud_microservice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-06 06:51:10.000000 shopcloud-microservice-0.9.0/shopcloud_microservice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-06 06:51:10.000000 shopcloud-microservice-0.9.0/shopcloud_microservice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 06:51:10.000000 shopcloud-microservice-0.9.0/shopcloud_microservice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-06 06:51:10.000000 shopcloud-microservice-0.9.0/shopcloud_microservice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-06 06:51:10.000000 shopcloud-microservice-0.9.0/shopcloud_microservice.egg-info/top_level.txt
```

### Comparing `shopcloud-microservice-0.8.0/LICENSE` & `shopcloud-microservice-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shopcloud-microservice-0.8.0/PKG-INFO` & `shopcloud-microservice-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopcloud-microservice
-Version: 0.8.0
+Version: 0.9.0
 Summary: CLI tool for manage microservices
 Home-page: https://github.com/Talk-Point/shopcloud-microservice-cli
 Author: Konstantin Stoldt
 Author-email: konstantin.stoldt@talk-point.de
 License: MIT
 Keywords: CLI
 Description-Content-Type: text/markdown
```

### Comparing `shopcloud-microservice-0.8.0/setup.py` & `shopcloud-microservice-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = {
     "name": 'shopcloud-microservice',
-    "version": '0.8.0',
+    "version": '0.9.0',
     "description": 'CLI tool for manage microservices',
     "long_description_content_type": "text/markdown",
     "long_description": README,
     "license": 'MIT',
     "packages": find_packages(),
     "author": 'Konstantin Stoldt',
     "author_email": 'konstantin.stoldt@talk-point.de',
```

### Comparing `shopcloud-microservice-0.8.0/shopcloud_microservice/__main__.py` & `shopcloud-microservice-0.9.0/shopcloud_microservice/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,27 +7,38 @@
     parser = argparse.ArgumentParser(
         description='Microservice management',
         prog='shopcloud-microservice'
     )
 
     subparsers = parser.add_subparsers(help='commands', title='commands')
     parser.add_argument('--debug', '-d', help='Debug', action='store_true')
+    parser.add_argument('--quit', '-q', help='Quiet', action='store_true')
     parser.add_argument('--simulate', '-s', help='Simulate the process', action='store_true')
     parser.add_argument('--secrethub-token', help='Secrethub-Token', type=str)
 
     parser_security = subparsers.add_parser('security', help='security')
     parser_security.add_argument(
         'action',
         const='generate',
         nargs='?',
-        choices=['merge-security-pull-requests', 'scan-code', 'scan-cloud']
+        choices=['merge-security-pull-requests']
     )
     parser_security.add_argument('repo', const='generate', nargs='?')
     parser_security.set_defaults(which='security')
 
+    parser_audit = subparsers.add_parser('audit', help='audit')
+    parser_audit.add_argument(
+        'action',
+        const='generate',
+        nargs='?',
+        choices=['code', 'cloud', 'app']
+    )
+    parser_audit.add_argument('repo', const='generate', nargs='?')
+    parser_audit.set_defaults(which='audit')
+
     args = parser.parse_args()
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit(1)
     rc = cli.main(args)
     if rc != 0:
         sys.exit(rc)
```

### Comparing `shopcloud-microservice-0.8.0/shopcloud_microservice/configs.py` & `shopcloud-microservice-0.9.0/shopcloud_microservice/configs.py`

 * *Files identical despite different names*

### Comparing `shopcloud-microservice-0.8.0/shopcloud_microservice/helpers.py` & `shopcloud-microservice-0.9.0/shopcloud_microservice/helpers.py`

 * *Files identical despite different names*

### Comparing `shopcloud-microservice-0.8.0/shopcloud_microservice/security.py` & `shopcloud-microservice-0.9.0/shopcloud_microservice/security.py`

 * *Files 10% similar despite different names*

```diff
@@ -158,33 +158,9 @@
         api_token = get_api_token(is_simulate=args.simulate)
 
         with parallel_backend('threading', n_jobs=-1):
             Parallel()(
                 delayed(run_repo_merge_security_pull_requests)(owner, m, is_simulate=args.simulate, api_token=api_token)
                 for m in repos
             )
-    elif args.action == 'scan-code':
-        dirpath = tempfile.mkdtemp()
-
-        print(f'cd {dirpath}')
-        print('git clone https://github.com/Talk-Point/semgrep-rules')
-        print('git clone <repo>')
-        print('cd <repo>')
-        print('pip install semgrep')
-        print('semgrep --config ../semgrep-rules/')
-        print('semgrep --config auto')
-        print('npm install -g observatory-cli')
-        print('observatory <hostname> --format=report')
-
-        input("Ready for cleanup? (y/n) ")
-        shutil.rmtree(dirpath)
-    elif args.action == 'scan-cloud':
-        dirpath = tempfile.mkdtemp()
-
-        print(f'pip3 install scoutsuite')
-        print(f'gcloud config set project shopcloud-worktable')
-        print(f'scout gcp -u')
-
-        input("Ready for cleanup? (y/n) ")
-        shutil.rmtree(dirpath)
 
     return 0
```

### Comparing `shopcloud-microservice-0.8.0/shopcloud_microservice/steps.py` & `shopcloud-microservice-0.9.0/shopcloud_microservice/steps.py`

 * *Files identical despite different names*

### Comparing `shopcloud-microservice-0.8.0/shopcloud_microservice.egg-info/PKG-INFO` & `shopcloud-microservice-0.9.0/shopcloud_microservice.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shopcloud-microservice
-Version: 0.8.0
+Version: 0.9.0
 Summary: CLI tool for manage microservices
 Home-page: https://github.com/Talk-Point/shopcloud-microservice-cli
 Author: Konstantin Stoldt
 Author-email: konstantin.stoldt@talk-point.de
 License: MIT
 Keywords: CLI
 Description-Content-Type: text/markdown
```

### Comparing `shopcloud-microservice-0.8.0/shopcloud_microservice.egg-info/SOURCES.txt` & `shopcloud-microservice-0.9.0/shopcloud_microservice.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 ./scripts/microservice
 shopcloud_microservice/__init__.py
 shopcloud_microservice/__main__.py
+shopcloud_microservice/audit.py
 shopcloud_microservice/cli.py
 shopcloud_microservice/configs.py
 shopcloud_microservice/exceptions.py
 shopcloud_microservice/helpers.py
 shopcloud_microservice/security.py
 shopcloud_microservice/steps.py
 shopcloud_microservice.egg-info/PKG-INFO
```

