# Comparing `tmp/student-repos-handler-1.2.0.tar.gz` & `tmp/student-repos-handler-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "student-repos-handler-1.2.0.tar", last modified: Mon Aug 30 23:27:03 2021, max compression
+gzip compressed data, was "student-repos-handler-1.3.0.tar", last modified: Mon Apr 10 22:44:08 2023, max compression
```

## Comparing `student-repos-handler-1.2.0.tar` & `student-repos-handler-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 fisa      (1000) fisa      (1000)        0 2021-08-30 23:27:03.112704 student-repos-handler-1.2.0/
--rw-rw-r--   0 fisa      (1000) fisa      (1000)     1009 2021-08-30 23:27:03.112704 student-repos-handler-1.2.0/PKG-INFO
--rw-r--r--   0 fisa      (1000) fisa      (1000)      256 2020-09-12 01:06:10.000000 student-repos-handler-1.2.0/README.md
--rwxr-xr-x   0 fisa      (1000) fisa      (1000)    11278 2021-08-30 23:22:31.000000 student-repos-handler-1.2.0/repos.py
--rw-rw-r--   0 fisa      (1000) fisa      (1000)       38 2021-08-30 23:27:03.112704 student-repos-handler-1.2.0/setup.cfg
--rw-rw-r--   0 fisa      (1000) fisa      (1000)      910 2021-08-30 23:26:46.000000 student-repos-handler-1.2.0/setup.py
-drwxrwxr-x   0 fisa      (1000) fisa      (1000)        0 2021-08-30 23:27:03.108704 student-repos-handler-1.2.0/student_repos_handler.egg-info/
--rw-rw-r--   0 fisa      (1000) fisa      (1000)     1009 2021-08-30 23:27:02.000000 student-repos-handler-1.2.0/student_repos_handler.egg-info/PKG-INFO
--rw-rw-r--   0 fisa      (1000) fisa      (1000)      299 2021-08-30 23:27:03.000000 student-repos-handler-1.2.0/student_repos_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 fisa      (1000) fisa      (1000)        1 2021-08-30 23:27:02.000000 student-repos-handler-1.2.0/student_repos_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 fisa      (1000) fisa      (1000)       38 2021-08-30 23:27:02.000000 student-repos-handler-1.2.0/student_repos_handler.egg-info/entry_points.txt
--rw-rw-r--   0 fisa      (1000) fisa      (1000)       19 2021-08-30 23:27:02.000000 student-repos-handler-1.2.0/student_repos_handler.egg-info/requires.txt
--rw-rw-r--   0 fisa      (1000) fisa      (1000)        6 2021-08-30 23:27:02.000000 student-repos-handler-1.2.0/student_repos_handler.egg-info/top_level.txt
+drwxrwxr-x   0 fisa      (1000) fisa      (1000)        0 2023-04-10 22:44:08.086051 student-repos-handler-1.3.0/
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)     1009 2023-04-10 22:44:08.086051 student-repos-handler-1.3.0/PKG-INFO
+-rw-r--r--   0 fisa      (1000) fisa      (1000)      256 2020-09-12 01:06:10.000000 student-repos-handler-1.3.0/README.md
+-rwxr-xr-x   0 fisa      (1000) fisa      (1000)    12435 2023-04-10 22:42:35.000000 student-repos-handler-1.3.0/repos.py
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)       38 2023-04-10 22:44:08.086051 student-repos-handler-1.3.0/setup.cfg
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)      910 2023-04-10 22:43:48.000000 student-repos-handler-1.3.0/setup.py
+drwxrwxr-x   0 fisa      (1000) fisa      (1000)        0 2023-04-10 22:44:08.086051 student-repos-handler-1.3.0/student_repos_handler.egg-info/
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)     1009 2023-04-10 22:44:07.000000 student-repos-handler-1.3.0/student_repos_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)      299 2023-04-10 22:44:07.000000 student-repos-handler-1.3.0/student_repos_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)        1 2023-04-10 22:44:07.000000 student-repos-handler-1.3.0/student_repos_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)       38 2023-04-10 22:44:07.000000 student-repos-handler-1.3.0/student_repos_handler.egg-info/entry_points.txt
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)       19 2023-04-10 22:44:07.000000 student-repos-handler-1.3.0/student_repos_handler.egg-info/requires.txt
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)        6 2023-04-10 22:44:07.000000 student-repos-handler-1.3.0/student_repos_handler.egg-info/top_level.txt
```

### Comparing `student-repos-handler-1.2.0/PKG-INFO` & `student-repos-handler-1.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: student-repos-handler
-Version: 1.2.0
+Version: 1.3.0
 Summary: Simple tool to handle multiple repos at once, oriented to the grading of assignments in UCSE DAR
 Home-page: https://github.com/fisadev/student-repos-handler
 Author: Juan Pedro Fisanotti
 Author-email: fisadev@gmail.com
 License: LICENSE.txt
 Description: # Student-repos-handler
```

### Comparing `student-repos-handler-1.2.0/repos.py` & `student-repos-handler-1.3.0/repos.py`

 * *Files 11% similar despite different names*

```diff
@@ -108,21 +108,36 @@
     def iterate_filtered_repos(self, filters):
         repos = self.filter_repos(filters)
         for repo in repos:
             print(colored('-- %s --' % repo, 'green'))
             yield repo
 
     def vcs_action_on_repos(self, filters, vcs_action):
+        repos_ok = []
+        repos_err = []
+
         for repo in self.iterate_filtered_repos(filters):
+            code_ok = True
+            wiki_ok = True
+
             if 'code' in repo.features:
                 print(colored(' -- Code --', 'green'))
-                vcs_action(repo, 'code')
+                code_ok = vcs_action(repo, 'code')
             if 'wiki' in repo.features:
                 print(colored(' -- Wiki --', 'green'))
-                vcs_action(repo, 'wiki')
+                wiki_ok = vcs_action(repo, 'wiki')
+
+            if code_ok and wiki_ok:
+                repos_ok.append(repo)
+            else:
+                repos_err.append(repo)
+
+            print()
+
+        self.summary_errors(repos_ok, repos_err)
 
     def update(self, *filters):
         self.vcs_action_on_repos(filters, self.update_vcs)
 
     def clean(self, *filters):
         self.vcs_action_on_repos(filters, self.clean_vcs)
 
@@ -147,40 +162,43 @@
                 clone_command = 'git clone'
 
             command = '%s %s %s' % (clone_command, repo_url, repo_path)
 
         result = system(command)
         if result != 0:
             print(colored('Error running command', 'red'))
+        return result == 0
 
     def clean_vcs(self, repo, section):
         repo_path = repo.path(section, self.repos_root)
 
         if repo.vcs == 'hg':
             clean_command = 'hg revert --all --no-backup'
         elif repo.vcs == 'git':
             clean_command = 'git checkout -- .'
 
         command = '(cd %s && %s)' % (repo_path, clean_command)
         result = system(command)
         if result != 0:
             print(colored('Error running command', 'red'))
+        return result == 0
 
     def status_vcs(self, repo, section):
         repo_path = repo.path(section, self.repos_root)
 
         if repo.vcs == 'hg':
             clean_command = 'hg status'
         elif repo.vcs == 'git':
             clean_command = 'git status'
 
         command = '(cd %s && %s)' % (repo_path, clean_command)
         result = system(command)
         if result != 0:
             print(colored('Error running command', 'red'))
+        return result == 0
 
     def code(self, editor, file_, *filters):
         return self.open_vcs_file('code', editor, filters, file_, any_extension=False)
 
     def wiki(self, editor, file_, *filters):
         return self.open_vcs_file('wiki', editor, filters, file_, any_extension=True)
 
@@ -196,23 +214,33 @@
     def revive_server(self, *filters):
         for repo in self.iterate_filtered_repos(filters):
             print('Accessing server...')
             response = requests.get(repo.server)
             print('Response code:', response.status_code)
 
     def run(self, command, *filters):
+        repos_ok = []
+        repos_err = []
         for repo in self.iterate_filtered_repos(filters):
             repo_path = repo.path('code', self.repos_root)
             putenv("REPO_PATH", repo_path)
             result = system('(cd %s && %s)' % (repo_path, command))
-            if result != 0:
+            if result == 0:
+                repos_ok.append(repo)
+            else:
+                repos_err.append(repo)
                 print(colored('Error running command', 'red'))
             print()
 
+        self.summary_errors(repos_ok, repos_err)
+
     def open_vcs_file(self, section, editor, filters, file_, any_extension=False):
+        repos_ok = []
+        repos_err = []
+
         for repo in self.iterate_filtered_repos(filters):
             file_path = path.join(repo.path(section, self.repos_root), file_)
             possible_files = []
 
             if any_extension:
                 directory = path.dirname(file_path)
 
@@ -221,20 +249,26 @@
                                       for file_name in listdir(directory)
                                       if file_name.split('.')[0] == file_]
             else:
                 if path.exists(file_path):
                     possible_files = [file_path,]
 
             if not possible_files:
+                repos_err.append(repo)
                 print(colored('File does not exists', 'red'))
             elif len(possible_files) > 1:
+                repos_err.append(repo)
                 print(colored('Many files on the wiki with that name:', 'red'))
                 print('\n'.join(possible_files))
             else:
+                repos_ok.append(repo)
                 system('%s %s' % (editor, possible_files[0]))
+            print()
+
+        self.summary_errors(repos_ok, repos_err)
 
     def list(self, *filters):
         repos = self.filter_repos(filters)
         for repo in repos:
             print(repo.long_description())
 
     def show_urls(self, *filters):
@@ -276,14 +310,22 @@
                                 description=description)
                     repos.append(repo)
 
             if len(repos) != len(set(repo.alias for repo in repos)):
                 raise ValueError('There are repos with the same alias')
         return repos
 
+    @classmethod
+    def summary_errors(cls, repos_ok, repos_err):
+        if len(repos_ok) + len(repos_err) > 1:
+            if repos_ok:
+                print(colored('Success:', 'green'), ', '.join(map(str, repos_ok)))
+            if repos_err:
+                print(colored('Errors:', 'red'), ', '.join(map(str, repos_err)))
+
 
 def main():
     current_path = path.abspath('.')
     config_path = ReposHandler.find_repos_config(current_path)
     if not config_path:
         print(colored('Unable to find repos.config', 'red'))
         sys.exit(1)
```

### Comparing `student-repos-handler-1.2.0/setup.py` & `student-repos-handler-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(
     name='student-repos-handler',
-    version='1.2.0',
+    version='1.3.0',
     description='Simple tool to handle multiple repos at once, oriented to the grading of assignments in UCSE DAR',
     long_description=open('README.md').read(),
     author='Juan Pedro Fisanotti',
     author_email='fisadev@gmail.com',
     url='https://github.com/fisadev/student-repos-handler',
     license='LICENSE.txt',
     python_requires='>=3.4',
```

### Comparing `student-repos-handler-1.2.0/student_repos_handler.egg-info/PKG-INFO` & `student-repos-handler-1.3.0/student_repos_handler.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: student-repos-handler
-Version: 1.2.0
+Version: 1.3.0
 Summary: Simple tool to handle multiple repos at once, oriented to the grading of assignments in UCSE DAR
 Home-page: https://github.com/fisadev/student-repos-handler
 Author: Juan Pedro Fisanotti
 Author-email: fisadev@gmail.com
 License: LICENSE.txt
 Description: # Student-repos-handler
```

