# Comparing `tmp/pyalpa-0.5.1.tar.gz` & `tmp/pyalpa-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalpa-0.5.1.tar", max compression
+gzip compressed data, was "pyalpa-0.6.0.tar", max compression
```

## Comparing `pyalpa-0.5.1.tar` & `pyalpa-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-04-09 14:49:39.981480 pyalpa-0.5.1/LICENSE
--rw-r--r--   0        0        0     1631 2023-04-09 14:49:39.981480 pyalpa-0.5.1/README.md
--rw-r--r--   0        0        0        0 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/cli/__init__.py
--rw-r--r--   0        0        0      710 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/cli/alpa_repo.py
--rw-r--r--   0        0        0     1230 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/cli/base.py
--rw-r--r--   0        0        0     6330 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/cli/local_repo.py
--rw-r--r--   0        0        0        0 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/config/__init__.py
--rw-r--r--   0        0        0     1015 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/config/local_config.py
--rw-r--r--   0        0        0     2673 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/config/packit.py
--rw-r--r--   0        0        0      813 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/constants.py
--rw-r--r--   0        0        0      111 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/exceptions.py
--rw-r--r--   0        0        0     3579 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/gh.py
--rw-r--r--   0        0        0     1447 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/messages.py
--rw-r--r--   0        0        0    12955 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/repository.py
--rw-r--r--   0        0        0     3858 2023-04-09 14:49:39.981480 pyalpa-0.5.1/alpa/upstream_integration.py
--rw-r--r--   0        0        0      762 2023-04-09 14:49:39.981480 pyalpa-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 pyalpa-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 19:41:22.776185 pyalpa-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1631 2023-04-11 19:41:22.776185 pyalpa-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/cli/__init__.py
+-rw-r--r--   0        0        0      739 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/cli/alpa_repo.py
+-rw-r--r--   0        0        0     1249 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/cli/base.py
+-rw-r--r--   0        0        0     6351 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/cli/local_repo.py
+-rw-r--r--   0        0        0      227 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/config/__init__.py
+-rw-r--r--   0        0        0     1079 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/config/alpa_local.py
+-rw-r--r--   0        0        0     2184 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/config/alpa_repo.py
+-rw-r--r--   0        0        0     1157 2023-04-11 19:41:22.776185 pyalpa-0.6.0/alpa/config/base.py
+-rw-r--r--   0        0        0     2759 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/config/metadata.py
+-rw-r--r--   0        0        0     2790 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/config/packit.py
+-rw-r--r--   0        0        0     1233 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/constants.py
+-rw-r--r--   0        0        0      158 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/exceptions.py
+-rw-r--r--   0        0        0     3900 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/gh.py
+-rw-r--r--   0        0        0     1447 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/messages.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/repository/__init__.py
+-rw-r--r--   0        0        0    10659 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/repository/base.py
+-rw-r--r--   0        0        0     4400 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/repository/branch.py
+-rw-r--r--   0        0        0     1661 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/repository/subdirectory.py
+-rw-r--r--   0        0        0     3879 2023-04-11 19:41:22.780185 pyalpa-0.6.0/alpa/upstream_integration.py
+-rw-r--r--   0        0        0      866 2023-04-11 19:41:22.780185 pyalpa-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2525 1970-01-01 00:00:00.000000 pyalpa-0.6.0/PKG-INFO
```

### Comparing `pyalpa-0.5.1/LICENSE` & `pyalpa-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.1/README.md` & `pyalpa-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.1/alpa/cli/alpa_repo.py` & `pyalpa-0.6.0/alpa/cli/alpa_repo.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 
 
 from os import getcwd
 from pathlib import Path
 
 import click
 
-from alpa.repository import AlpaRepo
+from alpa.repository.branch import AlpaRepoBranch
 
 
 pkg_name = click.argument("name", type=str)
 
 
 @click.command("create")
 @pkg_name
 def create(name: str) -> None:
     """Create new package"""
-    AlpaRepo(Path(getcwd())).create_package(name)
+    AlpaRepoBranch(Path(getcwd())).create_package(name)
 
 
 @click.command("delete")
 @pkg_name
 def delete(name: str) -> None:
-    """Delete existing package"""
-    raise NotImplementedError("Not implemented yet (1.0 goal)")
+    """Request deleting existing package"""
+    AlpaRepoBranch(Path(getcwd())).request_package_delete(name)
 
 
 @click.command("request-package")
 @pkg_name
 def request_package(name: str) -> None:
     """Request new branch for new package in Alpa repo"""
     raise NotImplementedError("Not implemented yet (1.0 goal)")
```

### Comparing `pyalpa-0.5.1/alpa/cli/base.py` & `pyalpa-0.6.0/alpa/cli/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     list_,
     genspec,
     add,
     get_pkg_archive,
     mockbuild,
     create_packit_config,
 )
-from alpa.repository import AlpaRepo
+from alpa.repository.branch import AlpaRepoBranch
 
 # TODO: get rid of the repetitive _Repo(Path(getcwd()))
 
 
 @click.group()
 def entry_point() -> None:
     pass
@@ -28,15 +28,15 @@
 
 
 @entry_point.command("clone")
 @click.argument("url", type=str)
 @click.option("--fork", is_flag=True, default=False)
 def clone(url: str, fork: bool) -> None:
     """Clone and prepare Alpa repository"""
-    AlpaRepo.clone(url, fork)
+    AlpaRepoBranch.clone(url, fork)
 
 
 entry_point.add_command(create)
 entry_point.add_command(delete)
 entry_point.add_command(request_package)
 
 entry_point.add_command(show_history)
```

### Comparing `pyalpa-0.5.1/alpa/cli/local_repo.py` & `pyalpa-0.6.0/alpa/cli/local_repo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """
 These commands need to create LocalRepo -> no GH token required
 """
 
 
 from os import getcwd
 from pathlib import Path
-from typing import List
 
 import click
-from alpa_conf import MetadataConfig
 from click import ClickException, Choice
 from specfile import Specfile
 
-from alpa.config.packit import PackitConfig
-from alpa.repository import LocalRepo, AlpaRepo
+from alpa.config import MetadataConfig, PackitConfig
+from alpa.repository.branch import LocalRepoBranch, AlpaRepoBranch
 from alpa.upstream_integration import UpstreamIntegration
 
 pkg_name = click.argument("name", type=str)
 
 
 @click.command("show-history")
 @click.option(
@@ -30,23 +28,23 @@
 )
 def show_history(oneline: bool) -> None:
     """Show git history of current package"""
     params = []
     if oneline:
         params.append("--oneline")
 
-    local_repo = LocalRepo(Path(getcwd()))
+    local_repo = LocalRepoBranch(Path(getcwd()))
     click.echo(local_repo.get_history_of_branch(local_repo.branch, params))
 
 
 @click.command("switch")
 @pkg_name
 def switch(name: str) -> None:
     """Switch to specified package"""
-    LocalRepo(Path(getcwd())).switch_to_package(name)
+    LocalRepoBranch(Path(getcwd())).switch_to_package(name)
 
 
 @click.command("commit")
 @click.option(
     "-m",
     "--message",
     type=str,
@@ -55,37 +53,37 @@
 )
 @click.option("-n", "--no-verify", is_flag=True, help="Do not run pre-commit")
 def commit(message: str, no_verify: bool) -> None:
     """Commit your changes in your package's repository"""
     if len(message) > 80:
         raise ClickException("Message longer than 80 characters")
 
-    LocalRepo(Path(getcwd())).commit(message, not no_verify)
+    LocalRepoBranch(Path(getcwd())).commit(message, not no_verify)
 
 
 @click.command("add")
 @click.argument("files", type=str, nargs=-1, required=True)
-def add(files: List[str]) -> None:
+def add(files: list[str]) -> None:
     """Add files to git history. Basically calls `git add <input>`"""
-    LocalRepo(Path(getcwd())).add(files)
+    LocalRepoBranch(Path(getcwd())).add(files)
 
 
 @click.command("push")
 @click.option(
     "-p",
     "--pull-request",
     is_flag=True,
     show_default=True,
     default=False,
     help="This will create pull request on GitHub for you.",
 )
 def push(pull_request: bool) -> None:
     """Pushes your commited changes to the Alpa repo so you can make PR"""
     repo_path = Path(getcwd())
-    local_repo = LocalRepo(repo_path)
+    local_repo = LocalRepoBranch(repo_path)
 
     packit_conf = PackitConfig(local_repo.package)
     if not packit_conf.packit_config_file_exists():
         packit_conf.create_packit_config()
         local_repo.git_cmd.add(".packit.yaml")
         local_repo.git_cmd.commit(
             '-m "alpa: automatically add .packit.yaml config to the package"'
@@ -93,15 +91,15 @@
 
     local_repo.push(local_repo.branch)
 
     if not pull_request:
         local_repo.git_cmd.branch("-d", local_repo.feat_branch)
         return
 
-    alpa = AlpaRepo(repo_path)
+    alpa = AlpaRepoBranch(repo_path)
     pr = alpa.gh_repo.create_pr(
         title=f"[alpa-cli] Create update of package {local_repo.package}",
         body=(
             "This PR was created automatically via alpa-cli for "
             f"user {alpa.gh_api.gh_user}"
         ),
         source_branch=f"{local_repo.feat_branch}",
@@ -113,23 +111,23 @@
     local_repo.git_cmd.switch(local_repo.package)
     local_repo.git_cmd.branch("-D", local_repo.feat_branch)
 
 
 @click.command("pull")
 def pull() -> None:
     """Pull last recent changes of package you are on from Alpa repo"""
-    local_repo = LocalRepo(Path(getcwd()))
+    local_repo = LocalRepoBranch(Path(getcwd()))
     local_repo.pull(local_repo.branch)
 
 
 @click.command("list")
 @click.option("-p", "--pattern", type=str, default="", help="Optional pattern to match")
 def list_(pattern: str) -> None:
     """List all packages or packages matching regex"""
-    for pkg in LocalRepo(Path(getcwd())).get_packages(pattern):
+    for pkg in LocalRepoBranch(Path(getcwd())).get_packages(pattern):
         click.echo(pkg)
 
 
 @click.command("genspec")
 @click.option(
     "--lang",
     type=Choice(["python", "java"], case_sensitive=False),
@@ -156,15 +154,15 @@
     is_flag=True,
     show_default=True,
     default=False,
     help="Override packit config file",
 )
 def create_packit_config(override: bool) -> None:
     """Creates packit config based on metadata.yaml file in package"""
-    if not LocalRepo(Path(getcwd())).create_packit_config(override):
+    if not LocalRepoBranch(Path(getcwd())).create_packit_config(override):
         raise ClickException(
             "Packit file already exists. To override it use --override flag."
         )
 
 
 def _get_chroots_to_build(meta: MetadataConfig, distros: list[str]) -> list[str]:
     chroots = []
```

### Comparing `pyalpa-0.5.1/alpa/config/local_config.py` & `pyalpa-0.6.0/alpa/config/alpa_local.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,41 @@
+"""
+Class for local cli config
+"""
+
+
 from os.path import isfile
 from pathlib import Path
 from typing import Optional
 
 from yaml import safe_load
 
 from alpa.constants import CONFIG_FILE_LOCATIONS
 
 
-class Config:
+class AlpaLocalConfig:
     def __init__(self, gh_api_token: str) -> None:
         self.gh_api_token = gh_api_token
 
     @staticmethod
     def _get_config_file_path() -> Optional[Path]:
         for location in CONFIG_FILE_LOCATIONS:
             expanded_path = Path(location).expanduser()
             if isfile(str(expanded_path)):
                 return expanded_path
 
         return None
 
     @classmethod
-    def get_config(cls, repo_name: str) -> Optional["Config"]:
+    def get_config(cls, repo_name: str) -> Optional["AlpaLocalConfig"]:
         cfg_file_path = cls._get_config_file_path()
         if cfg_file_path is None:
             return None
 
         with open(cfg_file_path) as alpa_cfg_file:
             config_dict = safe_load(alpa_cfg_file)
 
         for item in config_dict["api_keys"]:
             if item["repo"]["name"] == repo_name:
-                return Config(gh_api_token=item["repo"]["key"])
+                return AlpaLocalConfig(gh_api_token=item["repo"]["key"])
 
         return None
```

### Comparing `pyalpa-0.5.1/alpa/config/packit.py` & `pyalpa-0.6.0/alpa/config/packit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+"""
+Class that generates packit.yaml config based on other configs like
+Alpa repo or package metadata config
+"""
+
+
 from os import getcwd
 from pathlib import Path
 
 from yaml import dump
 
-from alpa_conf import AlpaRepoConfig, MetadataConfig
+from alpa.config import AlpaRepoConfig, MetadataConfig
 
 from alpa.constants import PACKIT_CONFIG_NAMES
 
 
 class PackitConfig:
     def __init__(self, package_name: str) -> None:
         self.package_name = package_name
```

### Comparing `pyalpa-0.5.1/alpa/gh.py` & `pyalpa-0.6.0/alpa/gh.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
-Integration with GitHub API.
+Wrapper aroung pygithub API since the documentation is awful..
 """
 
 
 from os import getenv
 from typing import Optional
 
 import click
 from click import UsageError
 from github import Github, Issue, PullRequest, UnknownObjectException
 
-from alpa.config.local_config import Config
+from alpa.config.alpa_local import AlpaLocalConfig
 from alpa.constants import GH_API_TOKEN_NAME, GH_WRITE_ACCESS
 from alpa.messages import NO_GH_API_KEY_FOUND, RETURNING_CLONE_URL_MSG
 
 
 class GithubRepo:
     def __init__(self, api: Github, namespace: str, repo_name: str) -> None:
         self.namespace = namespace
@@ -89,32 +89,38 @@
     def pr_exists(self, id: int) -> bool:
         try:
             self._repo.get_pull(id)
             return True
         except UnknownObjectException:
             return False
 
+    def get_issues(self, state: str, labels: list[str]) -> list[Issue]:
+        return list(self._repo.get_issues(state=state, labels=labels))
+
 
 class GithubAPI:
-    def __init__(self, repo_name: str) -> None:
-        self._gh_api = Github(self._get_access_token(repo_name))
+    def __init__(self, repo_name: str, gh_token: Optional[str] = None) -> None:
+        if gh_token is not None:
+            self._gh_api = Github(gh_token)
+        else:
+            self._gh_api = Github(self._get_access_token(repo_name))
 
     @property
     def gh_user(self) -> str:
         return self._gh_api.get_user().login
 
     @staticmethod
     def _get_access_token(repo_name: str) -> str:
         access_token_env = getenv(GH_API_TOKEN_NAME)
         if access_token_env is not None:
             return access_token_env
 
         # accessing config file here since it does not make sense to do it elsewhere,
         # but in the future the config will be useful in many places
-        access_token_config = Config.get_config(repo_name)
+        access_token_config = AlpaLocalConfig.get_config(repo_name)
         if access_token_config is None:
             raise UsageError(NO_GH_API_KEY_FOUND.format(token=GH_API_TOKEN_NAME))
 
         return access_token_config.gh_api_token
 
     def get_repo(self, namespace: str, repo_name: str) -> GithubRepo:
         return GithubRepo(self._gh_api, namespace, repo_name)
```

### Comparing `pyalpa-0.5.1/alpa/messages.py` & `pyalpa-0.6.0/alpa/messages.py`

 * *Files identical despite different names*

### Comparing `pyalpa-0.5.1/alpa/repository.py` & `pyalpa-0.6.0/alpa/repository/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """
 Set of commands that helps with integration of Alpa
 repository.
 """
 import subprocess
+from abc import ABC, abstractmethod
 from os import getcwd, environ
 from pathlib import Path
-import re
 from subprocess import call
 from tempfile import NamedTemporaryFile
-from typing import List, Optional, Iterable
+from typing import Optional, Iterable
 from urllib.parse import urlparse
 
 from click import UsageError, ClickException
 import click
-from git import Repo, Remote, GitCommandError
+from git import Repo, Remote
 
-from alpa.config.packit import PackitConfig
 from alpa.constants import (
     ALPA_FEAT_BRANCH,
     ALPA_FEAT_BRANCH_PREFIX,
-    MAIN_BRANCH,
     ORIGIN_NAME,
     UPSTREAM_NAME,
-    PackageRequest,
 )
 from alpa.gh import GithubAPI, GithubRepo
 from alpa.messages import (
     CLONED_REPO_IS_NOT_FORK,
-    NO_WRITE_ACCESS_ERR,
     NOT_IN_PREDEFINED_STATE,
     CLONED_REPO_IS_FORK,
     NO_PERMISSION_FOR_ALPA_REPO,
 )
 
 
-class LocalRepo:
+class LocalRepo(ABC):
     def __init__(self, repo_path: Path) -> None:
         self.repo_path = repo_path
         # TODO: this will differ in the future with repo_path
         self.repo_root_path = repo_path
         self.local_repo = Repo(str(self.repo_path), search_parent_directories=True)
         self.git_cmd = self.local_repo.git
 
@@ -48,27 +44,49 @@
         # do it after predefined state is checked since this depends on it
         # (see comment in the _should_be_fork)
         self.remote_name = UPSTREAM_NAME if self._should_be_fork() else ORIGIN_NAME
 
         # lazy properties
         self._namespace: Optional[str] = None
         self._repo_name: Optional[str] = None
+        self._git_root: Optional[Path] = None
+
+    @abstractmethod
+    def get_packages(self, regex: str) -> list[str]:
+        pass
+
+    @abstractmethod
+    def switch_to_package(self, package: str) -> None:
+        pass
+
+    @abstractmethod
+    def _ensure_feature_branch(self) -> None:
+        pass
+
+    @abstractmethod
+    def get_history_of_package(self, package: str) -> str:
+        pass
+
+    @property
+    @abstractmethod
+    def package(self) -> str:
+        pass
+
+    @abstractmethod
+    def create_packit_config(self, override: bool) -> bool:
+        pass
 
     @property
     def remote_associated_with_current_branch(self) -> str:
         return self.local_repo.active_branch.tracking_branch().remote_name
 
     @property
     def branch(self) -> str:
         return self.local_repo.active_branch.name
 
-    @property
-    def package(self) -> str:
-        return self.branch.removeprefix(ALPA_FEAT_BRANCH_PREFIX)
-
     @staticmethod
     def get_feat_branch_of_package(package: str) -> str:
         return ALPA_FEAT_BRANCH.format(pkgname=package)
 
     @property
     def feat_branch(self) -> str:
         return ALPA_FEAT_BRANCH.format(pkgname=self.package)
@@ -79,15 +97,15 @@
         for ref in remote_refs:
             parsed_ref = ref.split("/")[-1]
             if not parsed_ref.startswith(ALPA_FEAT_BRANCH_PREFIX):
                 relevant_refs.append(parsed_ref)
 
         return relevant_refs
 
-    def show_remote_branches(self, remote: str) -> List[str]:
+    def get_remote_branches(self, remote: str) -> list[str]:
         lines = [
             line.strip()
             for line in self.git_cmd.remote("--verbose", "show", remote).split("\n")
         ]
         # TODO: do a better job
         remote_branch_line = ["Remote branch:", "Remote branches:"]
         start = -1
@@ -114,27 +132,14 @@
 
         if end == -1:
             end = len(lines)
 
         lines_with_remote_branches = lines[start + 1 : end]
         return [line.split()[0] for line in lines_with_remote_branches]
 
-    def get_packages(self, regex: str) -> List[str]:
-        # self.local_repo.remote(name=self.remote_name).refs don't work on every case
-        refs_without_main = filter(
-            lambda ref: ref != "main", self.show_remote_branches(self.remote_name)
-        )
-        relevant_refs = self._get_relevant_remote_refs(refs_without_main)
-
-        if regex == "":
-            return list(relevant_refs)
-
-        pattern = re.compile(regex)
-        return [ref for ref in relevant_refs if pattern.match(ref)]
-
     def _is_repo_in_predefined_state(self) -> bool:
         remotes_name_set = {remote.name for remote in self.local_repo.remotes}
         return remotes_name_set == {ORIGIN_NAME, UPSTREAM_NAME} or remotes_name_set == {
             ORIGIN_NAME
         }
 
     def _should_be_fork(self) -> bool:
@@ -209,57 +214,28 @@
     def branch_exists(self, branch: str) -> bool:
         for ref in self.local_repo.references:
             if ref.name == branch:
                 return True
 
         return False
 
-    def switch_to_package(self, package: str) -> None:
-        if self.local_repo.is_dirty():
-            click.echo(
-                "Repo is dirty, please commit your changes before switching to"
-                f" another package.\n {self.get_status_output()}"
-            )
-            return None
-
-        feat_branch = self.get_feat_branch_of_package(package)
-        branch_to_switch = feat_branch if self.branch_exists(feat_branch) else package
-        try:
-            click.echo(
-                self.git_cmd.switch(branch_to_switch).replace("branch", "package")
-            )
-        except GitCommandError:
-            # switching to the package for the first time
-            click.echo(f"Switching to the package {package} for the first time")
-            click.echo(self.git_cmd.fetch(self.remote_name, branch_to_switch))
-            click.echo(
-                self.git_cmd.switch(branch_to_switch).replace("branch", "package")
-            )
-
-    def get_history_of_branch(self, branch: str, *params: List[str]) -> str:
+    def get_history_of_branch(self, branch: str, *params: list[str]) -> str:
         return self.git_cmd.log("--decorate", "--graph", *params, branch)
 
     @staticmethod
     def _get_message_from_editor() -> str:
         with NamedTemporaryFile(suffix=".alpa.tmp") as temp_file:
             call([environ.get("EDITOR", "vim"), temp_file.name])
             temp_file.seek(0)
             output = temp_file.read()
             if isinstance(output, (bytes, bytearray)):
                 return output.decode("utf-8")
 
             return output
 
-    def _ensure_feature_branch(self) -> None:
-        if self.branch != self.package:
-            return None
-
-        click.echo("Switching to feature branch")
-        self.git_cmd.switch("-c", self.feat_branch)
-
     def commit(self, message: str, pre_commit: bool) -> bool:
         if pre_commit:
             ret = subprocess.run(["pre-commit", "run", "--all-files"])
             if ret.returncode != 0:
                 return False
 
         self._ensure_feature_branch()
@@ -267,15 +243,15 @@
         if message:
             index.commit(message)
         else:
             index.commit(self._get_message_from_editor())
 
         return True
 
-    def add(self, files: List[str]) -> None:
+    def add(self, files: list[str]) -> None:
         self._ensure_feature_branch()
         # FIXME: alpa add . acts weird
         self.git_cmd.add(files)
 
     def pull(self, branch: str) -> None:
         click.echo(self.git_cmd.pull(self.remote_name, branch))
 
@@ -286,58 +262,40 @@
     def full_reponame(self) -> str:
         for remote in self.local_repo.remotes:
             if remote.name == self.remote_name:
                 return remote.url.split(":")[-1].removesuffix(".git")
 
         return ""
 
-    def create_packit_config(self, override: bool) -> bool:
-        packit_conf = PackitConfig(self.package)
-        if packit_conf.packit_config_file_exists() and not override:
-            return False
-
-        packit_conf.create_packit_config()
-        return True
+    @property
+    def git_root(self) -> Optional[Path]:
+        if self._git_root is not None:
+            return self._git_root
 
-    def get_git_root(self) -> Optional[Path]:
-        return Path(self.local_repo.working_tree_dir)
+        self._git_root = Path(self.local_repo.working_tree_dir)
+        return self._git_root
 
 
 class AlpaRepo(LocalRepo):
     def __init__(self, repo_path: Path, gh_api: Optional[GithubAPI] = None) -> None:
         super().__init__(repo_path)
 
         self.gh_api = gh_api or GithubAPI(self.repo_name)
         self.gh_repo = self.gh_api.get_repo(self.namespace, self.repo_name)
 
+    @abstractmethod
     def create_package(self, package: str) -> None:
-        upstream = self.gh_repo.get_upstream()
-        if upstream and not upstream.has_write_access(self.gh_api.gh_user):
-            raise ClickException(NO_WRITE_ACCESS_ERR)
-
-        self.git_cmd.switch(MAIN_BRANCH)
-        self.git_cmd.switch("-c", package)
-        self.git_cmd.push(self.remote_name, package)
-        click.echo(f"Package {package} created")
+        pass
 
+    @abstractmethod
     def request_package(self, package_name: str) -> None:
-        ensured_upstream = self.gh_repo.get_root_repo()
-        upstream_namespace = ensured_upstream.namespace
-        issue_repo = self.gh_api.get_repo(upstream_namespace, self.gh_repo.repo_name)
-        issue = issue_repo.create_issue(
-            PackageRequest.TITLE.value.format(package_name=package_name),
-            PackageRequest.BODY.value.format(
-                user=self.gh_api.gh_user,
-                package_name=package_name,
-                repo_name=self.gh_repo.repo_name,
-            ),
-        )
-        issue.add_to_labels(PackageRequest.LABEL)
+        pass
 
-    def delete_package(self) -> None:
+    @abstractmethod
+    def request_package_delete(self, package: str) -> None:
         pass
 
     @staticmethod
     def _prepare_cloned_repo(local_repo: Repo, gh_repo: GithubRepo) -> None:
         if not gh_repo.is_fork:
             return
```

### Comparing `pyalpa-0.5.1/alpa/upstream_integration.py` & `pyalpa-0.6.0/alpa/upstream_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 import shutil
 import subprocess
 from pathlib import Path
 from typing import Optional
 
 import click
 import requests
-from alpa_conf import MetadataConfig
+from alpa.config import MetadataConfig
 from click import ClickException
 from specfile import Specfile
 
-from alpa.repository import LocalRepo
+from alpa.repository.branch import LocalRepoBranch
 
 
-class UpstreamIntegration(LocalRepo):
+class UpstreamIntegration(LocalRepoBranch):
     def __init__(self, repo_path: Path) -> None:
         super().__init__(repo_path)
         self.metadata = MetadataConfig.get_config(repo_path)
         self.specfile = Specfile(Path(repo_path / f"{self.package}.spec"))
         self.name_version = (
             f"{self.specfile.expanded_name}-{self.specfile.expanded_version}"
         )
```

### Comparing `pyalpa-0.5.1/pyproject.toml` & `pyalpa-0.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyalpa"
-version = "0.5.1"
+version = "0.6.0"
 description = "Integration tool with Alpa repository"
 authors = ["Jiri Kyjovsky <j1.kyjovsky@gmail.com>"]
 maintainers = ["Jiří Kyjovský <j1.kyjovsky@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/alpa-team/alpa"
 repository = "https://github.com/alpa-team/alpa"
@@ -14,22 +14,30 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = ">=8.0.0"
 gitpython = ">=3.0"
 pygithub = ">=1.4"
 pyyaml = ">=5.0"
-alpa-conf = ">=0.4.0"
 specfile = ">=0.13.0"
+pydantic = ">=1.8"
+email-validator = ">=1.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.0.0"
+pyfakefs = ">=4.0.0"
+mypy = ">=0.900"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
+
 [tool.poetry.scripts]
 alpa = "alpa.cli.base:entry_point"
+
+
+[tool.mypy]
+plugins = ["pydantic.mypy"]
```

### Comparing `pyalpa-0.5.1/PKG-INFO` & `pyalpa-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pyalpa
-Version: 0.5.1
+Version: 0.6.0
 Summary: Integration tool with Alpa repository
 Home-page: https://github.com/alpa-team/alpa
 License: GPLv3
 Author: Jiri Kyjovsky
 Author-email: j1.kyjovsky@gmail.com
 Maintainer: Jiří Kyjovský
 Maintainer-email: j1.kyjovsky@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: alpa-conf (>=0.4.0)
 Requires-Dist: click (>=8.0.0)
+Requires-Dist: email-validator (>=1.0)
 Requires-Dist: gitpython (>=3.0)
+Requires-Dist: pydantic (>=1.8)
 Requires-Dist: pygithub (>=1.4)
 Requires-Dist: pyyaml (>=5.0)
 Requires-Dist: specfile (>=0.13.0)
 Project-URL: Repository, https://github.com/alpa-team/alpa
 Description-Content-Type: text/markdown
 
 ## Alpa
```

