# Comparing `tmp/nvosscript-1.1.7.tar.gz` & `tmp/nvosscript-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvosscript-1.1.7.tar", last modified: Tue Apr 11 07:53:57 2023, max compression
+gzip compressed data, was "nvosscript-1.1.8.tar", last modified: Tue Apr 11 09:49:37 2023, max compression
```

## Comparing `nvosscript-1.1.7.tar` & `nvosscript-1.1.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.429110 nvosscript-1.1.7/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.1.7/LICENSE
--rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-04-11 07:53:57.428683 nvosscript-1.1.7/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.1.7/README.md
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.414273 nvosscript-1.1.7/nvos/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.1.7/nvos/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)    12892 2023-04-11 07:52:31.000000 nvosscript-1.1.7/nvos/file.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.1.7/nvos/login.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     7331 2023-04-11 07:50:33.000000 nvosscript-1.1.7/nvos/remote.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     4376 2023-04-11 07:50:33.000000 nvosscript-1.1.7/nvos/run.py
--rw-r--r--   0 matador.wang   (503) staff       (20)      812 2023-04-11 07:50:33.000000 nvosscript-1.1.7/nvos/utils.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.417599 nvosscript-1.1.7/nvosscript.egg-info/
--rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-04-11 07:53:57.000000 nvosscript-1.1.7/nvosscript.egg-info/PKG-INFO
--rw-r--r--   0 matador.wang   (503) staff       (20)      682 2023-04-11 07:53:57.000000 nvosscript-1.1.7/nvosscript.egg-info/SOURCES.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-04-11 07:53:57.000000 nvosscript-1.1.7/nvosscript.egg-info/dependency_links.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-04-11 07:53:57.000000 nvosscript-1.1.7/nvosscript.egg-info/entry_points.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-04-11 07:53:57.000000 nvosscript-1.1.7/nvosscript.egg-info/requires.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       20 2023-04-11 07:53:57.000000 nvosscript-1.1.7/nvosscript.egg-info/top_level.txt
--rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-04-11 07:53:57.429155 nvosscript-1.1.7/setup.cfg
--rw-r--r--   0 matador.wang   (503) staff       (20)      805 2023-04-11 07:50:33.000000 nvosscript-1.1.7/setup.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.418371 nvosscript-1.1.7/start/
--rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.1.7/start/__init__.py
--rw-r--r--   0 matador.wang   (503) staff       (20)     3480 2023-04-11 07:50:33.000000 nvosscript-1.1.7/start/main.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.408278 nvosscript-1.1.7/venv/
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.427430 nvosscript-1.1.7/venv/bin/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-04-11 07:07:42.000000 nvosscript-1.1.7/venv/bin/activate_this.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)     1735 2023-04-11 07:08:34.000000 nvosscript-1.1.7/venv/bin/jp.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      632 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2html.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      754 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2html4.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)     1099 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2html5.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      831 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2latex.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      654 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2man.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      820 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2odt.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)     1758 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      639 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      675 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2s5.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      911 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2xetex.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      640 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rst2xml.py
--rwxr-xr-x   0 matador.wang   (503) staff       (20)      708 2023-04-11 07:08:20.000000 nvosscript-1.1.7/venv/bin/rstpep2html.py
-drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:53:57.428185 nvosscript-1.1.7/win/
--rw-r--r--   0 matador.wang   (503) staff       (20)     1283 2023-04-11 07:50:33.000000 nvosscript-1.1.7/win/win_auto_script.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 09:49:37.523821 nvosscript-1.1.8/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1073 2023-04-11 06:52:30.000000 nvosscript-1.1.8/LICENSE
+-rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-04-11 09:49:37.523398 nvosscript-1.1.8/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)       78 2023-04-11 06:52:30.000000 nvosscript-1.1.8/README.md
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 09:49:37.509117 nvosscript-1.1.8/nvos/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 06:52:30.000000 nvosscript-1.1.8/nvos/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)    12890 2023-04-11 09:49:24.000000 nvosscript-1.1.8/nvos/file.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1662 2023-04-11 07:50:33.000000 nvosscript-1.1.8/nvos/login.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     7331 2023-04-11 07:50:33.000000 nvosscript-1.1.8/nvos/remote.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     4376 2023-04-11 07:50:33.000000 nvosscript-1.1.8/nvos/run.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)      812 2023-04-11 07:50:33.000000 nvosscript-1.1.8/nvos/utils.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 09:49:37.512450 nvosscript-1.1.8/nvosscript.egg-info/
+-rw-r--r--   0 matador.wang   (503) staff       (20)      333 2023-04-11 09:49:37.000000 nvosscript-1.1.8/nvosscript.egg-info/PKG-INFO
+-rw-r--r--   0 matador.wang   (503) staff       (20)      682 2023-04-11 09:49:37.000000 nvosscript-1.1.8/nvosscript.egg-info/SOURCES.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)        1 2023-04-11 09:49:37.000000 nvosscript-1.1.8/nvosscript.egg-info/dependency_links.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       41 2023-04-11 09:49:37.000000 nvosscript-1.1.8/nvosscript.egg-info/entry_points.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       47 2023-04-11 09:49:37.000000 nvosscript-1.1.8/nvosscript.egg-info/requires.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       31 2023-04-11 09:49:37.000000 nvosscript-1.1.8/nvosscript.egg-info/top_level.txt
+-rw-r--r--   0 matador.wang   (503) staff       (20)       38 2023-04-11 09:49:37.523866 nvosscript-1.1.8/setup.cfg
+-rw-r--r--   0 matador.wang   (503) staff       (20)      805 2023-04-11 09:45:48.000000 nvosscript-1.1.8/setup.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 09:49:37.513331 nvosscript-1.1.8/start/
+-rw-r--r--   0 matador.wang   (503) staff       (20)        0 2023-04-11 07:50:33.000000 nvosscript-1.1.8/start/__init__.py
+-rw-r--r--   0 matador.wang   (503) staff       (20)     3480 2023-04-11 09:48:19.000000 nvosscript-1.1.8/start/main.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 09:49:37.503397 nvosscript-1.1.8/venv/
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 09:49:37.522193 nvosscript-1.1.8/venv/bin/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1175 2023-04-11 07:07:42.000000 nvosscript-1.1.8/venv/bin/activate_this.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)     1735 2023-04-11 07:08:34.000000 nvosscript-1.1.8/venv/bin/jp.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      632 2023-04-11 07:08:20.000000 nvosscript-1.1.8/venv/bin/rst2html.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      754 2023-04-11 07:08:20.000000 nvosscript-1.1.8/venv/bin/rst2html4.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)     1099 2023-04-11 07:08:20.000000 nvosscript-1.1.8/venv/bin/rst2html5.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      831 2023-04-11 07:08:20.000000 nvosscript-1.1.8/venv/bin/rst2latex.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      654 2023-04-11 07:08:20.000000 nvosscript-1.1.8/venv/bin/rst2man.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      820 2023-04-11 07:08:20.000000 nvosscript-1.1.8/venv/bin/rst2odt.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)     1758 2023-04-11 07:08:20.000000 nvosscript-1.1.8/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      639 2023-04-11 07:08:20.000000 nvosscript-1.1.8/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      675 2023-04-11 07:08:20.000000 nvosscript-1.1.8/venv/bin/rst2s5.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      911 2023-04-11 07:08:20.000000 nvosscript-1.1.8/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      640 2023-04-11 07:08:20.000000 nvosscript-1.1.8/venv/bin/rst2xml.py
+-rwxr-xr-x   0 matador.wang   (503) staff       (20)      708 2023-04-11 07:08:20.000000 nvosscript-1.1.8/venv/bin/rstpep2html.py
+drwxr-xr-x   0 matador.wang   (503) staff       (20)        0 2023-04-11 09:49:37.522882 nvosscript-1.1.8/win/
+-rw-r--r--   0 matador.wang   (503) staff       (20)     1283 2023-04-11 07:50:33.000000 nvosscript-1.1.8/win/win_auto_script.py
```

### Comparing `nvosscript-1.1.7/LICENSE` & `nvosscript-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/nvos/file.py` & `nvosscript-1.1.8/nvos/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,16 +148,16 @@
         if project_space["git_branch"] == "nvos_default":
             not_exit_git_data.append(project_space)
         else:
             exit_git_data.append(project_space)
     if len(not_exit_git_data) == 0:
         project_space_list.clear()
         for project_space in exit_git_data:
-            if project_space["git_branch"] != "(no branch)":
-                project_space_list.append(project_space)
+            # if project_space["git_branch"] != "(no branch)":
+            project_space_list.append(project_space)
         return project_space_list
     if len(exit_git_data) == 0:
         result_list = []
         for file_path in os.listdir(workspace_path):
             if file_path == ".idea" or file_path == ".repo" or file_path == ".ndtc" or file_path == ".DS_Store":
                 continue
             if os.path.isdir(os.path.join(workspace_path, file_path)):
```

### Comparing `nvosscript-1.1.7/nvos/login.py` & `nvosscript-1.1.8/nvos/login.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/nvos/remote.py` & `nvosscript-1.1.8/nvos/remote.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/nvos/run.py` & `nvosscript-1.1.8/nvos/run.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/nvos/utils.py` & `nvosscript-1.1.8/nvos/utils.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/nvosscript.egg-info/SOURCES.txt` & `nvosscript-1.1.8/nvosscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/setup.py` & `nvosscript-1.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='nvosscript',
-    version='1.1.7',
+    version='1.1.8',
     description='nvos toolchain script',
     packages=find_namespace_packages(),
     author = 'andre.zhao',
     author_email = 'andre.zhao@nio.com',
     keywords='pack',
     readme = "README.md",
     install_requires=[
```

### Comparing `nvosscript-1.1.7/start/main.py` & `nvosscript-1.1.8/start/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     elif args.subcommand == "async":
         run.command_async()
     elif args.subcommand == "pull":
         run.command_pull()
     elif args.subcommand == "push":
         run.command_push()
     elif args.subcommand == "version":
-        print("1.1.7")
+        print("1.1.8")
     elif args.subcommand == 'env':
         run.command_env(args.switch)
     elif args.subcommand == "path":
         current_file_path = os.path.abspath(__file__)
         current_file_dir = os.path.dirname(current_file_path)
         current_file_dir = os.path.dirname(current_file_dir)
         win_path = os.path.join(current_file_dir, 'win', 'win_auto_script.py')
```

### Comparing `nvosscript-1.1.7/venv/bin/activate_this.py` & `nvosscript-1.1.8/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/venv/bin/jp.py` & `nvosscript-1.1.8/venv/bin/jp.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/venv/bin/rst2html.py` & `nvosscript-1.1.8/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/venv/bin/rst2html4.py` & `nvosscript-1.1.8/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/venv/bin/rst2html5.py` & `nvosscript-1.1.8/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/venv/bin/rst2latex.py` & `nvosscript-1.1.8/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/venv/bin/rst2man.py` & `nvosscript-1.1.8/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/venv/bin/rst2odt.py` & `nvosscript-1.1.8/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/venv/bin/rst2odt_prepstyles.py` & `nvosscript-1.1.8/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/venv/bin/rst2pseudoxml.py` & `nvosscript-1.1.8/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/venv/bin/rst2s5.py` & `nvosscript-1.1.8/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/venv/bin/rst2xetex.py` & `nvosscript-1.1.8/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/venv/bin/rst2xml.py` & `nvosscript-1.1.8/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/venv/bin/rstpep2html.py` & `nvosscript-1.1.8/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `nvosscript-1.1.7/win/win_auto_script.py` & `nvosscript-1.1.8/win/win_auto_script.py`

 * *Files identical despite different names*

