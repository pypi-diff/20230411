# Comparing `tmp/gpush-2.0.0.tar.gz` & `tmp/gpush-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpush-2.0.0.tar", last modified: Mon Apr 10 19:25:55 2023, max compression
+gzip compressed data, was "gpush-2.1.0.tar", last modified: Tue Apr 11 06:40:05 2023, max compression
```

## Comparing `gpush-2.0.0.tar` & `gpush-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:25:55.128754 gpush-2.0.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-10 19:25:51.000000 gpush-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1300 2023-04-10 19:25:55.128754 gpush-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1188 2023-04-10 19:25:51.000000 gpush-2.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1826 2023-04-10 19:25:51.000000 gpush-2.0.0/gpush
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 19:25:55.128754 gpush-2.0.0/gpush.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1300 2023-04-10 19:25:55.000000 gpush-2.0.0/gpush.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      191 2023-04-10 19:25:55.000000 gpush-2.0.0/gpush.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 19:25:55.000000 gpush-2.0.0/gpush.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-10 19:25:55.000000 gpush-2.0.0/gpush.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 19:25:55.000000 gpush-2.0.0/gpush.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      224 2023-04-10 19:25:51.000000 gpush-2.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 19:25:55.128754 gpush-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      521 2023-04-10 19:25:52.000000 gpush-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:40:05.609789 gpush-2.1.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-11 06:40:01.000000 gpush-2.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-04-11 06:40:05.609789 gpush-2.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-04-11 06:40:01.000000 gpush-2.1.0/README.md
+-rwxr-xr-x   0 root         (0) root         (0)     2549 2023-04-11 06:40:01.000000 gpush-2.1.0/gpush
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:40:05.609789 gpush-2.1.0/gpush.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-04-11 06:40:05.000000 gpush-2.1.0/gpush.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      191 2023-04-11 06:40:05.000000 gpush-2.1.0/gpush.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 06:40:05.000000 gpush-2.1.0/gpush.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-04-11 06:40:05.000000 gpush-2.1.0/gpush.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 06:40:05.000000 gpush-2.1.0/gpush.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      224 2023-04-11 06:40:01.000000 gpush-2.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 06:40:05.609789 gpush-2.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      521 2023-04-11 06:40:02.000000 gpush-2.1.0/setup.py
```

### Comparing `gpush-2.0.0/LICENSE` & `gpush-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpush-2.0.0/PKG-INFO` & `gpush-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpush
-Version: 2.0.0
+Version: 2.1.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gpush
 
 `gpush` is a command line utility for standardising commit messages using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
```

### Comparing `gpush-2.0.0/README.md` & `gpush-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gpush-2.0.0/gpush` & `gpush-2.1.0/gpush`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,41 @@
 
 """
 Python script to handle git commit and push to standardise commit messages using conventional commit
 messages.
 
 Usage: gpush
 """
+import sys
 
 import inquirer
 from git import Repo
+import argparse
 
+found_version = False
+with open("setup.py", encoding="UTF-8") as setup_file:
+    for line in setup_file:
+        if line.startswith("__version__"):
+            version = line.split("=")[1].replace("\"","").strip()
+            found_version = True
+
+if not found_version:
+    print("__version__ not detected in setup.py")
+    sys.exit(1)
+
+parser = argparse.ArgumentParser(
+    prog="gpush " + version,
+    description="Git commit helper for conventional commit messages",
+)
+parser.add_argument(
+    '--version',
+    action='store_true',
+    help="Option to print the current version only"
+)
+args = parser.parse_args()
 
 def git_push(commit_message):
     """
     Function to push commit up to Git on the current branch for the repository
     :param commit_message: String containing the conventional commit message formatted commit
     message
     :return: True/False
@@ -60,8 +83,11 @@
     commit_message = (
         answers["type"] + is_breaking_change + ": " + answers["commit_message"]
     )
     git_push(commit_message)
 
 
 if __name__ == "__main__":
-    collect_details()
+    if args.version:
+        print("Current version: " + version)
+    else:
+        collect_details()
```

### Comparing `gpush-2.0.0/gpush.egg-info/PKG-INFO` & `gpush-2.1.0/gpush.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpush
-Version: 2.0.0
+Version: 2.1.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gpush
 
 `gpush` is a command line utility for standardising commit messages using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
```

### Comparing `gpush-2.0.0/setup.py` & `gpush-2.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("README.md", encoding="UTF-8") as readme_file:
     readme_contents = readme_file.read()
 
 with open("requirements.txt", encoding="UTF-8") as requirements_file:
     required = requirements_file.read().splitlines()
 
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 
 setup(
     name="gpush",
     version=__version__,
     long_description=readme_contents,
     long_description_content_type="text/markdown",
     install_requires=required,
```

