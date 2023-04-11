# Comparing `tmp/nvosscript-1.1.6.tar.gz` & `tmp/nvosscript-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.1.6.tar", last modified: Tue Apr 11 03:34:11 2023, max compression
+gzip compressed data, was "nvosscript-1.1.7.tar", last modified: Tue Apr 11 07:53:57 2023, max compression
```

## Comparing `nvosscript-1.1.6.tar` & `nvosscript-1.1.7.tar`

### file list

```diff
@@ -1,25 +1,41 @@
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-11 03:34:11.688730 nvosscript-1.1.6/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1073 2023-03-22 09:01:10.000000 nvosscript-1.1.6/LICENSE
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-11 03:34:11.688551 nvosscript-1.1.6/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)       78 2023-03-22 09:07:29.000000 nvosscript-1.1.6/README.md
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-11 03:34:11.686565 nvosscript-1.1.6/nvos/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-03-21 08:49:46.000000 nvosscript-1.1.6/nvos/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)    12894 2023-04-11 03:19:59.000000 nvosscript-1.1.6/nvos/file.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1662 2023-04-06 06:54:07.000000 nvosscript-1.1.6/nvos/login.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     7331 2023-04-11 03:09:14.000000 nvosscript-1.1.6/nvos/remote.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     4247 2023-04-11 03:24:00.000000 nvosscript-1.1.6/nvos/run.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)      812 2023-03-30 03:32:22.000000 nvosscript-1.1.6/nvos/utils.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-11 03:34:11.687634 nvosscript-1.1.6/nvosscript.egg-info/
--rw-r--r--   0 andre.zhao   (503) staff       (20)      333 2023-04-11 03:34:11.000000 nvosscript-1.1.6/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 andre.zhao   (503) staff       (20)      372 2023-04-11 03:34:11.000000 nvosscript-1.1.6/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)        1 2023-04-11 03:34:11.000000 nvosscript-1.1.6/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       41 2023-04-11 03:34:11.000000 nvosscript-1.1.6/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       47 2023-04-11 03:34:11.000000 nvosscript-1.1.6/nvosscript.egg-info/requires.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       21 2023-04-11 03:34:11.000000 nvosscript-1.1.6/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 andre.zhao   (503) staff       (20)       38 2023-04-11 03:34:11.688774 nvosscript-1.1.6/setup.cfg
--rw-r--r--   0 andre.zhao   (503) staff       (20)      805 2023-04-11 03:24:33.000000 nvosscript-1.1.6/setup.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-11 03:34:11.687871 nvosscript-1.1.6/start/
--rw-r--r--   0 andre.zhao   (503) staff       (20)        0 2023-04-04 03:24:28.000000 nvosscript-1.1.6/start/__init__.py
--rw-r--r--   0 andre.zhao   (503) staff       (20)     3480 2023-04-11 03:24:43.000000 nvosscript-1.1.6/start/main.py
-drwxr-xr-x   0 andre.zhao   (503) staff       (20)        0 2023-04-11 03:34:11.688109 nvosscript-1.1.6/win/
--rw-r--r--   0 andre.zhao   (503) staff       (20)     1283 2023-04-11 01:53:27.000000 nvosscript-1.1.6/win/win_auto_script.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.429110 nvosscript-1.1.7/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.1.7/LICENSE
+-rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-04-11 07:53:57.428683 nvosscript-1.1.7/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.1.7/README.md
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.414273 nvosscript-1.1.7/nvos/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.1.7/nvos/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)    12892 2023-04-11 07:52:31.000000 nvosscript-1.1.7/nvos/file.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.1.7/nvos/login.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     7331 2023-04-11 07:50:33.000000 nvosscript-1.1.7/nvos/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     4376 2023-04-11 07:50:33.000000 nvosscript-1.1.7/nvos/run.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      812 2023-04-11 07:50:33.000000 nvosscript-1.1.7/nvos/utils.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.417599 nvosscript-1.1.7/nvosscript.egg-info/
+-rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-04-11 07:53:57.000000 nvosscript-1.1.7/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)      682 2023-04-11 07:53:57.000000 nvosscript-1.1.7/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-04-11 07:53:57.000000 nvosscript-1.1.7/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-04-11 07:53:57.000000 nvosscript-1.1.7/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-04-11 07:53:57.000000 nvosscript-1.1.7/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       20 2023-04-11 07:53:57.000000 nvosscript-1.1.7/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-04-11 07:53:57.429155 nvosscript-1.1.7/setup.cfg
+-rw-r--r--   0 matador.wang   (503) staff       (20)      805 2023-04-11 07:50:33.000000 nvosscript-1.1.7/setup.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.418371 nvosscript-1.1.7/start/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.1.7/start/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     3480 2023-04-11 07:50:33.000000 nvosscript-1.1.7/start/main.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.408278 nvosscript-1.1.7/venv/
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.427430 nvosscript-1.1.7/venv/bin/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-04-11 07:07:42.000000 nvosscript-1.1.7/venv/bin/activate_this.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)     1735 2023-04-11 07:08:34.000000 nvosscript-1.1.7/venv/bin/jp.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      632 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2html.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      754 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2html4.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)     1099 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2html5.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      831 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2latex.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      654 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2man.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      820 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2odt.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)     1758 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      639 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      675 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2s5.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      911 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      640 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2xml.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      708 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rstpep2html.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.428185 nvosscript-1.1.7/win/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1283 2023-04-11 07:50:33.000000 nvosscript-1.1.7/win/win_auto_script.py
```

### Comparing `nvosscript-1.1.6/LICENSE` & `nvosscript-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.6/nvos/file.py` & `nvosscript-1.1.7/nvos/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,16 +195,16 @@
             if temp["project_space"] == item["project_space"]:
                 flag = False
                 break
         if flag:
             filter_duplicate.append(item)
     project_space_list.clear()
     for project_space in exit_git_data:
-        if project_space["git_branch"] != "(no branch)":
-            project_space_list.append(project_space)
+        # if project_space["git_branch"] != "(no branch)":
+        project_space_list.append(project_space)
     project_space_list.extend(filter_duplicate)
     return project_space_list
 
 
 def get_current_git_branch(workspace_path):
     git_path = os.path.join(workspace_path, ".git")
     if not os.path.exists(git_path):
```

### Comparing `nvosscript-1.1.6/nvos/login.py` & `nvosscript-1.1.7/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.6/nvos/remote.py` & `nvosscript-1.1.7/nvos/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.6/nvos/run.py` & `nvosscript-1.1.7/nvos/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,10 +118,12 @@
     workspace_env = []
     with open(os.path.expanduser(os.path.join("~", "workspace_env")), 'r') as f:
         for line in f:
             workspace_env.append(line.strip())
     for item in workspace_env:
         try:
             os.remove(os.path.join(item, ".ndtc", 'offset'))
+            os.remove(os.path.join(item, ".ndtc", 'project_space'))
+            os.remove(os.path.join(item, ".ndtc", 'config'))
         except OSError as e:
             print(f"Error: {os.path.join(item, '.ndtc', 'offset')} : {e.strerror}")
```

### Comparing `nvosscript-1.1.6/nvos/utils.py` & `nvosscript-1.1.7/nvos/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.6/setup.py` & `nvosscript-1.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.1.6',
+    version='1.1.7',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.1.6/start/main.py` & `nvosscript-1.1.7/start/main.py`

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
-        print("1.1.6")
+        print("1.1.7")
     elif args.subcommand == 'env':
         run.command_env(args.switch)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
         current_file_dir = os.path.dirname(current_file_dir)
         win_path = os.path.join(current_file_dir, 'win', 'win_auto_script.py')
```

### Comparing `nvosscript-1.1.6/win/win_auto_script.py` & `nvosscript-1.1.7/win/win_auto_script.py`

 * *Files identical despite different names*

