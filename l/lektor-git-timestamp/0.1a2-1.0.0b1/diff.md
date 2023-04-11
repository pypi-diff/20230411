# Comparing `tmp/lektor-git-timestamp-0.1a2.tar.gz` & `tmp/lektor-git-timestamp-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpl_46a20z/tmpwihwq4t1/lektor-git-timestamp-0.1a2.tar", last modified: Thu Feb  4 02:34:07 2021, max compression
+gzip compressed data, was "lektor-git-timestamp-1.0.0b1.tar", last modified: Tue Apr 11 19:52:55 2023, max compression
```

## Comparing `lektor-git-timestamp-0.1a2.tar` & `lektor-git-timestamp-1.0.0b1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-04 02:34:07.968086 lektor-git-timestamp-0.1a2/
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-04 02:34:07.968086 lektor-git-timestamp-0.1a2/.github/
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-04 02:34:07.968086 lektor-git-timestamp-0.1a2/.github/workflows/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      757 2021-02-04 02:25:30.000000 lektor-git-timestamp-0.1a2/.github/workflows/tests.yml
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)       85 2020-06-16 22:21:17.000000 lektor-git-timestamp-0.1a2/.gitignore
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      235 2021-02-04 02:25:30.000000 lektor-git-timestamp-0.1a2/CHANGES.md
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)     1062 2020-06-16 22:08:44.000000 lektor-git-timestamp-0.1a2/LICENSE
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)       72 2020-06-16 22:10:11.000000 lektor-git-timestamp-0.1a2/MANIFEST.in
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     7228 2021-02-04 02:34:07.968086 lektor-git-timestamp-0.1a2/PKG-INFO
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)     4838 2020-06-16 22:17:51.000000 lektor-git-timestamp-0.1a2/README.md
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-04 02:34:07.968086 lektor-git-timestamp-0.1a2/lektor_git_timestamp.egg-info/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     7228 2021-02-04 02:34:07.000000 lektor-git-timestamp-0.1a2/lektor_git_timestamp.egg-info/PKG-INFO
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      450 2021-02-04 02:34:07.000000 lektor-git-timestamp-0.1a2/lektor_git_timestamp.egg-info/SOURCES.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)        1 2021-02-04 02:34:07.000000 lektor-git-timestamp-0.1a2/lektor_git_timestamp.egg-info/dependency_links.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       74 2021-02-04 02:34:07.000000 lektor-git-timestamp-0.1a2/lektor_git_timestamp.egg-info/entry_points.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       10 2021-02-04 02:34:07.000000 lektor-git-timestamp-0.1a2/lektor_git_timestamp.egg-info/requires.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       21 2021-02-04 02:34:07.000000 lektor-git-timestamp-0.1a2/lektor_git_timestamp.egg-info/top_level.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     4942 2021-02-04 02:25:30.000000 lektor-git-timestamp-0.1a2/lektor_git_timestamp.py
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)      146 2020-06-16 22:08:57.000000 lektor-git-timestamp-0.1a2/pyproject.toml
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)     1218 2021-02-04 02:34:07.968086 lektor-git-timestamp-0.1a2/setup.cfg
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)       57 2020-06-16 22:14:33.000000 lektor-git-timestamp-0.1a2/setup.py
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2021-02-04 02:34:07.968086 lektor-git-timestamp-0.1a2/tests/
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)      734 2020-06-16 22:06:49.000000 lektor-git-timestamp-0.1a2/tests/conftest.py
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)    10271 2021-02-04 01:50:18.000000 lektor-git-timestamp-0.1a2/tests/test_plugin.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1034 2021-02-04 02:25:30.000000 lektor-git-timestamp-0.1a2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-11 19:52:55.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-11 19:52:55.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:52:55.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 19:52:55.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 19:52:55.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 19:52:55.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/tests/test-site/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tests/test-site/Test Site.lektorproject
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/tests/test-site/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tests/test-site/content/contents.lr
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/tests/test-site/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tests/test-site/models/page.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tox.ini
```

### Comparing `lektor-git-timestamp-0.1a2/LICENSE` & `lektor-git-timestamp-1.0.0b1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright © 2020 Geoffrey T. Dairiki
+Copyright © 2020, 2021, 2023 Geoffrey T. Dairiki
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `lektor-git-timestamp-0.1a2/README.md` & `lektor-git-timestamp-1.0.0b1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -115,10 +115,28 @@
 
 - any commits whose commit message include the tag `[nochange]` will be ignored
 - the first commit (the one whose timestamp is used for `pub_date`) is ignored
 
 If there has only been one commit of the source file, `last_mod` will not have
 a default value.  (It will evaluate to a jinja2 Undefined instance.)
 
+## Warning: On sorting by `gittimestamp` in `Lektor < 3.3`
+
+A common use case for timestamps is for sorting records.
+E.g. in a blog one generally wants to display posts in reverse
+chronological order by post date.  This generally won't work using
+`gittimestamp` timestamps with version of Lektor before 3.3.
+
+The `gittimestamp` type is implemented using a _field
+descriptor_. (This is required in order to defer computation of the
+field value until after the record for the page is available.) In
+`lektor<3.3`, field descriptors are supported for most usages, the
+_one glaring exception_ being when sorting records.
+
+This was fixed in Lektor PR
+[#789](https://github.com/lektor/lektor/pull/789) which was merged to
+the master branch on February 6, 2021, but didn't make it into a release
+until Lektor 3.3, released on December 13 2021.
+
 ## Author
 
 Jeff Dairiki <dairiki@dairiki.org>
```

### Comparing `lektor-git-timestamp-0.1a2/lektor_git_timestamp.py` & `lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from collections import namedtuple
 import datetime
 import hashlib
 from operator import attrgetter
 import os
 import pickle
 import re
@@ -19,24 +18,24 @@
 
 from lektorlib.recordcache import get_or_create_virtual
 
 VIRTUAL_PATH_PREFIX = 'git-timestamp'
 
 
 def run_git(*args):
-    cmd = ['git'] + list(args)
-    output = subprocess.check_output(cmd, universal_newlines=True)
-    return output.rstrip()
+    cmd = ('git', *args)
+    proc = subprocess.run(cmd, capture_output=True, text=True, check=True)
+    return proc.stdout.rstrip()
 
 
 def _fs_mtime(filename):
     try:
         st = os.stat(filename)
     except OSError as exc:
-        reporter.report_generic("{}: {!s}".format(filename, exc))
+        reporter.report_generic(f"{filename}: {exc!s}")
         return None
     else:
         # (truncate to one second resolution)
         return int(st.st_mtime)
 
 
 def _is_dirty(filename):
@@ -98,25 +97,25 @@
     def get(cls, record):
         def creator():
             return cls(record)
         return get_or_create_virtual(record, VIRTUAL_PATH_PREFIX, creator)
 
     @property
     def path(self):
-        return "{}@{}".format(self.record.path, VIRTUAL_PATH_PREFIX)
+        return f"{self.record.path}@{VIRTUAL_PATH_PREFIX}"
 
     def get_checksum(self, path_cache):
         return _compute_checksum(self.timestamps)
 
     @cached_property
     def timestamps(self):
         return tuple(_iter_timestamps(self.source_filename))
 
 
-class GitTimestampDescriptor(object):
+class GitTimestampDescriptor:
     def __init__(self, raw,
                  ignore_commits=None,
                  strategy='last',
                  skip_first_commit=False):
         self.raw = raw
         self.kwargs = {
             'ignore_commits': ignore_commits,
@@ -135,30 +134,30 @@
         if mtime is None:
             return self.raw.missing_value("no suitable git timestamp exists")
         return datetime.datetime.fromtimestamp(mtime)
 
 
 class GitTimestampType(DateTimeType):
     def value_from_raw(self, raw):
-        value = super(GitTimestampType, self).value_from_raw(raw)
+        value = super().value_from_raw(raw)
         if jinja2.is_undefined(value):
             options = self.options
             value = GitTimestampDescriptor(
                 raw,
                 ignore_commits=options.get('ignore_commits'),
                 strategy=options.get('strategy', 'last'),
                 skip_first_commit=bool_from_string(
                     options.get('skip_first_commit', False)),
                 )
         return value
 
 
 class GitTimestampPlugin(Plugin):
     name = 'git-timestamp'
-    description = u'Lektor type to deduce page modification time from git'
+    description = 'Lektor type to deduce page modification time from git'
 
     def on_setup_env(self, **extra):
         env = self.env
         env.add_type(GitTimestampType)
         env.virtualpathresolver(VIRTUAL_PATH_PREFIX)(self.resolve_virtual_path)
 
     @staticmethod
```

### Comparing `lektor-git-timestamp-0.1a2/tests/test_plugin.py` & `lektor-git-timestamp-1.0.0b1/tests/test_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# -*- coding: utf-8 -*-
 import datetime
 import os
 import re
-import subprocess
 import sys
 
 import pytest
 
 import jinja2
 from lektor.environment import PRIMARY_ALT
 from lektor.reporter import BufferReporter
@@ -23,103 +21,49 @@
     GitTimestampSource,
     GitTimestampDescriptor,
     GitTimestampType,
     GitTimestampPlugin,
     )
 
 
-try:
-    utc = datetime.timezone.utc
-except AttributeError:          # py2
-    class UTC(datetime.tzinfo):
-        def utcoffset(self, dt):
-            return datetime.timedelta(0)
-
-        def tzname(self, dt):
-            return "UTC"
-
-        def dst(self, dt):
-            return datetime.timedelta(0)
-    utc = UTC()
-
-
 def test_run_git():
     output = run_git('--version')
     assert output.startswith('git version')
 
 
-class DummyGitRepo(object):
-    def __init__(self, work_tree):
-        self.work_tree = work_tree
-        self.run_git('init')
-        self.run_git('commit', '--message=initial', '--allow-empty')
-
-    def run_git(self, *args, **kwargs):
-        cmd = ['git'] + list(args)
-        subprocess.check_call(cmd, cwd=str(self.work_tree), **kwargs)
-
-    def touch(self, filename, ts=None):
-        file_path = self.work_tree / filename
-        file_path.touch()
-        if ts is not None:
-            os.utime(str(file_path), (ts, ts))
-
-    def modify(self, filename):
-        file_path = self.work_tree / filename
-        with file_path.open('at') as f:
-            f.write(u'changed\n')
-
-    def commit(self, filename, ts=None, message='test'):
-        if ts is None:
-            env = os.environ
-        else:
-            dt = datetime.datetime.fromtimestamp(ts, utc)
-            env = os.environ.copy()
-            env['GIT_AUTHOR_DATE'] = dt.isoformat('T')
-        self.modify(filename)
-        self.run_git('add', str(filename))
-        self.run_git('commit', '--message', str(message), env=env)
-
-
-@pytest.fixture
-def git_repo(tmp_path):
-    os.chdir(str(tmp_path))
-    return DummyGitRepo(tmp_path)
-
-
-class Test__fs_mtime(object):
+class Test__fs_mtime:
     def test(self, git_repo):
         ts = 1589238180
         git_repo.touch('test.txt', ts)
         assert _fs_mtime('test.txt') == ts
 
     def test_missing_file(self, git_repo, env):
         with BufferReporter(env) as reporter:
             assert _fs_mtime('test.txt') is None
         event, data = reporter.buffer[0]
         assert event == 'generic'
         assert re.match(r'(?i)test.txt: .*\bno such file', data['message'])
 
 
-class Test__is_dirty(object):
+class Test__is_dirty:
     def test_dirty_if_not_in_git(self, git_repo):
         git_repo.touch('test.txt')
         assert _is_dirty('test.txt')
 
     def test_clean(self, git_repo):
         git_repo.commit('test.txt')
         assert not _is_dirty('test.txt')
 
     def test_dirty(self, git_repo):
         git_repo.commit('test.txt')
         git_repo.modify('test.txt')
         assert _is_dirty('test.txt')
 
 
-class Test__iter_timestamps(object):
+class Test__iter_timestamps:
     def test_from_git(self, git_repo):
         ts = 1589238186
         git_repo.commit('test.txt', ts, 'message')
         assert list(_iter_timestamps('test.txt')) == [(ts, 'message')]
 
     def test_from_mtime(self, git_repo):
         ts = 1589238186
@@ -134,15 +78,15 @@
         git_repo.touch('test.txt', ts2)
         assert list(_iter_timestamps('test.txt')) == [
             (ts2, None),
             (ts1, 'commit'),
             ]
 
 
-class Test_get_mtime(object):
+class Test_get_mtime:
     def test_not_in_git(self):
         ts = 1589238006
         timestamps = (timestamp(ts, None),)
         assert get_mtime(timestamps) == ts
 
     def test_clean(self, git_repo):
         ts = 1589238186
@@ -209,27 +153,27 @@
         assert get_mtime(timestamps, strategy='latest') == ts2
 
     def test_missing_file(self, git_repo):
         timestamps = ()
         assert get_mtime(timestamps) is None
 
 
-class DummyPage(object):
+class DummyPage:
     alt = PRIMARY_ALT
 
     def __init__(self, source_filename, path='/', pad=None):
         self.source_filename = source_filename
         self.path = path
         self.pad = pad
 
     def iter_source_filenames(self):
         yield self.source_filename
 
 
-class TestGitTimestampSource(object):
+class TestGitTimestampSource:
     @pytest.fixture
     def ts_now(self):
         return 1592256980
 
     @pytest.fixture
     def record(self, git_repo, ts_now, pad):
         git_repo.touch('test.txt', ts_now)
@@ -251,27 +195,27 @@
         assert src.timestamps == (timestamp(ts_now, None),)
 
 
 @pytest.mark.parametrize(('data', 'checksum'), [
     ((),
      "5d460934f4a194c28ce73ada3b56d2e025d5c47c"),
     pytest.param(
-        (timestamp(1592256980, u"message"),),
+        (timestamp(1592256980, "message"),),
         "db24b207c382159c97a2a6cd177c05c0f218277a",
         marks=pytest.mark.xfail(
             sys.version_info >= (3,) and sys.version_info < (3, 7),
-            reason="pickle pickles integers differently in py35 and py36")
+            reason="pickle pickles integers differently in py36")
         ),
     ])
 def test__compute_checksum(data, checksum):
     # These checksums should be portable across platforms
     assert _compute_checksum(data) == checksum
 
 
-class TestGitTimestampDescriptor(object):
+class TestGitTimestampDescriptor:
     @pytest.fixture
     def desc(self):
         raw = RawValue('test', None)
         return GitTimestampDescriptor(raw)
 
     @pytest.fixture
     def record(self, git_repo, pad):
@@ -279,37 +223,39 @@
         return DummyPage(source_filename, pad=pad)
 
     def test_class_descriptor(self, desc):
         assert desc.__get__(None, object) is desc
 
     def test_get(self, desc, git_repo, record):
         dt = datetime.datetime.now().replace(microsecond=0)
-        ts = int(dt.strftime('%s'))
-        git_repo.commit('test.txt', ts)
+        git_repo.commit('test.txt', dt)
         assert desc.__get__(record) == dt
 
     def test_get_returns_undefined(self, desc, record):
         assert jinja2.is_undefined(desc.__get__(record))
 
     def test_get_declares_dependency(self, desc, record, ctx):
         desc.__get__(record)
-        assert '/@git-timestamp' in ctx.referenced_virtual_dependencies
+        virtual_dependencies = ctx.referenced_virtual_dependencies
+        if hasattr(virtual_dependencies, "values"):  # Lektor < 3.4.0b5
+            virtual_dependencies = set(virtual_dependencies.values())
+        assert '/@git-timestamp' in {v.path for v in virtual_dependencies}
 
     def test_init_kwargs(self):
         raw = RawValue('test', None)
         kwargs = {
             'ignore_commits': 'nochange',
             'strategy': 'first',
             'skip_first_commit': True,
             }
         desc = GitTimestampDescriptor(raw, **kwargs)
         assert desc.kwargs == kwargs
 
 
-class TestGitTimestampType(object):
+class TestGitTimestampType:
     @pytest.fixture
     def type_(self, env):
         options = {}
         return GitTimestampType(env, options)
 
     def test_value_from_raw_explicit(self, type_):
         raw = RawValue('test', '2020-01-02 03:04')
@@ -317,15 +263,15 @@
 
     def test_value_from_raw(self, type_):
         raw = RawValue('test', None)
         value = type_.value_from_raw(raw)
         assert isinstance(value, GitTimestampDescriptor)
 
 
-class TestGitTimestampPlugin(object):
+class TestGitTimestampPlugin:
     @pytest.fixture
     def plugin(self, env):
         return GitTimestampPlugin(env, 'git-timestamp')
 
     @pytest.fixture
     def record(self, git_repo, pad):
         source_filename = os.path.abspath('test.txt')
```

### Comparing `lektor-git-timestamp-0.1a2/tox.ini` & `lektor-git-timestamp-1.0.0b1/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 [tox]
 minversion = 3
-envlist = py27,py35,py36,py37,py38,py39,lint
+envlist = {py37,py38,py39,py310,py311}{,-lektor33},lint
 
 [gh-actions]
 python =
-    2.7: py27
-    3.5: py35
-    3.6: py36
     3.7: py37
     3.8: py38
-    3.9: py39, lint
+    3.9: py39
+    3.10: py310
+    3.11: py311, lint
 
 [testenv]
 deps =
     pytest
     pytest-cov
-    lektor
+    !lektor33: lektor>=3.4.0a0
+    lektor33: lektor<3.4.0
 setenv =
     # Prevent parallel pytest-cov runs from clobbering each others .coverage file
     COVERAGE_FILE = {envtmpdir}/.coverage
 passenv =
     # Needed by git (to find global config settings user.email, user.name)
     HOME
 commands =
     py.test --cov lektor_git_timestamp {posargs:--cov-fail-under=100 tests}
 
+# Download latest pip.
+# This works around issues with concurrent access to pip cache
+# when running tox in parallel mode.
+download = true
+
 [testenv:lint]
 skip_install = True
-basepython = python3.9
 deps =
-    pep517 >= 0.9
+    build
     flake8
     twine
-    check-manifest
 commands =
-    python -m pep517.build --source --out-dir {envtmpdir}/dist {toxinidir}
+    python -m build --sdist --outdir {envtmpdir}/dist {toxinidir}
     twine check {envtmpdir}/dist/*
     flake8
-    check-manifest
-
-[pytest]
-addopts =
-    --cov-report=term-missing --cov-report=html
 
 [flake8]
 exclude =
     .tox,
     .git,
     __pycache__,
     .eggs,
```

