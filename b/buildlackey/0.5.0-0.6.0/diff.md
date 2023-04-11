# Comparing `tmp/buildlackey-0.5.0.tar.gz` & `tmp/buildlackey-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildlackey-0.5.0.tar", last modified: Mon Apr 10 18:29:52 2023, max compression
+gzip compressed data, was "buildlackey-0.6.0.tar", last modified: Tue Apr 11 00:38:34 2023, max compression
```

## Comparing `buildlackey-0.5.0.tar` & `buildlackey-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-10 18:29:52.256160 buildlackey-0.5.0/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-04-07 13:32:43.000000 buildlackey-0.5.0/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43940 2023-04-10 18:29:52.256024 buildlackey-0.5.0/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3760 2023-04-10 14:04:12.000000 buildlackey-0.5.0/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-10 18:29:52.253793 buildlackey-0.5.0/buildlackey/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5344 2023-04-10 01:27:16.000000 buildlackey-0.5.0/buildlackey/Commands.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      237 2023-04-04 01:39:34.000000 buildlackey-0.5.0/buildlackey/Environment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1045 2023-04-04 01:43:08.000000 buildlackey-0.5.0/buildlackey/EnvironmentBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-04-08 19:28:49.000000 buildlackey-0.5.0/buildlackey/Version.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-31 14:31:31.000000 buildlackey-0.5.0/buildlackey/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-10 18:29:52.255318 buildlackey-0.5.0/buildlackey/exceptions/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 buildlackey-0.5.0/buildlackey/exceptions/ProjectNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 buildlackey-0.5.0/buildlackey/exceptions/ProjectsBaseNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 01:41:26.000000 buildlackey-0.5.0/buildlackey/exceptions/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-10 18:29:52.255793 buildlackey-0.5.0/buildlackey/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 02:21:22.000000 buildlackey-0.5.0/buildlackey/resources/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      857 2023-04-07 13:34:44.000000 buildlackey-0.5.0/buildlackey/resources/loggingConfiguration.json
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        5 2023-04-10 17:50:52.000000 buildlackey-0.5.0/buildlackey/resources/version.txt
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-10 18:29:52.254607 buildlackey-0.5.0/buildlackey.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43940 2023-04-10 18:29:52.000000 buildlackey-0.5.0/buildlackey.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      621 2023-04-10 18:29:52.000000 buildlackey-0.5.0/buildlackey.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-10 18:29:52.000000 buildlackey-0.5.0/buildlackey.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      215 2023-04-10 18:29:52.000000 buildlackey-0.5.0/buildlackey.egg-info/entry_points.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-04-10 18:29:52.000000 buildlackey-0.5.0/buildlackey.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-10 18:29:52.000000 buildlackey-0.5.0/buildlackey.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-10 18:29:52.256192 buildlackey-0.5.0/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1331 2023-04-10 17:51:20.000000 buildlackey-0.5.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 00:38:34.849679 buildlackey-0.6.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-04-07 13:32:43.000000 buildlackey-0.6.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43932 2023-04-11 00:38:34.849540 buildlackey-0.6.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3752 2023-04-10 18:32:21.000000 buildlackey-0.6.0/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 00:38:34.847736 buildlackey-0.6.0/buildlackey/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5648 2023-04-11 00:33:02.000000 buildlackey-0.6.0/buildlackey/Commands.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1226 2023-04-11 00:27:42.000000 buildlackey-0.6.0/buildlackey/Environment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      469 2023-04-08 19:28:49.000000 buildlackey-0.6.0/buildlackey/Version.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-31 14:31:31.000000 buildlackey-0.6.0/buildlackey/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 00:38:34.848990 buildlackey-0.6.0/buildlackey/exceptions/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 buildlackey-0.6.0/buildlackey/exceptions/ProjectNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 buildlackey-0.6.0/buildlackey/exceptions/ProjectsBaseNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 01:41:26.000000 buildlackey-0.6.0/buildlackey/exceptions/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 00:38:34.849301 buildlackey-0.6.0/buildlackey/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-04 02:21:22.000000 buildlackey-0.6.0/buildlackey/resources/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      857 2023-04-07 13:34:44.000000 buildlackey-0.6.0/buildlackey/resources/loggingConfiguration.json
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        5 2023-04-11 00:37:57.000000 buildlackey-0.6.0/buildlackey/resources/version.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-11 00:38:34.848546 buildlackey-0.6.0/buildlackey.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    43932 2023-04-11 00:38:34.000000 buildlackey-0.6.0/buildlackey.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      590 2023-04-11 00:38:34.000000 buildlackey-0.6.0/buildlackey.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-11 00:38:34.000000 buildlackey-0.6.0/buildlackey.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      215 2023-04-11 00:38:34.000000 buildlackey-0.6.0/buildlackey.egg-info/entry_points.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-04-11 00:38:34.000000 buildlackey-0.6.0/buildlackey.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       12 2023-04-11 00:38:34.000000 buildlackey-0.6.0/buildlackey.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-11 00:38:34.849711 buildlackey-0.6.0/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1331 2023-04-10 17:51:20.000000 buildlackey-0.6.0/setup.py
```

### Comparing `buildlackey-0.5.0/LICENSE` & `buildlackey-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `buildlackey-0.5.0/PKG-INFO` & `buildlackey-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildlackey
-Version: 0.5.0
+Version: 0.6.0
 Summary: Project Maintenance Scripts
 Home-page: https://github.com/buildlackey
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
@@ -668,15 +668,15 @@
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/versionoverlord/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/versionoverlord/tree/master)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/buildlackey/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/buildlackey/tree/master)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
```

### Comparing `buildlackey-0.5.0/README.md` & `buildlackey-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/versionoverlord/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/versionoverlord/tree/master)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/buildlackey/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/buildlackey/tree/master)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/
-versionoverlord/tree/master.svg?style=shield)](https://dl.circleci.com/status-
-badge/redirect/gh/hasii2011/versionoverlord/tree/master) [![Maintenance](https:
-//img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/
-Naereen/StrapDown.js/graphs/commit-activity) [![macOS](https://svgshare.com/i/
-ZjP.svg)](https://svgshare.com/i/ZjP.svg) [![forthebadge made-with-python]
-(http://ForTheBadge.com/images/badges/made-with-python.svg)](https://
-www.python.org/) ## Rationale These utilities are meant to help me with my
-repositories and their maintenance. ## Dependencies These utilities work best
-using the following opinionated dependencies * Python [virtual environments]
-(https://realpython.com/python-virtual-environments-a-primer/) on a per
-project/repository basis * [direnv](https://direnv.net) to set up the project
-virtual environment and any necessary environment variables * Building using
-setup.py and the [build](https://pypi.org/project/build/) module to create
-source and binary distributions. The documentation is [here](https://pypa-
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/buildlackey/
+tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/
+gh/hasii2011/buildlackey/tree/master) [![Maintenance](https://img.shields.io/
+badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/
+graphs/commit-activity) [![macOS](https://svgshare.com/i/ZjP.svg)](https://
+svgshare.com/i/ZjP.svg) [![forthebadge made-with-python](http://
+ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
+) ## Rationale These utilities are meant to help me with my repositories and
+their maintenance. ## Dependencies These utilities work best using the
+following opinionated dependencies * Python [virtual environments](https://
+realpython.com/python-virtual-environments-a-primer/) on a per project/
+repository basis * [direnv](https://direnv.net) to set up the project virtual
+environment and any necessary environment variables * Building using setup.py
+and the [build](https://pypi.org/project/build/) module to create source and
+binary distributions. The documentation is [here](https://pypa-
 build.readthedocs.io/en/stable/) * Using [pypi](https://pypi.org/) for source
 and binary distributions * A correctly setup [$(HOME)/.pypirc](https://
 packaging.python.org/en/latest/specifications/pypirc/) for easy interaction
 with [twine](https://pypi.org/project/twine/) and [pypi](https://pypi.org/) ##
 Required Environment Variables The above commands depend on the following
 environment variables. ```bash PROJECTS_BASE - The local directory where the
 python projects are based PROJECT - The name of the project; It should be a
```

### Comparing `buildlackey-0.5.0/buildlackey/Commands.py` & `buildlackey-0.6.0/buildlackey/Commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 
-from os import system as osSystem
 from os import chdir
 
 from os import sep as osSep
+from os import system as osSystem
 
 from click import argument
 from click import clear
 from click import command
 from click import secho
 from click import version_option
 
-
+from buildlackey.Environment import EnvironmentBase
 from buildlackey.Version import Version
 
+
 # noinspection SpellCheckingInspection
 UNIT_TEST_CLI: str = 'python3 -Wdefault -m tests.TestAll'
 
 DELETE_DIST_BUILD:       str = 'rm -rfv dist build'
 DELETE_GENERAL_EGG_INFO: str = "find . -type d -name '*'.egg-info -delete"
 DELETE_LOG_FILES:        str = 'find . -type f -name "*.log"      -delete'
 DELETE_EGGS:             str = 'rm -rfv .eggs'
@@ -37,25 +38,29 @@
     secho(f'{project=}', color=True, reverse=True)
     secho('')
     changeToProjectRoot(projectsBase=projects_base, project=project)
 
 
 @command()
 @version_option(version=f'{Version().version}', message='%(prog)s version %(version)s')
-@argument('projects_base', envvar=PROJECTS_BASE)
-@argument('project',       envvar=PROJECT)
-def runtests(projects_base: str, project: str):
+def runtests():
     """
     \b
-    Runs the unit tests for the project specified by the following environment variables
+    Runs the unit tests for the project specified by the following environment variables;
+
     \b
         PROJECTS_BASE -  The local directory where the python projects are based
         PROJECT       -  The name of the project;  It should be a directory name
+    \b
+    However, if one or the other is not defined the command assumes it is executing in a CI
+    environment and thus the current working directory is the project base directory.
     """
-    doCommandStart(projects_base, project)
+    envBase: EnvironmentBase = EnvironmentBase()
+    if envBase.validProjectsBase is True and envBase.validProjectDirectory() is True:
+        changeToProjectRoot(projectsBase=envBase.projectsBase, project=envBase.projectDirectory)
 
     secho(f'{UNIT_TEST_CLI}')
     status: int = osSystem(f'{UNIT_TEST_CLI}')
     secho(f'{status=}')
 
 
 @command()
```

### Comparing `buildlackey-0.5.0/buildlackey/resources/loggingConfiguration.json` & `buildlackey-0.6.0/buildlackey/resources/loggingConfiguration.json`

 * *Files identical despite different names*

### Comparing `buildlackey-0.5.0/buildlackey.egg-info/PKG-INFO` & `buildlackey-0.6.0/buildlackey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildlackey
-Version: 0.5.0
+Version: 0.6.0
 Summary: Project Maintenance Scripts
 Home-page: https://github.com/buildlackey
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
@@ -668,15 +668,15 @@
         if any, to sign a "copyright disclaimer" for the program, if necessary.
         For more information on this, and how to apply and follow the GNU AGPL, see
         <https://www.gnu.org/licenses/>.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/versionoverlord/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/versionoverlord/tree/master)
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/hasii2011/buildlackey/tree/master.svg?style=shield)](https://dl.circleci.com/status-badge/redirect/gh/hasii2011/buildlackey/tree/master)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
```

### Comparing `buildlackey-0.5.0/buildlackey.egg-info/SOURCES.txt` & `buildlackey-0.6.0/buildlackey.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 setup.py
 buildlackey/Commands.py
 buildlackey/Environment.py
-buildlackey/EnvironmentBase.py
 buildlackey/Version.py
 buildlackey/__init__.py
 buildlackey.egg-info/PKG-INFO
 buildlackey.egg-info/SOURCES.txt
 buildlackey.egg-info/dependency_links.txt
 buildlackey.egg-info/entry_points.txt
 buildlackey.egg-info/requires.txt
```

### Comparing `buildlackey-0.5.0/setup.py` & `buildlackey-0.6.0/setup.py`

 * *Files identical despite different names*

