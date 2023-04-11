# Comparing `tmp/nvosscript-1.1.5.tar.gz` & `tmp/nvosscript-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.1.5.tar", last modified: Mon Apr 10 11:42:00 2023, max compression
+gzip compressed data, was "nvosscript-1.1.6.tar", last modified: Tue Apr 11 03:34:11 2023, max compression
```

## Comparing `nvosscript-1.1.5.tar` & `nvosscript-1.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 11:42:00.835532 nvosscript-1.1.5/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.1.5/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-10 11:42:00.835392 nvosscript-1.1.5/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.1.5/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 11:42:00.833397 nvosscript-1.1.5/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.1.5/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    12391 2023-04-10 07:03:10.000000 nvosscript-1.1.5/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-06 06:54:07.000000 nvosscript-1.1.5/nvos/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     7331 2023-04-10 10:09:11.000000 nvosscript-1.1.5/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     3524 2023-04-10 09:34:12.000000 nvosscript-1.1.5/nvos/run.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      812 2023-03-30 03:32:22.000000 nvosscript-1.1.5/nvos/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 11:42:00.834502 nvosscript-1.1.5/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-10 11:42:00.000000 nvosscript-1.1.5/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      372 2023-04-10 11:42:00.000000 nvosscript-1.1.5/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-10 11:42:00.000000 nvosscript-1.1.5/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-10 11:42:00.000000 nvosscript-1.1.5/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-04-10 11:42:00.000000 nvosscript-1.1.5/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       21 2023-04-10 11:42:00.000000 nvosscript-1.1.5/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-10 11:42:00.835584 nvosscript-1.1.5/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-04-10 10:14:52.000000 nvosscript-1.1.5/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 11:42:00.834745 nvosscript-1.1.5/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.1.5/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     3480 2023-04-10 10:15:03.000000 nvosscript-1.1.5/start/main.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-10 11:42:00.835058 nvosscript-1.1.5/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1283 2023-04-06 07:02:53.000000 nvosscript-1.1.5/win/win_auto_script.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-11 03:34:11.688730 nvosscript-1.1.6/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.1.6/LICENSE
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-11 03:34:11.688551 nvosscript-1.1.6/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.1.6/README.md
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-11 03:34:11.686565 nvosscript-1.1.6/nvos/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.1.6/nvos/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)    12894 2023-04-11 03:19:59.000000 nvosscript-1.1.6/nvos/file.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-06 06:54:07.000000 nvosscript-1.1.6/nvos/login.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     7331 2023-04-11 03:09:14.000000 nvosscript-1.1.6/nvos/remote.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     4247 2023-04-11 03:24:00.000000 nvosscript-1.1.6/nvos/run.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      812 2023-03-30 03:32:22.000000 nvosscript-1.1.6/nvos/utils.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-11 03:34:11.687634 nvosscript-1.1.6/nvosscript.egg-info/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-11 03:34:11.000000 nvosscript-1.1.6/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      372 2023-04-11 03:34:11.000000 nvosscript-1.1.6/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-11 03:34:11.000000 nvosscript-1.1.6/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-11 03:34:11.000000 nvosscript-1.1.6/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-04-11 03:34:11.000000 nvosscript-1.1.6/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       21 2023-04-11 03:34:11.000000 nvosscript-1.1.6/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-11 03:34:11.688774 nvosscript-1.1.6/setup.cfg
+-rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-04-11 03:24:33.000000 nvosscript-1.1.6/setup.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-11 03:34:11.687871 nvosscript-1.1.6/start/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.1.6/start/__init__.py
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     3480 2023-04-11 03:24:43.000000 nvosscript-1.1.6/start/main.py
+drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-11 03:34:11.688109 nvosscript-1.1.6/win/
+-rw-r--r--   0 andre.zhao   (503) staff       (20)     1283 2023-04-11 01:53:27.000000 nvosscript-1.1.6/win/win_auto_script.py
```

### Comparing `nvosscript-1.1.5/LICENSE` & `nvosscript-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.5/nvos/file.py` & `nvosscript-1.1.6/nvos/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,27 @@
     find_json_config(workspace_path, file_list, project_space_list)
     # 将来可以优化上传文件信息，针对于已经上传过的就不在上传
     with open(os.path.join(nvos_dir, "config"), 'w') as file:
         for item in file_list:
             file.write(json.dumps(item) + "\n")
 
     remote.upload_file(file_list, project_space_list)
+
+    workspace_env = []
+    if os.path.exists(os.path.expanduser(os.path.join("~", "workspace_env"))):
+        with open(os.path.expanduser(os.path.join("~", "workspace_env")), 'r') as f:
+            for line in f:
+                workspace_env.append(line.strip())
+    workspace_env.append(workspace_path)
+    workspace_env = list(set(workspace_env))
+
+    with open(os.path.expanduser(os.path.join("~", "workspace_env")), 'w') as f:
+        for item in workspace_env:
+            f.write(item + "\n")
+
     return True
 
 
 def pull_data_from_cloud(workspace_path):
     sync_project_data(workspace_path)
 
     overwrite_file(workspace_path)
```

### Comparing `nvosscript-1.1.5/nvos/login.py` & `nvosscript-1.1.6/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.5/nvos/remote.py` & `nvosscript-1.1.6/nvos/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,19 +146,19 @@
 def post_data(url, params):
     headers = {"content-type": "application/json"}
     logger.info(f'request url:{url} params:{params}')
     response = requests.post(url, headers=headers, data=json.dumps(params))
     logger.info(f"response status_code: {response.status_code} text: {response.text} \n content:{response.content}")
     if response.status_code == 200:
         result = json.loads(response.text)
-        if result["code"] == "200":
+        if result["success"]:
             return result["data"]
         else:
             message = result["message"]
-            raise Exception('please error message is :{}'.format(message))
+            raise Exception('please check error message is :{}'.format(message))
     return {}
 
 
 def md5(git_branch, project_space):
     string = "%s%s" % (git_branch, project_space)
     hash_object = hashlib.md5(string.encode())
     md5_hash = hash_object.hexdigest()
```

### Comparing `nvosscript-1.1.5/nvos/run.py` & `nvosscript-1.1.6/nvos/run.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,15 +27,19 @@
         try:
             shutil.rmtree(os.path.join(os.getcwd(), ".ndtc"))
         except OSError as e:
             print(f"Error: {os.path.join(os.getcwd(), '.ndtc')} : {e.strerror}")
         return
 
     print("please wait one minute.........")
-    file.init_work_space(workspace_path)
+    try:
+        file.init_work_space(workspace_path)
+    except Exception as e:
+        logger.exception("command_init")
+        print(f"Error: {e}")
 
 
 def command_async():
     global all_workspace_path
     workspace_path, success = common_verify()
     if not success:
         return
@@ -73,23 +77,31 @@
 
 
 def command_pull():
     workspace_path, success = common_verify()
     if not success:
         return
     print("please wait one minute.........")
-    file.pull_data_from_cloud(workspace_path)
+    try:
+        file.pull_data_from_cloud(workspace_path)
+    except Exception as e:
+        logger.exception("command_pull")
+        print(f"Error: {e}")
 
 
 def command_push():
     workspace_path, success = common_verify()
     if not success:
         return
     print("please wait one minute.........")
-    file.push_data_to_cloud(workspace_path)
+    try:
+        file.push_data_to_cloud(workspace_path)
+    except Exception as e:
+        logger.exception("command_push")
+        print(f"Error: {e}")
 
 
 def common_verify():
     workspace_path, success = utils.check_workspace_exist(os.getcwd())
     if not success:
         print(
             "Please executor this command that your before executor init command of directory or subdirectory, or you can  executor init this directory")
@@ -99,7 +111,17 @@
         print("Please login first. you could use login command to login this script")
         return workspace_path, False
     return workspace_path, True
 
 
 def command_env(env):
     remote.switch_env(env)
+    workspace_env = []
+    with open(os.path.expanduser(os.path.join("~", "workspace_env")), 'r') as f:
+        for line in f:
+            workspace_env.append(line.strip())
+    for item in workspace_env:
+        try:
+            os.remove(os.path.join(item, ".ndtc", 'offset'))
+        except OSError as e:
+            print(f"Error: {os.path.join(item, '.ndtc', 'offset')} : {e.strerror}")
+
```

### Comparing `nvosscript-1.1.5/nvos/utils.py` & `nvosscript-1.1.6/nvos/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.5/setup.py` & `nvosscript-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.1.5',
+    version='1.1.6',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.1.5/start/main.py` & `nvosscript-1.1.6/start/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     elif args.subcommand == "async":
         run.command_async()
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.1.5")
+        print("1.1.6")
     elif args.subcommand == 'env':
         run.command_env(args.switch)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
         current_file_dir = os.path.dirname(current_file_dir)
         win_path = os.path.join(current_file_dir, 'win', 'win_auto_script.py')
```

### Comparing `nvosscript-1.1.5/win/win_auto_script.py` & `nvosscript-1.1.6/win/win_auto_script.py`

 * *Files identical despite different names*

