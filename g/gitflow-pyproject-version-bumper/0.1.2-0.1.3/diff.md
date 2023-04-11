# Comparing `tmp/gitflow-pyproject-version-bumper-0.1.2.tar.gz` & `tmp/gitflow-pyproject-version-bumper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitflow-pyproject-version-bumper-0.1.2.tar", max compression
+gzip compressed data, was "gitflow-pyproject-version-bumper-0.1.3.tar", max compression
```

## Comparing `gitflow-pyproject-version-bumper-0.1.2.tar` & `gitflow-pyproject-version-bumper-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-03-30 21:36:49.551250 gitflow-pyproject-version-bumper-0.1.2/LICENSE
--rw-r--r--   0        0        0      953 2023-03-30 21:36:49.551250 gitflow-pyproject-version-bumper-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-03-30 21:36:49.551250 gitflow-pyproject-version-bumper-0.1.2/gitflow_pyproject_version_bumper/__init__.py
--rw-r--r--   0        0        0     1614 2023-03-31 07:06:04.630853 gitflow-pyproject-version-bumper-0.1.2/gitflow_pyproject_version_bumper/__main__.py
--rwxr-xr-x   0        0        0     1303 2023-03-30 21:36:49.551250 gitflow-pyproject-version-bumper-0.1.2/gitflow_pyproject_version_bumper/post_checkout.py
--rw-r--r--   0        0        0      627 2023-03-31 07:06:12.783083 gitflow-pyproject-version-bumper-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1763 1970-01-01 00:00:00.000000 gitflow-pyproject-version-bumper-0.1.2/setup.py
--rw-r--r--   0        0        0     1791 1970-01-01 00:00:00.000000 gitflow-pyproject-version-bumper-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-11 19:43:24.234598 gitflow-pyproject-version-bumper-0.1.3/LICENSE
+-rw-r--r--   0        0        0      953 2023-04-11 19:43:24.234598 gitflow-pyproject-version-bumper-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-03-30 21:36:49.551250 gitflow-pyproject-version-bumper-0.1.3/gitflow_pyproject_version_bumper/__init__.py
+-rw-r--r--   0        0        0     1614 2023-04-11 19:43:24.262598 gitflow-pyproject-version-bumper-0.1.3/gitflow_pyproject_version_bumper/__main__.py
+-rwxr-xr-x   0        0        0     1340 2023-04-11 19:43:57.506640 gitflow-pyproject-version-bumper-0.1.3/gitflow_pyproject_version_bumper/post_checkout.py
+-rw-r--r--   0        0        0      627 2023-04-11 19:44:04.234648 gitflow-pyproject-version-bumper-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1763 1970-01-01 00:00:00.000000 gitflow-pyproject-version-bumper-0.1.3/setup.py
+-rw-r--r--   0        0        0     1791 1970-01-01 00:00:00.000000 gitflow-pyproject-version-bumper-0.1.3/PKG-INFO
```

### Comparing `gitflow-pyproject-version-bumper-0.1.2/LICENSE` & `gitflow-pyproject-version-bumper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gitflow-pyproject-version-bumper-0.1.2/README.md` & `gitflow-pyproject-version-bumper-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gitflow-pyproject-version-bumper-0.1.2/gitflow_pyproject_version_bumper/__main__.py` & `gitflow-pyproject-version-bumper-0.1.3/gitflow_pyproject_version_bumper/__main__.py`

 * *Files identical despite different names*

### Comparing `gitflow-pyproject-version-bumper-0.1.2/gitflow_pyproject_version_bumper/post_checkout.py` & `gitflow-pyproject-version-bumper-0.1.3/gitflow_pyproject_version_bumper/post_checkout.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,35 @@
 BRANCH_CHECKOUT_TYPE = "1"
 
 _, _, _, checkout_type = sys.argv
 if checkout_type != BRANCH_CHECKOUT_TYPE:
     exit()
 
 repo = git.Repo()
+try:
+    head = repo.active_branch
+except TypeError:
+    exit()
+
 pyproject_toml_path = pathlib.Path(repo.working_dir).joinpath("pyproject.toml")
 with repo.config_reader() as git_config:
     gitflow_release_prefix = git_config.get(
         section='gitflow "prefix"',
         option="release",
         fallback="release/",
     )
     gitflow_hotfix_prefix = git_config.get(
         section='gitflow "prefix"',
         option="hotfix",
         fallback="hotfix/",
     )
 
-if repo.active_branch.name.startswith(gitflow_release_prefix):
+if head.name.startswith(gitflow_release_prefix):
     new_version = repo.active_branch.name[len(gitflow_release_prefix) :]
-elif repo.active_branch.name.startswith(gitflow_hotfix_prefix):
+elif head.name.startswith(gitflow_hotfix_prefix):
     new_version = repo.active_branch.name[len(gitflow_hotfix_prefix) :]
 else:
     exit()
 
 with open(pyproject_toml_path, "rb") as f:
     pyproject = tomlkit.load(f)
```

### Comparing `gitflow-pyproject-version-bumper-0.1.2/pyproject.toml` & `gitflow-pyproject-version-bumper-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitflow-pyproject-version-bumper"
-version = "0.1.2"
+version = "0.1.3"
 description = "Automatic pyproject.toml based app version bumper"
 authors = ["Grigory Bukovsky <booqoffsky@yandex.ru>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "gitflow_pyproject_version_bumper"}]
 repository = 'https://github.com/booqoffsky/gitflow-pyproject-version-bumper'
 keywords = ['gitflow', 'version', 'bumper', 'auto', 'pyproject', 'poetry', 'updater']
```

### Comparing `gitflow-pyproject-version-bumper-0.1.2/setup.py` & `gitflow-pyproject-version-bumper-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['GitPython>=3.1.31,<4.0.0', 'tomlkit>=0.11.7,<0.12.0']
 
 setup_kwargs = {
     'name': 'gitflow-pyproject-version-bumper',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Automatic pyproject.toml based app version bumper',
     'long_description': "![python version](https://img.shields.io/pypi/pyversions/gitflow-pyproject-version-bumper?style=for-the-badge) \n[![version](https://img.shields.io/pypi/v/gitflow-pyproject-version-bumper?style=for-the-badge)](https://pypi.org/project/gitflow-pyproject-version-bumper/)\n\n# gitflow-pyproject-version-bumper\n> A git hook to automatically update the application version \n> in pyproject.toml when a release is started using [gitflow](https://github.com/nvie/gitflow).\n\n# Installation\nFrom PyPi:\n\n```\npip3 install gitflow-pyproject-version-bumper\npython3 -m gitflow_pyproject_version_bumper install\n```\n\nIf you want to install it from sources, try this:\n\n```\npython3 -m pip install poetry\npython3 -m pip install .\npython3 -m gitflow_pyproject_version_bumper install\n```\n\n# Usage\nJust start a release, as you usually do:\n`git flow release start 1.2.3`\n\nThat's it.\nThe app version in pyproject.toml has already been updated, \nand the change has been committed.\n",
     'author': 'Grigory Bukovsky',
     'author_email': 'booqoffsky@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/booqoffsky/gitflow-pyproject-version-bumper',
```

### Comparing `gitflow-pyproject-version-bumper-0.1.2/PKG-INFO` & `gitflow-pyproject-version-bumper-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitflow-pyproject-version-bumper
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automatic pyproject.toml based app version bumper
 Home-page: https://github.com/booqoffsky/gitflow-pyproject-version-bumper
 License: MIT
 Keywords: gitflow,version,bumper,auto,pyproject,poetry,updater
 Author: Grigory Bukovsky
 Author-email: booqoffsky@yandex.ru
 Requires-Python: >=3.8,<4.0
```

