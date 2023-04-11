# Comparing `tmp/smyg-0.5.4.tar.gz` & `tmp/smyg-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smyg-0.5.4.tar", max compression
+gzip compressed data, was "smyg-0.5.5.tar", max compression
```

## Comparing `smyg-0.5.4.tar` & `smyg-0.5.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1074 2023-02-28 14:40:14.827915 smyg-0.5.4/LICENSE
--rw-r--r--   0        0        0     7874 2023-02-28 14:40:14.827915 smyg-0.5.4/README.md
--rw-r--r--   0        0        0      903 2023-04-08 05:58:45.268063 smyg-0.5.4/pyproject.toml
--rw-r--r--   0        0        0       44 2023-04-08 05:58:29.543923 smyg-0.5.4/smyg/__init__.py
--rw-r--r--   0        0        0      125 2023-04-08 05:50:26.909484 smyg-0.5.4/smyg/__main__.py
--rw-r--r--   0        0        0     3856 2023-03-20 12:25:27.549846 smyg-0.5.4/smyg/binding.py
--rw-r--r--   0        0        0    10219 2023-04-08 05:57:24.275373 smyg-0.5.4/smyg/cli.py
--rw-r--r--   0        0        0      736 2023-02-28 14:40:14.827915 smyg-0.5.4/smyg/formatter.py
--rw-r--r--   0        0        0     2214 2023-02-28 14:40:14.827915 smyg-0.5.4/smyg/metrics/code_changes.py
--rw-r--r--   0        0        0     2247 2023-02-28 14:40:14.827915 smyg-0.5.4/smyg/metrics/code_churn.py
--rw-r--r--   0        0        0     3806 2023-04-08 04:48:52.348220 smyg-0.5.4/smyg/prom.py
--rw-r--r--   0        0        0      421 2023-02-28 14:40:14.827915 smyg-0.5.4/smyg/templates/code_changes.j2
--rw-r--r--   0        0        0      244 2023-02-28 14:40:14.827915 smyg-0.5.4/smyg/templates/commit.j2
--rw-r--r--   0        0        0      305 2023-02-28 14:40:14.827915 smyg-0.5.4/smyg/templates/commits.j2
--rw-r--r--   0        0        0     1289 2023-02-28 14:40:14.827915 smyg-0.5.4/smyg/utils.py
--rw-r--r--   0        0        0     7040 2023-02-28 14:40:14.827915 smyg-0.5.4/smyg/vcs.py
--rw-r--r--   0        0        0     9088 1970-01-01 00:00:00.000000 smyg-0.5.4/setup.py
--rw-r--r--   0        0        0     8884 1970-01-01 00:00:00.000000 smyg-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-02-28 14:40:14.827915 smyg-0.5.5/LICENSE
+-rw-r--r--   0        0        0     7874 2023-02-28 14:40:14.827915 smyg-0.5.5/README.md
+-rw-r--r--   0        0        0      903 2023-04-11 06:14:22.544397 smyg-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-04-11 06:14:33.352501 smyg-0.5.5/smyg/__init__.py
+-rw-r--r--   0        0        0      125 2023-04-08 05:50:26.909484 smyg-0.5.5/smyg/__main__.py
+-rw-r--r--   0        0        0     3887 2023-04-11 06:13:52.004100 smyg-0.5.5/smyg/binding.py
+-rw-r--r--   0        0        0    10219 2023-04-08 05:57:24.275373 smyg-0.5.5/smyg/cli.py
+-rw-r--r--   0        0        0      736 2023-02-28 14:40:14.827915 smyg-0.5.5/smyg/formatter.py
+-rw-r--r--   0        0        0     2214 2023-02-28 14:40:14.827915 smyg-0.5.5/smyg/metrics/code_changes.py
+-rw-r--r--   0        0        0     2247 2023-02-28 14:40:14.827915 smyg-0.5.5/smyg/metrics/code_churn.py
+-rw-r--r--   0        0        0     3806 2023-04-08 04:48:52.348220 smyg-0.5.5/smyg/prom.py
+-rw-r--r--   0        0        0      421 2023-02-28 14:40:14.827915 smyg-0.5.5/smyg/templates/code_changes.j2
+-rw-r--r--   0        0        0      244 2023-02-28 14:40:14.827915 smyg-0.5.5/smyg/templates/commit.j2
+-rw-r--r--   0        0        0      386 2023-04-11 06:13:52.004100 smyg-0.5.5/smyg/templates/commits.j2
+-rw-r--r--   0        0        0     1289 2023-02-28 14:40:14.827915 smyg-0.5.5/smyg/utils.py
+-rw-r--r--   0        0        0     7058 2023-04-11 06:13:52.004100 smyg-0.5.5/smyg/vcs.py
+-rw-r--r--   0        0        0     9088 1970-01-01 00:00:00.000000 smyg-0.5.5/setup.py
+-rw-r--r--   0        0        0     8884 1970-01-01 00:00:00.000000 smyg-0.5.5/PKG-INFO
```

### Comparing `smyg-0.5.4/LICENSE` & `smyg-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `smyg-0.5.4/README.md` & `smyg-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `smyg-0.5.4/pyproject.toml` & `smyg-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['poetry-core>=1.0.0']
 build-backend = 'poetry.core.masonry.api'
 
 [tool.poetry]
 name = 'smyg'
-version = '0.5.4'
+version = '0.5.5'
 description = 'git metric calculation'
 
 license = 'MIT'
 
 authors = [
   'Nikolay Mikhaylichenko <nn.mikh@yandex.ru>',
 ]
```

### Comparing `smyg-0.5.4/smyg/binding.py` & `smyg-0.5.5/smyg/binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     if sha:
         repo = pydriller.Repository(path,
                                     from_commit=sha,
                                     only_in_branch=branch,
                                     only_no_merge=True,
                                     order='reverse')
-        commits = list(repo.traverse_commits())[:-1]
+        commits = list(repo.traverse_commits())
     else:
         repo = pydriller.Repository(path,
                                     only_in_branch=branch,
                                     only_no_merge=True,
                                     order='reverse')
         commits = list(repo.traverse_commits())
     # ---
@@ -114,8 +114,9 @@
             committer_email=commit.committer.email,
             committer_date=commit.committer_date,
             project_name=commit.project_name,
             added=commit.insertions,
             deleted=commit.deletions,
             changed_files=commit.files,
             branches=commit.branches,
+            parents=commit.parents,
             )
```

### Comparing `smyg-0.5.4/smyg/cli.py` & `smyg-0.5.5/smyg/cli.py`

 * *Files identical despite different names*

### Comparing `smyg-0.5.4/smyg/formatter.py` & `smyg-0.5.5/smyg/formatter.py`

 * *Files identical despite different names*

### Comparing `smyg-0.5.4/smyg/metrics/code_changes.py` & `smyg-0.5.5/smyg/metrics/code_changes.py`

 * *Files identical despite different names*

### Comparing `smyg-0.5.4/smyg/metrics/code_churn.py` & `smyg-0.5.5/smyg/metrics/code_churn.py`

 * *Files identical despite different names*

### Comparing `smyg-0.5.4/smyg/prom.py` & `smyg-0.5.5/smyg/prom.py`

 * *Files identical despite different names*

### Comparing `smyg-0.5.4/smyg/utils.py` & `smyg-0.5.5/smyg/utils.py`

 * *Files identical despite different names*

### Comparing `smyg-0.5.4/smyg/vcs.py` & `smyg-0.5.5/smyg/vcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,14 +224,15 @@
     committer_email: str
     committer_date: datetime.datetime
     project_name: str
     added: int
     deleted: int
     changed_files: int
     branches: list
+    parents: list
 
     def as_dict(self) -> dict:
         '''Represent instance as dict'''
         return dataclasses.asdict(self)
 
     def as_seriable_dict(self) -> dict:
         '''Represent instance as seriable dict'''
```

### Comparing `smyg-0.5.4/setup.py` & `smyg-0.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['smyg = smyg.cli:app']}
 
 setup_kwargs = {
     'name': 'smyg',
-    'version': '0.5.4',
+    'version': '0.5.5',
     'description': 'git metric calculation',
     'long_description': '# ShowMeYourGit\n\n**showmeyourgit** (or smyg) is a project for calculating git metrics: added lines, deleted lines, commits count, changed files, code changes ratio, code churn ratio.\n\n## Installation\n\nUse the package manager [pip](https://pip.pypa.io/en/stable/) to install smyg.\n\n```bash\npip install --user smyg\n```\n\n## Usage\n\nClone [example project](https://github.com/nmix/example-project)\n```bash\ngit clone https://github.com/nmix/example-project.git\ncd example-project\n```\n\n### commit\n\n Show commit info\n\n```bash\n# --- show command help\n$ smyg commit --help\n\n# --- show last commit info for current branch\n$ smyg commit\ncdcb7c6ac0b92b1e16cfdd6f1e6abf0ed8f73e48 | update README\n2023-02-20 16:42:41+03:00 | Nikolay Mikhaylichenko\n[\'main\']\nAdded lines:       26\nDeleted lines:      0\nChanged files:      1\n\n# --- show last commit info in json format\n$ smyg commit --output json | jq\n{\n  "hash": "cdcb7c6ac0b92b1e16cfdd6f1e6abf0ed8f73e48",\n  "msg": "update README",\n  "author_name": "Nikolay Mikhaylichenko",\n  "author_email": "nn.mikh@yandex.ru",\n  "author_date": "2023-02-20 16:42:41+03:00",\n  "committer_name": "Nikolay Mikhaylichenko",\n  "committer_email": "nn.mikh@yandex.ru",\n  "committer_date": "2023-02-20 16:42:41+03:00",\n  "project_name": "example-project",\n  "added": 26,\n  "deleted": 0,\n  "changed_files": 1,\n  "branches": [\n    "main"\n  ]\n}\n\n# --- show info about arbitary commit\n$ smyg commit 07cb19ceba138f1d7e4a1d48f024e520f3657a1d\n07cb19ceba138f1d7e4a1d48f024e520f3657a1d | commit 2-1\n2023-02-20 16:26:48+03:00 | Nikolay Mikhaylichenko\n[\'branch-2\']\nAdded lines:        6\nDeleted lines:      0\nChanged files:      1\n```\n\n### branch-commits\n\nShow changes for bundle of commits in branch.\n\nIf we know last commit of previous bundle then we take all commits after that. In Gitlab CI previous commit SHA may be in `CI_COMMIT_BEFORE_SHA` environment variable (see [Predefined variables reference](https://docs.gitlab.com/ee/ci/variables/predefined_variables.html)).\n\nIf we dont have previous commit then we take only commits for *single* branch. *Signle* branch means that commit belongs only one branch. **Here it is mandatory to have a complete local copy of the repository with all branches.**\n\n```bash\n# --- show command help\n$ smyg branch-commits --help\n\n# --- if you just clone the example repository, the entire commit list will be displayed (from Initial commit)\n#     this is because only one branch is locally received and all commits belongs to it\n$ smyg branch-commits\n\ncdcb7c6ac0b92b1e16cfdd6f1e6abf0ed8f73e48 | update README\n2023-02-20 16:42:41+03:00 | Nikolay Mikhaylichenko\n[\'main\']\nAdded lines:       26\nDeleted lines:      0\nChanged files:      1\n\n7febdeea7b4f82d15f7fa0765c12f10928af7a1a | lorem ipsum in main\n2023-02-20 16:33:58+03:00 | Nikolay Mikhaylichenko\n[\'main\']\nAdded lines:        6\nDeleted lines:      0\nChanged files:      1\n\n# ... skip remaining commits\n\n# --- checkout branch-3 and repeat the command\n#     we get only 3 commits for the branch\n$ git checkout branch-3\nSwitched to a new branch \'branch-3\'\n$ smyg branch-commits\n\n414d13a92998f9de86dd60d41f05f092e64350f3 | commit 3-3\n2023-02-20 16:32:42+03:00 | Nikolay Mikhaylichenko\n[\'branch-3\']\nAdded lines:        2\nDeleted lines:      0\nChanged files:      1\n\n776206b033b8a149c4ee491ec9bee23273f98afc | commit 3-2\n2023-02-20 16:32:13+03:00 | Nikolay Mikhaylichenko\n[\'branch-3\']\nAdded lines:        2\nDeleted lines:      0\nChanged files:      1\n\naa4f97ed8366b8d72a0be2c1c114aa503b531190 | commit 3-1\n2023-02-20 16:31:54+03:00 | Nikolay Mikhaylichenko\n[\'branch-3\']\nAdded lines:        4\nDeleted lines:      0\nChanged files:      1\n\n# --- branch commits with previous SHA\n$ git checkout main\nsmyg branch-commits 5317cd6080033ae5a9ce3166095745e862a52c9d\n\ncdcb7c6ac0b92b1e16cfdd6f1e6abf0ed8f73e48 | update README\n2023-02-20 16:42:41+03:00 | Nikolay Mikhaylichenko\n[\'main\']\nAdded lines:       26\nDeleted lines:      0\nChanged files:      1\n\n7febdeea7b4f82d15f7fa0765c12f10928af7a1a | lorem ipsum in main\n2023-02-20 16:33:58+03:00 | Nikolay Mikhaylichenko\n[\'main\']\nAdded lines:        6\nDeleted lines:      0\nChanged files:      1\n\nbbead3ba03de57909ee622fac4b973de180f5e5f | Branch 2 (#2)\n\ncommit 2-1  | commit 2-2 | commit 2-3\n2023-02-20 16:29:39+03:00 | Nikolay Mikhaylichenko\n[\'branch-3\', \'main\']\nAdded lines:        8\nDeleted lines:      0\nChanged files:      1\n```\n\n### codechanges\n\nShow total added and deleted lines count for current ref.\n\n```bash\n# --- show command help\n$ smyg codechanges --help\n\n# --- changes for current ref\n$ smyg codechanges\nRatio (%):         11\nAdded lines:      107\nDeleted lines:     12\n\n# --- code changes between commits\n$ smyg codechanges --from-commit 3a085582e8df7c1d622c412eb54eb5ee96e82c48  \\\n  --to-commit bbead3ba03de57909ee622fac4b973de180f5e5f\nRatio (%):         42\nAdded lines:       26\nDeleted lines:     11\n```\n\n### codechurn\n\nShow count of added lines and count of deleted lines from those that were added. Displays the level of work that was not released.\n\n> Ideally, it should coincide with the codechanges for whole project history. For complex branching it may slightly different.\n\n```bash\n# --- show command help\n$ smyg codechurn --help\n\n# --- churn for current ref (equal with codechanges, it is expected)\nsmyg codechurn\nRatio (%):         11\nAdded lines:      107\nDeleted lines:     12\n\n# --- churn from specified commit (not equal with codechanges, it is expected)\n$ smyg codechurn --from-commit 44c6334f38fe796f38c39e1d11a8d19925684926 \\\n    --to-commit fccfa86625353409018ccd467f0050b57152656e\nRatio (%):         23\nAdded lines:       26\nDeleted lines:      6\n```\n\n## Prometheus Metrics\n\nYou can push metrics to Prometheus PushGateway. \nRecommended to use Aggregation Gateway like https://github.com/zapier/prom-aggregation-gateway.\n\n`commit` and `branch_commits` is a *Counter* type, `codechanges` and `codechurn` - *Gauge*. \n\nYou must specify environment variables `PUSHGATEWAY_URL` and `PROJECT_NAME` and command option `--push-metrics` to send metrics. For basic auth access specify `PUSHGATEWAY_USERNAME` and `PUSHGATEWAY_PASSWORD`.\n\n```bash\n$ git checkout main\n\n$ docker run --rm -p 8080:80 ghcr.io/zapier/prom-aggregation-gateway:v0.7.0\n\n$ PUSHGATEWAY_URL=localhost:8080 PROJECT_NAME=example_project \\\n    smyg commit --push-metrics\ncdcb7c6ac0b92b1e16cfdd6f1e6abf0ed8f73e48 | update README\n2023-02-20 16:42:41+03:00 | Nikolay Mikhaylichenko\n[\'main\']\nAdded lines:       26\nDeleted lines:      0\nChanged files:      1\n\n$ curl localhost:8080/metrics\n# HELP commit_added_lines_total Number of added lines in commit\n# TYPE commit_added_lines_total counter\ncommit_added_lines_total{author_email="nn.mikh@yandex.ru",author_name="Nikolay Mikhaylichenko",job="showmeyourgit",project_name="example_project"} 26\n# HELP commit_changed_files_total Number of changed files in commit\n# TYPE commit_changed_files_total counter\ncommit_changed_files_total{author_email="nn.mikh@yandex.ru",author_name="Nikolay Mikhaylichenko",job="showmeyourgit",project_name="example_project"} 1\n# HELP commit_deleted_lines_total Number of added deleted in commit\n# TYPE commit_deleted_lines_total counter\ncommit_deleted_lines_total{author_email="nn.mikh@yandex.ru",author_name="Nikolay Mikhaylichenko",job="showmeyourgit",project_name="example_project"} 0\n# HELP commits_total Number of commits\n# TYPE commits_total counter\ncommits_total{author_email="nn.mikh@yandex.ru",author_name="Nikolay Mikhaylichenko",job="showmeyourgit",project_name="example_project"} 1\n```\n\n## Develop & Test\n\n```bash\n$ git clone git@github.com:nmix/showmeyourgit.git\n$ cd showmeyourgit\n$ poetry install\n$ poetry shell\n$ pytest\n```\n\n## Contributing\n\nPull requests are welcome. For major changes, please open an issue first\nto discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n## License\n\n[MIT](https://choosealicense.com/licenses/mit/)\n',
     'author': 'Nikolay Mikhaylichenko',
     'author_email': 'nn.mikh@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nmix/showmeyourgit',
```

### Comparing `smyg-0.5.4/PKG-INFO` & `smyg-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smyg
-Version: 0.5.4
+Version: 0.5.5
 Summary: git metric calculation
 Home-page: https://github.com/nmix/showmeyourgit
 License: MIT
 Keywords: git,metrics
 Author: Nikolay Mikhaylichenko
 Author-email: nn.mikh@yandex.ru
 Requires-Python: >=3.7.2,<4.0.0
```

