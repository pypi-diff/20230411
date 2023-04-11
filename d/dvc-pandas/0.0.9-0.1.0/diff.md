# Comparing `tmp/dvc-pandas-0.0.9.tar.gz` & `tmp/dvc-pandas-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/bernhard/Kausal/dvc-pandas/dist/tmp02n8nhqm/dvc-pandas-0.0.9.tar", last modified: Fri Jul 16 16:25:16 2021, max compression
+gzip compressed data, was "dvc-pandas-0.1.0.tar", last modified: Tue Apr 11 16:37:11 2023, max compression
```

## Comparing `dvc-pandas-0.0.9.tar` & `dvc-pandas-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 bernhard  (1000) bernhard  (1000)        0 2021-07-16 16:25:16.000000 dvc-pandas-0.0.9/
-drwxr-xr-x   0 bernhard  (1000) bernhard  (1000)        0 2021-07-16 16:25:16.000000 dvc-pandas-0.0.9/src/
-drwxr-xr-x   0 bernhard  (1000) bernhard  (1000)        0 2021-07-16 16:25:16.000000 dvc-pandas-0.0.9/src/dvc_pandas/
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)      154 2021-06-10 08:17:20.000000 dvc-pandas-0.0.9/src/dvc_pandas/__init__.py
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)     2886 2021-07-15 13:36:53.000000 dvc-pandas-0.0.9/src/dvc_pandas/dataset.py
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)      352 2021-06-10 08:17:20.000000 dvc-pandas-0.0.9/src/dvc_pandas/dvc.py
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)     2452 2021-06-14 08:15:43.000000 dvc-pandas-0.0.9/src/dvc_pandas/git.py
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)     9242 2021-07-16 16:23:48.000000 dvc-pandas-0.0.9/src/dvc_pandas/repository.py
-drwxr-xr-x   0 bernhard  (1000) bernhard  (1000)        0 2021-07-16 16:25:16.000000 dvc-pandas-0.0.9/src/dvc_pandas.egg-info/
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)      593 2021-07-16 16:25:16.000000 dvc-pandas-0.0.9/src/dvc_pandas.egg-info/PKG-INFO
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)      366 2021-07-16 16:25:16.000000 dvc-pandas-0.0.9/src/dvc_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)        1 2021-07-16 16:25:16.000000 dvc-pandas-0.0.9/src/dvc_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)       79 2021-07-16 16:25:16.000000 dvc-pandas-0.0.9/src/dvc_pandas.egg-info/requires.txt
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)       11 2021-07-16 16:25:16.000000 dvc-pandas-0.0.9/src/dvc_pandas.egg-info/top_level.txt
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)     1068 2021-03-29 11:36:09.000000 dvc-pandas-0.0.9/LICENSE
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)       13 2021-03-29 11:36:27.000000 dvc-pandas-0.0.9/README.md
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)      304 2021-06-10 08:17:20.000000 dvc-pandas-0.0.9/pyproject.toml
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)     1011 2021-07-16 16:25:16.000000 dvc-pandas-0.0.9/setup.cfg
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)      120 2021-03-30 08:00:24.000000 dvc-pandas-0.0.9/setup.py
--rw-r--r--   0 bernhard  (1000) bernhard  (1000)      593 2021-07-16 16:25:16.000000 dvc-pandas-0.0.9/PKG-INFO
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/
+-rw-rw-r--   0 jey       (1000) jey       (1000)     1068 2021-04-06 11:20:04.000000 dvc-pandas-0.1.0/LICENSE
+-rw-rw-r--   0 jey       (1000) jey       (1000)      556 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/PKG-INFO
+-rw-rw-r--   0 jey       (1000) jey       (1000)       13 2021-04-06 11:20:04.000000 dvc-pandas-0.1.0/README.md
+-rw-rw-r--   0 jey       (1000) jey       (1000)      304 2022-02-09 06:54:41.000000 dvc-pandas-0.1.0/pyproject.toml
+-rw-rw-r--   0 jey       (1000) jey       (1000)     1026 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/setup.cfg
+-rw-rw-r--   0 jey       (1000) jey       (1000)      120 2021-04-06 11:20:04.000000 dvc-pandas-0.1.0/setup.py
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/src/
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/src/dvc_pandas/
+-rw-rw-r--   0 jey       (1000) jey       (1000)      154 2021-06-12 14:42:57.000000 dvc-pandas-0.1.0/src/dvc_pandas/__init__.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)     3606 2023-01-24 20:05:52.000000 dvc-pandas-0.1.0/src/dvc_pandas/dataset.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)      352 2021-06-12 14:42:57.000000 dvc-pandas-0.1.0/src/dvc_pandas/dvc.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)     2705 2023-04-11 14:35:40.000000 dvc-pandas-0.1.0/src/dvc_pandas/git.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)    13448 2023-04-11 16:35:22.000000 dvc-pandas-0.1.0/src/dvc_pandas/repository.py
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/src/dvc_pandas.egg-info/
+-rw-rw-r--   0 jey       (1000) jey       (1000)      556 2023-04-11 16:37:11.000000 dvc-pandas-0.1.0/src/dvc_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 jey       (1000) jey       (1000)      413 2023-04-11 16:37:11.000000 dvc-pandas-0.1.0/src/dvc_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 jey       (1000) jey       (1000)        1 2023-04-11 16:37:11.000000 dvc-pandas-0.1.0/src/dvc_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 jey       (1000) jey       (1000)       92 2023-04-11 16:37:11.000000 dvc-pandas-0.1.0/src/dvc_pandas.egg-info/requires.txt
+-rw-rw-r--   0 jey       (1000) jey       (1000)       11 2023-04-11 16:37:11.000000 dvc-pandas-0.1.0/src/dvc_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-04-11 16:37:11.267756 dvc-pandas-0.1.0/tests/
+-rw-rw-r--   0 jey       (1000) jey       (1000)      941 2021-10-08 15:22:36.000000 dvc-pandas-0.1.0/tests/test_dataset.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)     7606 2021-06-12 14:42:57.000000 dvc-pandas-0.1.0/tests/test_repository.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dvc-pandas-0.0.9/src/dvc_pandas/dataset.py` & `dvc-pandas-0.1.0/src/dvc_pandas/dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 from datetime import datetime
 from typing import Dict, Optional
 import pandas as pd
-from pint_pandas import PintArray
-
-
-def _quantify_series(series, unit):
-    if unit:
-        return PintArray(series, unit)
-    return series
+from pint_pandas import PintType
 
 
 class Dataset:
     df: pd.DataFrame
     identifier: str
     modified_at: Optional[datetime]
     units: Optional[Dict[str, str]]
@@ -36,26 +30,42 @@
             raise ValueError("Dataset metadata may not contain the key 'units'.")
         if units is not None:
             for column in units.keys():
                 if column not in df.columns:
                     raise ValueError(f"Unit specified for unknown column name '{column}'.")
 
         if units:
-            self.df = pd.DataFrame({
-                column: _quantify_series(df[column], units.get(column))
-                for column in df.columns
-            })
+            df = df.copy()
+            for col, unit in units.items():
+                df[col] = df[col].astype(PintType(unit))
+            self.df = df
         else:
+            if not metadata or 'units' not in metadata:
+                units = self._determine_pint_units(df)
             self.df = df.copy()
 
         self.identifier = identifier
         self.units = units
         self.metadata = metadata
         self.modified_at = modified_at
 
+    def _determine_pint_units(self, df: pd.DataFrame) -> Optional[Dict[str, str]]:
+        """Determine units from pint DataFrames."""
+
+        if not hasattr(df, 'pint'):
+            return None
+        units = {}
+        for col in df.columns:
+            if not hasattr(df[col], 'pint'):
+                continue
+            units[col] = str(df[col].pint.units)
+        if not units:
+            return None
+        return units
+
     def copy(self):
         return Dataset(self.df, self.identifier, units=self.units, metadata=self.metadata)
 
     @property
     def dvc_metadata(self) -> Optional[Dict]:
         """
         Return the metadata as it should be stored in the .dvc file.
@@ -67,13 +77,22 @@
         metadata = {}
         if self.metadata is not None:
             metadata = self.metadata
         if self.units is not None:
             metadata['units'] = self.units
         return metadata
 
+    def to_parquet(self, path: str):
+        df = self.df.copy()
+        # Strip units from pint dataframes before serialization.
+        for col in df.columns:
+            if not hasattr(df[col], 'pint'):
+                continue
+            df[col] = df[col].pint.m
+        df.to_parquet(path)
+
     def equals(self, other: pd.DataFrame) -> bool:
         compare_attrs = ('identifier', 'units', 'metadata')
         return self.df.equals(other.df) and all(getattr(self, a) == getattr(other, a) for a in compare_attrs)
 
     def __str__(self):
         return self.identifier
```

### Comparing `dvc-pandas-0.0.9/src/dvc_pandas/git.py` & `dvc-pandas-0.1.0/src/dvc_pandas/git.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,29 +2,35 @@
 import hashlib
 import logging
 import os
 from appdirs import user_cache_dir
 from pathlib import Path
 
 logger = logging.getLogger(__name__)
+GitRepo = git.Repo
 
 DEFAULT_CACHE_ROOT = user_cache_dir('dvc-pandas', 'kausaltech')
 PUSH_SUCCEEDED_FLAGS = git.remote.PushInfo.FAST_FORWARD | git.remote.PushInfo.NEW_HEAD
 
 
-def cache_dir_for_url(url, cache_root=None):
+def cache_dir_for_url(url, prefix: str | None = None, cache_root: str | None = None):
     """Return directory within the given cache_root directory for the given URL."""
     if cache_root is None:
         cache_root = DEFAULT_CACHE_ROOT
 
     dir_name = hashlib.md5(str(url).encode('utf-8')).hexdigest()
-    return Path(cache_root) / dir_name
+    p = Path(cache_root)
+    if prefix:
+        p /= prefix
+    return p / dir_name
 
 
-def local_cache_dir(location=None, cache_local_repository=False, cache_root=None):
+def local_cache_dir(
+    location: str | None = None, prefix: str | None = None, cache_local_repository: bool = False,
+    cache_root: str | None = None):
     """
     Return local repository directory for `location`.
 
     If `location` is a URL, returns the corresponding directory in the cache.
     If it is a path to a local directory and cache_local_repository is False,
     returns the directory.
     """
@@ -34,33 +40,33 @@
         except KeyError:
             raise Exception("No repository location provided and DVC_PANDAS_REPOSITORY not set")
 
     # Don't use cache if location is a local repository
     if not cache_local_repository and Path(location).exists():
         return location
 
-    return cache_dir_for_url(location, cache_root)
+    return cache_dir_for_url(location, prefix=prefix, cache_root=cache_root)
 
 
-def get_cache_repo(location=None, cache_local_repository=False, cache_root=None) -> git.Repo:
+def get_cache_repo(location=None, prefix: str | None = None, cache_local_repository=False, cache_root=None) -> GitRepo:
     """
     Return git repository for the given location, which can either be a URL or a path to a local repository.
 
     If given a URL and the repository does not exist in the cache, clones it first into the cache.
     """
-    repo_dir = local_cache_dir(location, cache_local_repository=cache_local_repository, cache_root=cache_root)
+    repo_dir = local_cache_dir(location, prefix=prefix, cache_local_repository=cache_local_repository, cache_root=cache_root)
     try:
         repo = git.Repo(repo_dir)
     except git.exc.NoSuchPathError:
         logger.debug(f"Clone git repository {location} to {repo_dir}")
         repo = git.Repo.clone_from(location, repo_dir)
     return repo
 
 
-def push(repo):
+def push(repo: GitRepo):
     """Push to remote; raise an exception if it failed."""
     result, = repo.remote().push()
     # We don't accept any flags except those in PUSH_SUCCEEDED_FLAGS, and there should be at least one of them
     success_flags = result.flags & PUSH_SUCCEEDED_FLAGS
     fail_flags = result.flags ^ success_flags
     if fail_flags or not success_flags:
         raise Exception(f"Push to git repository failed: {result.summary}")
```

### Comparing `dvc-pandas-0.0.9/src/dvc_pandas/repository.py` & `dvc-pandas-0.1.0/src/dvc_pandas/repository.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,142 +1,232 @@
+from __future__ import annotations
+from contextlib import contextmanager
+from hashlib import md5
+
+import git
+import gitdb
 import logging
 import os
-from pathlib import Path
 from datetime import datetime, timezone
-from typing import List, Optional, TYPE_CHECKING
+from pathlib import Path
+from typing import List, Optional
 
+import fasteners
 import pandas as pd
 from ruamel.yaml import YAML
 
 import dvc.repo
 
 from .dataset import Dataset
 from .dvc import set_dvc_file_metadata
-from .git import get_cache_repo
+from .git import get_cache_repo, GitRepo
 from .git import push as git_push
 
 logger = logging.getLogger(__name__)
 
 
 class TemporaryGitCheckout:
-    def __init__(self, repo, commit_id=None):
+    def __init__(self, repo: GitRepo, commit_id: str | None = None):
         self.repo = repo
         self.commit_id = commit_id
         self.original_branch = None
 
     def __enter__(self):
         if self.commit_id:
-            self.original_branch = self.repo.active_branch
-            self.repo.head.reference = self.repo.commit(self.commit_id)
+            try:
+                self.original_branch = self.repo.active_branch
+            except TypeError:
+                self.original_branch = None
+
+            try:
+                self.repo.head.reference = self.repo.commit(self.commit_id)
+            except (git.exc.BadName, gitdb.exc.BadObject, ValueError, IndexError):
+                logger.debug("Commit does not exist; pull and retry")
+                # Commit doesn't exist, try to pull and see what happens
+                self.repo.remote().pull()
+                self.repo.head.reference = self.repo.commit(self.commit_id)
             self.repo.head.reset(index=True, working_tree=True)
+            # TODO: Pull if commit ID doesn't exist? Flag for enabling this beha
 
     def __exit__(self, *exc):
         if self.original_branch:
             self.original_branch.checkout()
 
 
+class ReentrantLock:
+    """Lock that keeps track of invocations."""
+    process_lock: fasteners.InterProcessLock
+    thread_lock: fasteners.ReaderWriterLock
+
+    def __init__(self, lock_file: str):
+        self.process_lock = fasteners.InterProcessLock(lock_file)
+        self.thread_lock = fasteners.ReaderWriterLock()
+        self.acquisition_count = 0
+
+    @contextmanager
+    def lock(self):
+        with self.thread_lock.write_lock():
+            if not self.acquisition_count:
+                self.process_lock.acquire()
+            self.acquisition_count += 1
+            yield
+            assert self.acquisition_count >= 1
+            self.acquisition_count -= 1
+            if not self.acquisition_count:
+                self.process_lock.release()
+
+def ensure_repo_lock(func):
+    """Wrap a Repository class method with a lock."""
+    def acquire_lock(self: Repository, *args, **kwargs):
+        with self.lock.lock():
+            return func(self, *args, **kwargs)
+
+    return acquire_lock
+
+
 class DatasetStageItem:
     def __init__(self, dataset):
         self.identifier = dataset.identifier
         self.metadata = dataset.dvc_metadata
 
 
 class Repository:
     dvc_remote: Optional[str]
-    repo_url: Optional[str]
+    repo_url: str
+    target_commit_id: Optional[str]
     dataset_stage: List[DatasetStageItem]
+    git_repo: GitRepo
+    dvc_repo: dvc.repo.Repo
+    lock: ReentrantLock
 
     def __init__(
-        self, repo_url: str = None, dvc_remote: str = None, cache_local_repository=False,
-        cache_root=None
+        self, repo_url: str, dvc_remote: str | None = None, cache_prefix: str | None = None,
+        cache_local_repository: bool = False, cache_root: str | None = None
     ):
         """
         Initialize repository.
 
         Clones git repository if it's not in the cache.
         """
         if dvc_remote is None:
             dvc_remote = os.environ.get('DVC_PANDAS_DVC_REMOTE')
 
         self.repo_url = repo_url
         self.dvc_remote = dvc_remote
         self.cache_local_repository = cache_local_repository
         self.git_repo = get_cache_repo(
-            repo_url, cache_local_repository=cache_local_repository, cache_root=cache_root
+            repo_url, prefix=cache_prefix, cache_local_repository=cache_local_repository, cache_root=cache_root
         )
         self.repo_dir = Path(self.git_repo.working_dir)
-        self.dvc_repo = dvc.repo.Repo(self.repo_dir)
+        self.dvc_repo = dvc.repo.Repo(str(self.repo_dir))
         self.dataset_stage = []
+        self.target_commit_id = None
+        self.lock = ReentrantLock(str(self.repo_dir / '.dvc-pandas.lock'))
 
-    def load_dataset(self, identifier: str, skip_pull_if_exists=False, commit=None) -> Dataset:
+    def log_info(self, message: str):
+        logger.info('[%s] %s' % (self.repo_url, message))
+
+    @ensure_repo_lock
+    def load_dataset(self, identifier: str, skip_pull_if_exists=False) -> Dataset:
         """
         Load dataset with the given identifier from the given repository.
 
         If `skip_pull_if_exists` is True, does not update the dataset if a parquet file exists for the identifier,
         regardless of the content.
-
-        The `commit` argument can be set to a git commit ID to get the dataset from a specific commit instead of the
-        latest one.
         """
-        with TemporaryGitCheckout(self.git_repo, commit):
+        def should_pull(parquet_path: Path, metadata: dict):
+            if not skip_pull_if_exists:
+                return True
+            if not parquet_path.exists():
+                return True
+            m = metadata['outs'][0]
+            if parquet_path.stat().st_size != m['size']:
+                self.log_info(f"Size mismatch with {parquet_path}")
+                return True
+            with open(parquet_path, 'rb') as f:
+                h = md5(f.read()).hexdigest()
+                if h != m['md5']:
+                    self.log_info(f"MD5 hash mismatch with {parquet_path}")
+                    return True
+            return False
+
+        with TemporaryGitCheckout(self.git_repo, self.target_commit_id):
             parquet_path = self.repo_dir / (identifier + '.parquet')
-            if not (parquet_path.exists() and skip_pull_if_exists):
-                logger.debug(f"Pull dataset {parquet_path} from DVC")
-                self.dvc_repo.pull(str(parquet_path))
-            df = pd.read_parquet(parquet_path)
 
             # Get metadata (including units) from .dvc file
             dvc_file_path = parquet_path.parent / (parquet_path.name + '.dvc')
             yaml = YAML()
             with open(dvc_file_path, 'rt') as file:
-                metadata = yaml.load(file).get('meta')
+                dvc_data = yaml.load(file)
+
+            if should_pull(parquet_path, dvc_data):
+                self.log_info(f"Pull dataset {parquet_path} from DVC using remote {self.dvc_remote}")
+                self.dvc_repo.pull(str(parquet_path), remote=self.dvc_remote)
 
+            df = pd.read_parquet(parquet_path)
+
+            metadata = dvc_data.get('meta')
             if metadata is None:
                 units = None
             else:
                 units = metadata.pop('units', None)
 
             mtime = dvc_file_path.stat().st_mtime
             modified_at = datetime.fromtimestamp(mtime, tz=timezone.utc)
 
             return Dataset(df, identifier, modified_at=modified_at, units=units, metadata=metadata)
 
-    def load_dataframe(self, identifier: str, skip_pull_if_exists=False, commit=None) -> pd.DataFrame:
+    def load_dataframe(self, identifier: str, skip_pull_if_exists=False) -> pd.DataFrame:
         """
         Same as load_dataset, but only provides the DataFrame for convenience.
         """
-        dataset = self.load_dataset(identifier, skip_pull_if_exists, commit)
+        dataset = self.load_dataset(identifier, skip_pull_if_exists)
         return dataset.df
 
+    @ensure_repo_lock
     def has_dataset(self, identifier: str) -> bool:
         """
         Check if a dataset with the given identifier exists.
         """
-        dvc_file_path = self.repo_dir / (identifier + '.parquet.dvc')
-        return os.path.exists(dvc_file_path)
+        with TemporaryGitCheckout(self.git_repo, self.target_commit_id):
+            dvc_file_path = self.repo_dir / (identifier + '.parquet.dvc')
+            return os.path.exists(dvc_file_path)
 
+    @ensure_repo_lock
     def pull_datasets(self):
         """
         Make sure the git repository is pulled to the latest version.
         """
-        logger.debug("Pull from git remote")
-        self.git_repo.remote().pull()
+        self.log_info("Pull from git remote")
+        origin = self.git_repo.remote()
+        origin.fetch()
+        for remote_ref in origin.refs:
+            if remote_ref.remote_head in ('master', 'main'):
+                break
+        else:
+            raise KeyError("No 'master' or 'main' branch found for origin")
+        ref: git.Head = getattr(self.git_repo.heads, remote_ref.remote_head)
+        ref.set_commit(remote_ref.commit)
+        ref.checkout()
 
+    @ensure_repo_lock
     def push_dataset(self, dataset: Dataset):
         """
         Add the given dataset as a parquet file to DVC, create a commit and push it.
 
         Updates the git repository first. If something goes wrong, restores the repository and all files to the state
         of origin/master.
 
         This is a convenience method wrapping add() and push(). If the dataset stage (the one populated by add()) is not
         empty, this raises a ValueError.
         """
         if self.dataset_stage:
             raise ValueError("push_dataset was called with nonempty stage.")
+        if self.read_only:
+            raise ValueError("push_dataset was called while repository is read-only.")
 
         self.pull_datasets()
         parquet_path = self.repo_dir / (dataset.identifier + '.parquet')
         self.add(dataset)
         try:
             self.push()
         except Exception:
@@ -146,31 +236,39 @@
             self.git_repo.head.reset('origin/master', index=True, working_tree=True)
 
             logger.debug(f"Checkout {parquet_path} from DVC")
             self.dvc_repo.checkout(str(parquet_path), force=True)
 
             # Remove rolled back stuff that may be left on the remote
             # self.dvc_repo.gc(all_commits=True, cloud=True, remote=self.dvc_remote)
-            # TODO: Before reinstating the previous line, make sure gc doesn't delete blobs for which we don't have a
-            # git commit because our git repository is outdated.
+            # TODO: Before reinstating the previous line, make sure gc doesn't delete blobs for which we don't have
+            # a git commit because our git repository is outdated.
             raise
         finally:
             # Remove old version (or new if we rolled back) from cache
             logger.debug("Collect garbage in local DVC repository")
             self.dvc_repo.gc(workspace=True)
 
+    @ensure_repo_lock
     def add(self, dataset: Dataset):
         """Create or update parquet file from dataset, but do not create .dvc file, commit or push."""
+        if self.read_only:
+            raise ValueError("add was called while repository is read-only.")
+
         parquet_path = self.repo_dir / (dataset.identifier + '.parquet')
         os.makedirs(parquet_path.parent, exist_ok=True)
-        dataset.df.to_parquet(str(parquet_path))
+        dataset.to_parquet(str(parquet_path))
         self.dataset_stage.append(DatasetStageItem(dataset))
 
+    @ensure_repo_lock
     def push(self):
         """Upload, commit and push the staged files and clear the stage."""
+        if self.read_only:
+            raise ValueError("add was called while repository is read-only.")
+
         for stage_item in self.dataset_stage:
             path = self.repo_dir / (stage_item.identifier + '.parquet')
 
             # Remove old .dvc file (if it exists) and replace it with a new one
             dvc_file_path = path.parent / (path.name + '.dvc')
             if dvc_file_path.exists():
                 logger.debug(f"Remove file {dvc_file_path} from DVC")
@@ -198,30 +296,48 @@
             logger.debug("Push to git repository")
             git_push(self.git_repo)
         else:
             logger.debug("No commit needed")
 
         self.dataset_stage = []
 
+    @property
+    def read_only(self):
+        return self.target_commit_id is not None
+
+    @ensure_repo_lock
     def _need_commit(self) -> bool:
         if not self.git_repo.is_dirty():
             return False
-        # We don't commit if the only files changed are .gitignore files. DVC sometimes reorders the lines in .gitignore
-        # even though no file has changed.
+        # We don't commit if the only files changed are .gitignore files. DVC sometimes reorders the lines in
+        # .gitignore even though no file has changed.
         diffs = self.git_repo.index.diff(self.git_repo.head.commit)
         return any(os.path.basename(diff.a_path) != '.gitignore' for diff in diffs)
 
+    @property
+    def commit_id(self):
+        """Git commit ID that this object will operate on"""
+        return self.target_commit_id or self.git_repo.head.commit.hexsha
+
+    def set_target_commit(self, commit_id: str | None):
+        """
+        Set commit ID that this object will operate on.
+
+        If `commit_id` is not None, the given commit ID will be checked out temporarily for most commands and the
+        repository will be read-only. Set it to None to use the latest commit.
+        """
+        self.target_commit_id = commit_id
+
 
 # FIXME: Make common base class instead of extending Repository
 class StaticRepository(Repository):
     def __init__(self, config):
         self.datasets = {dataset['identifier']: dataset for dataset in config}
 
     def load_dataset(self, identifier, skip_pull_if_exists=False):
-        import pandas as pd
         spec = self.datasets[identifier]
         # TODO: Index?
         df = pd.DataFrame(columns=spec['columns'], data=spec['data'])
         # TODO: units and metadata
         return Dataset(df, identifier, units=None, metadata=None)
 
     def has_dataset(self, identifier):
```

### Comparing `dvc-pandas-0.0.9/src/dvc_pandas.egg-info/PKG-INFO` & `dvc-pandas-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: dvc-pandas
-Version: 0.0.9
+Version: 0.1.0
 Summary: Wrapper for DVC and git to easily fetch Pandas dataframes
 Home-page: https://github.com/kausaltech/dvc-pandas
 Author: Bernhard Bliem
 Author-email: bernhard.bliem@kausal.tech
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kausaltech/dvc-pandas/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dvc-pandas
-
-
```

### Comparing `dvc-pandas-0.0.9/LICENSE` & `dvc-pandas-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-pandas-0.0.9/setup.cfg` & `dvc-pandas-0.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dvc-pandas
-version = 0.0.9
+version = 0.1.0
 author = Bernhard Bliem
 author_email = bernhard.bliem@kausal.tech
 description = Wrapper for DVC and git to easily fetch Pandas dataframes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kausaltech/dvc-pandas
 project_urls = 
@@ -14,19 +14,21 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.7
 install_requires = 
 	GitPython
 	appdirs
-	dvc[s3]
+	dvc
+	dvc-s3
+	fasteners
 	pyarrow
 	pandas
 	pint-pandas
 	python-snappy
 	ruamel.yaml
 
 [options.packages.find]
```

### Comparing `dvc-pandas-0.0.9/PKG-INFO` & `dvc-pandas-0.1.0/src/dvc_pandas.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: dvc-pandas
-Version: 0.0.9
+Version: 0.1.0
 Summary: Wrapper for DVC and git to easily fetch Pandas dataframes
 Home-page: https://github.com/kausaltech/dvc-pandas
 Author: Bernhard Bliem
 Author-email: bernhard.bliem@kausal.tech
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kausaltech/dvc-pandas/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dvc-pandas
-
-
```

