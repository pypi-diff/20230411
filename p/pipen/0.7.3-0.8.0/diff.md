# Comparing `tmp/pipen-0.7.3.tar.gz` & `tmp/pipen-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen-0.7.3.tar", max compression
+gzip compressed data, was "pipen-0.8.0.tar", max compression
```

## Comparing `pipen-0.7.3.tar` & `pipen-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-04-10 01:40:38.233460 pipen-0.7.3/LICENSE
--rw-r--r--   0        0        0     9390 2023-04-10 01:40:38.233460 pipen-0.7.3/README.md
--rw-r--r--   0        0        0      318 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/__init__.py
--rw-r--r--   0        0        0       68 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/__main__.py
--rw-r--r--   0        0        0     7143 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/_job_caching.py
--rw-r--r--   0        0        0     6434 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/channel.py
--rw-r--r--   0        0        0       83 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/cli/__init__.py
--rw-r--r--   0        0        0      912 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/cli/_hooks.py
--rw-r--r--   0        0        0     1651 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/cli/_main.py
--rw-r--r--   0        0        0      973 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/cli/help.py
--rw-r--r--   0        0        0     3701 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/cli/plugins.py
--rw-r--r--   0        0        0     2906 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/cli/profile.py
--rw-r--r--   0        0        0     1452 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/cli/version.py
--rw-r--r--   0        0        0     2623 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/defaults.py
--rw-r--r--   0        0        0     1840 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/exceptions.py
--rw-r--r--   0        0        0     9478 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/job.py
--rw-r--r--   0        0        0    16199 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/pipen.py
--rw-r--r--   0        0        0     9562 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/pluginmgr.py
--rw-r--r--   0        0        0    24161 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/proc.py
--rw-r--r--   0        0        0     5507 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/procgroup.py
--rw-r--r--   0        0        0     4067 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/progressbar.py
--rw-r--r--   0        0        0     1857 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/scheduler.py
--rw-r--r--   0        0        0     3668 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/template.py
--rw-r--r--   0        0        0    14404 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/utils.py
--rw-r--r--   0        0        0       54 2023-04-10 01:40:38.237460 pipen-0.7.3/pipen/version.py
--rw-r--r--   0        0        0     1767 2023-04-10 01:40:38.237460 pipen-0.7.3/pyproject.toml
--rw-r--r--   0        0        0    10706 1970-01-01 00:00:00.000000 pipen-0.7.3/setup.py
--rw-r--r--   0        0        0    10502 1970-01-01 00:00:00.000000 pipen-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 17:04:51.925708 pipen-0.8.0/LICENSE
+-rw-r--r--   0        0        0     9390 2023-04-11 17:04:51.925708 pipen-0.8.0/README.md
+-rw-r--r--   0        0        0      318 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/__init__.py
+-rw-r--r--   0        0        0       68 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/__main__.py
+-rw-r--r--   0        0        0     7143 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/_job_caching.py
+-rw-r--r--   0        0        0     6434 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/channel.py
+-rw-r--r--   0        0        0       83 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/__init__.py
+-rw-r--r--   0        0        0      912 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/_hooks.py
+-rw-r--r--   0        0        0     1651 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/_main.py
+-rw-r--r--   0        0        0      973 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/help.py
+-rw-r--r--   0        0        0     3701 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/plugins.py
+-rw-r--r--   0        0        0     2906 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/profile.py
+-rw-r--r--   0        0        0     1422 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/cli/version.py
+-rw-r--r--   0        0        0     2623 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/defaults.py
+-rw-r--r--   0        0        0     1832 2023-04-11 17:04:51.929708 pipen-0.8.0/pipen/exceptions.py
+-rw-r--r--   0        0        0     9478 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/job.py
+-rw-r--r--   0        0        0    16597 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/pipen.py
+-rw-r--r--   0        0        0     9965 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/pluginmgr.py
+-rw-r--r--   0        0        0    23511 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/proc.py
+-rw-r--r--   0        0        0     5507 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/procgroup.py
+-rw-r--r--   0        0        0     4067 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/progressbar.py
+-rw-r--r--   0        0        0     1857 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/scheduler.py
+-rw-r--r--   0        0        0     3668 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/template.py
+-rw-r--r--   0        0        0    14662 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/utils.py
+-rw-r--r--   0        0        0       54 2023-04-11 17:04:51.933708 pipen-0.8.0/pipen/version.py
+-rw-r--r--   0        0        0     1665 2023-04-11 17:04:51.933708 pipen-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    10516 1970-01-01 00:00:00.000000 pipen-0.8.0/setup.py
+-rw-r--r--   0        0        0    10350 1970-01-01 00:00:00.000000 pipen-0.8.0/PKG-INFO
```

### Comparing `pipen-0.7.3/LICENSE` & `pipen-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/README.md` & `pipen-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/_job_caching.py` & `pipen-0.8.0/pipen/_job_caching.py`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/channel.py` & `pipen-0.8.0/pipen/channel.py`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/cli/_hooks.py` & `pipen-0.8.0/pipen/cli/_hooks.py`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/cli/_main.py` & `pipen-0.8.0/pipen/cli/_main.py`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/cli/help.py` & `pipen-0.8.0/pipen/cli/help.py`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/cli/plugins.py` & `pipen-0.8.0/pipen/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/cli/profile.py` & `pipen-0.8.0/pipen/cli/profile.py`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/cli/version.py` & `pipen-0.8.0/pipen/cli/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         from .. import __version__
 
         versions = {"python": sys.version, "pipen": __version__}
 
         for pkg in (
             "liquidpy",
             "pandas",
-            "python-slugify",
             "enlighten",
             "argx",
             "xqute",
             "python-simpleconf",
             "pipda",
             "varname",
         ):
```

### Comparing `pipen-0.7.3/pipen/defaults.py` & `pipen-0.8.0/pipen/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/exceptions.py` & `pipen-0.8.0/pipen/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,9 +58,9 @@
     """Failed to render a template"""
 
 
 class ConfigurationError(PipenException):
     """When something wrong set as configuration"""
 
 
-class ProcWorkdirConflictException(PipenException):
+class PipenOrProcNameError(PipenException):
     """ "When more than one processes are sharing the same workdir"""
```

### Comparing `pipen-0.7.3/pipen/job.py` & `pipen-0.8.0/pipen/job.py`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/pipen.py` & `pipen-0.8.0/pipen/pipen.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,27 +12,31 @@
 from diot import Diot
 from rich import box
 from rich.panel import Panel
 from rich.table import Table
 from rich.text import Text
 from rich.console import Group
 from simpleconf import ProfileConfig
-from slugify import slugify  # type: ignore
 from varname import varname, VarnameException
 
 from .defaults import CONFIG, CONFIG_FILES
-from .exceptions import ProcDependencyError, PipenSetDataError
+from .exceptions import (
+    PipenOrProcNameError,
+    ProcDependencyError,
+    PipenSetDataError,
+)
 from .pluginmgr import plugin
 from .proc import Proc
 from .progressbar import PipelinePBar
 from .utils import (
     copy_dict,
     desc_from_docstring,
     get_logpanel_width,
     get_plugin_context,
+    is_valid_name,
     log_rich_renderable,
     logger,
     pipen_banner,
 )
 
 
 class Pipen:
@@ -88,23 +92,29 @@
             self.name = self.__class__.__name__
         else:
             try:
                 self.name = varname()
             except VarnameException:
                 self.name = f"pipen-{self.__class__.PIPELINE_COUNT}"
 
+        if not is_valid_name(self.name):
+            raise PipenOrProcNameError(
+                f"Invalid pipeline name: {self.name}, "
+                r"expecting '^[\w.-]$'"
+            )
+
         self.desc = (
             desc
             or self.__class__.desc
             or desc_from_docstring(self.__class__)
         )
         self.outdir = Path(
             outdir
             or self.__class__.outdir
-            or f"./{slugify(self.name)}_results"
+            or f"./{self.name}_results"
         ).resolve()
         self.workdir: Path = None
         self.profile: str = "default"
 
         self.starts: List[Proc] = self.__class__.starts
         if self.starts and not isinstance(self.starts, (tuple, list)):
             self.starts = [self.starts]
@@ -160,15 +170,15 @@
         Args:
             profile: The default profile to use for the run
 
         Returns:
             True if the pipeline ends successfully else False
         """
         self.profile = profile
-        self.workdir = Path(self.config.workdir) / slugify(self.name)
+        self.workdir = Path(self.config.workdir) / self.name
         self.workdir.mkdir(parents=True, exist_ok=True)
 
         succeeded = True
         await self._init()
         logger.setLevel(self.config.loglevel.upper())
         log_rich_renderable(pipen_banner(), "magenta", logger.info)
         try:
@@ -453,14 +463,19 @@
                 nexts, key=lambda prc: (prc.order or 0, prc.name)
             ):
                 if proc in self.procs:
                     raise ProcDependencyError(
                         f"Cyclic dependency: {proc.name}"
                     )
 
+                if proc.name in [p.name for p in self.procs]:
+                    raise PipenOrProcNameError(
+                        f"'{proc.name}' is already used by another process."
+                    )
+
                 # Add proc to self.procs if all their requires
                 # are added to self.procs
                 # Then remove proc from nexts
                 # If there are still procs in nexts
                 # meaning some requires of those procs cannot run before
                 # those procs.
                 if not set(proc.requires) - set(self.procs):  # type: ignore
```

### Comparing `pipen-0.7.3/pipen/pluginmgr.py` & `pipen-0.8.0/pipen/pluginmgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,17 @@
 
 
 class PipenMainPlugin:
     """The builtin main plugin, used to update the progress bar and
     cache the job"""
 
     name = "main"
+    # The priority is set to -1000 to make sure it is the first plugin
+    # to be called
+    order = -1000
 
     @plugin.impl
     def on_proc_shutdown(self, proc: Proc, sig: signal.Signals):
         """When a process is shutting down"""
         if sig:  # pragma: no cover
             proc.log(
                 "warning",
@@ -257,14 +260,22 @@
 
     @plugin.impl
     async def on_job_running(self, proc: Proc, job: Job):
         """Update the progress bar when a job starts to run"""
         proc.pbar.update_job_running()
 
     @plugin.impl
+    async def on_job_cached(self, proc: Proc, job: Job):
+        """Update the progress bar when a job is cached"""
+        proc.pbar.update_job_submitted()
+        proc.pbar.update_job_running()
+        proc.pbar.update_job_succeeded()
+        job.status = JobStatus.FINISHED
+
+    @plugin.impl
     async def on_job_succeeded(self, proc: Proc, job: Job):
         """Cache the job and update the progress bar when a job is succeeded"""
         # now the returncode is 0, however, we need to check if output files
         # have been created or not, this makes sure job.cache not fail
         for outkey, outtype in job._output_types.items():
             if outtype == ProcOutputType.VAR:
                 continue
```

### Comparing `pipen-0.7.3/pipen/proc.py` & `pipen-0.8.0/pipen/proc.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,36 +18,36 @@
 )
 
 # Slow down the import, try do it at runtime
 # import pandas
 from diot import Diot
 from rich import box
 from rich.panel import Panel
-from slugify import slugify  # type: ignore
 from varname import VarnameException, varname
 from xqute import JobStatus, Xqute
 
 from .defaults import ProcInputType
 from .exceptions import (
     ProcInputKeyError,
     ProcInputTypeError,
     ProcScriptFileNotFound,
-    ProcWorkdirConflictException,
+    PipenOrProcNameError,
 )
 from .pluginmgr import plugin
 from .scheduler import get_scheduler
 from .template import Template, get_template_engine
 from .utils import (
     brief_list,
     cached_property,
     copy_dict,
     desc_from_docstring,
     get_logpanel_width,
     ignore_firstline_dedent,
     is_subclass,
+    is_valid_name,
     log_rich_renderable,
     logger,
     make_df_colnames_unique_inplace,
     strsplit,
     update_dict,
     get_shebang,
     get_base,
@@ -290,14 +290,20 @@
         # triggers cls.__setattr__() to compute requires
         cls.nexts = []
         cls.requires = cls.requires
 
         if cls.name is None or (parent and cls.name == parent.name):
             cls.name = cls.__name__
 
+        if not is_valid_name(cls.name):
+            raise PipenOrProcNameError(
+                f"{cls.name} is not a valid process name, expecting "
+                r"'^[\w.-]+$'"
+            )
+
         cls.envs = update_dict(parent.envs if parent else None, cls.envs)
         cls.plugin_opts = update_dict(
             parent.plugin_opts if parent else None,
             cls.plugin_opts,
         )
         cls.scheduler_opts = update_dict(
             parent.scheduler_opts if parent else {},
@@ -315,18 +321,15 @@
         """
         # instance properties
         self.pipeline = pipeline
 
         self.pbar = None
         self.jobs: List[Any] = []
         self.xqute = None
-        self.__class__.workdir = Path(self.pipeline.workdir) / slugify(
-            self.name
-        )
-
+        self.__class__.workdir = Path(self.pipeline.workdir) / self.name
         # plugins can modify some default attributes
         plugin.hooks.on_proc_init(self)
 
         # Compute the properties
         # otherwise, the property can be accessed directly from class vars
         if self.desc is None:
             self.desc: str = desc_from_docstring(self.__class__)
@@ -356,29 +359,15 @@
         self.output = self._compute_output()
         # scheduler
         self.scheduler = get_scheduler(  # type: ignore
             self.scheduler or self.pipeline.config.scheduler
         )
         # script
         self.script = self._compute_script()  # type: ignore
-
-        # check if it's the same proc using the workdir
-        # since the directory name is slugified
-        proc_name_file = self.workdir / "proc.name"  # type: ignore
-        if (
-            proc_name_file.is_file()
-            and proc_name_file.read_text() != self.name
-        ):
-            raise ProcWorkdirConflictException(
-                "Workdir name is conflicting with process "
-                f"{proc_name_file.read_text()!r}, use a differnt pipeline "
-                "workdir or a different process name."
-            )
         self.workdir.mkdir(exist_ok=True)
-        proc_name_file.write_text(self.name)
 
         if self.submission_batch is None:
             self.submission_batch = self.pipeline.config.submission_batch
 
     async def _init(self) -> None:
         """Init all other properties and jobs"""
         import pandas
@@ -451,18 +440,14 @@
 
         await plugin.hooks.on_proc_start(self)
 
         cached_jobs = []
         for job in self.jobs:
             if await job.cached:
                 cached_jobs.append(job.index)
-                self.pbar.update_job_submitted()
-                self.pbar.update_job_running()
-                self.pbar.update_job_succeeded()
-                job.status = JobStatus.FINISHED
                 await plugin.hooks.on_job_cached(self, job)
             else:
                 await self.xqute.put(job)
         if cached_jobs:
             self.log("info", "Cached jobs: [%s]", brief_list(cached_jobs))
         await self.xqute.run_until_complete()
         self.pbar.done()
```

### Comparing `pipen-0.7.3/pipen/procgroup.py` & `pipen-0.8.0/pipen/procgroup.py`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/progressbar.py` & `pipen-0.8.0/pipen/progressbar.py`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/scheduler.py` & `pipen-0.8.0/pipen/scheduler.py`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/template.py` & `pipen-0.8.0/pipen/template.py`

 * *Files identical despite different names*

### Comparing `pipen-0.7.3/pipen/utils.py` & `pipen-0.8.0/pipen/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Provide some utilities"""
 from __future__ import annotations
 
+import re
 import sys
 import logging
 import textwrap
 import typing
 from itertools import groupby
 from operator import itemgetter
 from io import StringIO
@@ -554,7 +555,19 @@
         mark_name: The mark name
         default: The default value if the mark is not found
 
     Returns:
         The marked value
     """
     return proc.__meta__.get(mark_name, default)
+
+
+def is_valid_name(name: str) -> bool:
+    """Check if a name is valid for a proc or pipen
+
+    Args:
+        name: The name to check
+
+    Returns:
+        True if valid, otherwise False
+    """
+    return re.match(r"^[\w.-]+$", name) is not None
```

### Comparing `pipen-0.7.3/pyproject.toml` & `pipen-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "pipen"
-version = "0.7.3"
+version = "0.8.0"
 description = "A pipeline framework for python"
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen"
 repository = "https://github.com/pwwang/pipen"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dependencies]
-python = "^3.7.1" # align with datar/pandas
+python = "^3.8" # align with datar/pandas
 liquidpy = "^0.8"
-pandas = "^1.3"
-python-slugify = "^8"
+pandas = "^1.4"
 enlighten = "^1"
 cached-property = "^1"
 argx = "^0.2"
 xqute = "^0.1"
 ## included in xqute
 # rich = "^12"
 # diot = "^0.1"
 # simplug = "^0.0"
 ## including rtoml
 python-simpleconf = {version = "^0.5", extras = ["toml"]}
 pipda = "^0.11"
-varname = [
-   {version = "<0.11", python = "<3.8"},
-   {version = "^0.11", python = "^3.8"},
-]
+varname = "^0.11"
 
 [tool.poetry.dev-dependencies]
 openpyxl = "^3"
 pytest = "^7"
 pytest-cov = "^4"
 pytest-xdist = "^3"
 datar = { version = "^0.11", extras = ["pandas"] }
```

### Comparing `pipen-0.7.3/setup.py` & `pipen-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,40 +8,35 @@
 {'': ['*']}
 
 install_requires = \
 ['argx>=0.2,<0.3',
  'cached-property>=1,<2',
  'enlighten>=1,<2',
  'liquidpy>=0.8,<0.9',
- 'pandas>=1.3,<2.0',
+ 'pandas>=1.4,<2.0',
  'pipda>=0.11,<0.12',
  'python-simpleconf[toml]>=0.5,<0.6',
- 'python-slugify>=8,<9',
+ 'varname>=0.11,<0.12',
  'xqute>=0.1,<0.2']
 
-extras_require = \
-{':python_version < "3.8"': ['varname<0.11'],
- ':python_version >= "3.8" and python_version < "4.0"': ['varname>=0.11,<0.12']}
-
 entry_points = \
 {'console_scripts': ['pipen = pipen.cli:main']}
 
 setup_kwargs = {
     'name': 'pipen',
-    'version': '0.7.3',
+    'version': '0.8.0',
     'description': 'A pipeline framework for python',
     'long_description': '<div align="center">\n    <img src="./pipen.png" width="320px">\n\n**A pipeline framework for python**\n\n</div>\n\n______________________________________________________________________\n\n[![Pypi][6]][7] [![Github][8]][9] ![Building][10] [![Docs and API][11]][1] [![Codacy][12]][13] [![Codacy coverage][14]][13] [![Deps][5]][23]\n\n[Documentation][1] | [ChangeLog][2] | [Examples][3] | [API][4]\n\n## Features\n\n- Easy to use\n- Nearly zero-configuration\n- Nice logging\n- Highly extendable\n\n## Installation\n\n```bash\npip install -U pipen\n```\n\n## Quickstart\n\n`example.py`\n\n```python\nfrom pipen import Proc, Pipen\n\nclass P1(Proc):\n    """Sort input file"""\n    input = "infile"\n    input_data = ["/tmp/data.txt"]\n    output = "outfile:file:intermediate.txt"\n    script = "cat {{in.infile}} | sort > {{out.outfile}}"\n\nclass P2(Proc):\n    """Paste line number"""\n    requires = P1\n    input = "infile"\n    output = "outfile:file:result.txt"\n    script = "paste <(seq 1 3) {{in.infile}} > {{out.outfile}}"\n\nclass MyPipeline(Pipen):\n    starts = P1\n\nif __name__ == "__main__":\n    MyPipeline().run()\n```\n\n```shell\n> echo -e "3\\n2\\n1" > /tmp/data.txt\n> python example.py\n```\n\n```log\n[09/13/21 04:23:37] I main                    _____________________________________   __\n[09/13/21 04:23:37] I main                    ___  __ \\___  _/__  __ \\__  ____/__  | / /\n[09/13/21 04:23:37] I main                    __  /_/ /__  / __  /_/ /_  __/  __   |/ /\n[09/13/21 04:23:37] I main                    _  ____/__/ /  _  ____/_  /___  _  /|  /\n[09/13/21 04:23:37] I main                    /_/     /___/  /_/     /_____/  /_/ |_/\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main                                 version: 0.7.0\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main    ╭═════════════════════════════ MYPIPELIN ═══════════════════════════════╮\n[09/13/21 04:23:37] I main    ║  # procs          = 2                                                 ║\n[09/13/21 04:23:37] I main    ║  plugins          = [\'main\', \'verbose-0.0.1\']                         ║\n[09/13/21 04:23:37] I main    ║  profile          = default                                           ║\n[09/13/21 04:23:37] I main    ║  outdir           = mypipeline_results                                ║\n[09/13/21 04:23:37] I main    ║  cache            = True                                              ║\n[09/13/21 04:23:37] I main    ║  dirsig           = 1                                                 ║\n[09/13/21 04:23:37] I main    ║  error_strategy   = ignore                                            ║\n[09/13/21 04:23:37] I main    ║  forks            = 1                                                 ║\n[09/13/21 04:23:37] I main    ║  lang             = bash                                              ║\n[09/13/21 04:23:37] I main    ║  loglevel         = info                                              ║\n[09/13/21 04:23:37] I main    ║  num_retries      = 3                                                 ║\n[09/13/21 04:23:37] I main    ║  plugin_opts      = {}                                                ║\n[09/13/21 04:23:37] I main    ║  plugins          = None                                              ║\n[09/13/21 04:23:37] I main    ║  scheduler        = local                                             ║\n[09/13/21 04:23:37] I main    ║  scheduler_opts   = {}                                                ║\n[09/13/21 04:23:37] I main    ║  submission_batch = 8                                                 ║\n[09/13/21 04:23:37] I main    ║  template         = liquid                                            ║\n[09/13/21 04:23:37] I main    ║  template_opts    = {}                                                ║\n[09/13/21 04:23:37] I main    ║  workdir          = ./.pipen                                          ║\n[09/13/21 04:23:37] I main    ╰═══════════════════════════════════════════════════════════════════════╯\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main    ╭───────────────────────────────── P1 ──────────────────────────────────╮\n[09/13/21 04:23:37] I main    │ Sort input file                                                       │\n[09/13/21 04:23:37] I main    ╰───────────────────────────────────────────────────────────────────────╯\n[09/13/21 04:23:37] I main    P1: Workdir: \'.pipen/mypipeline/p1\'\n[09/13/21 04:23:37] I main    P1: <<< [START]\n[09/13/21 04:23:37] I main    P1: >>> [\'P2\']\n[09/13/21 04:23:37] I verbose P1: size: 1\n[09/13/21 04:23:37] I verbose P1: [0/0] in.infile: /tmp/data.txt\n[09/13/21 04:23:37] I verbose P1: [0/0] out.outfile:\n                      /home/pwwang/github/pipen/.pipen/mypipeline/p1/0/output/intermediate.txt\n[09/13/21 04:23:38] I verbose P1: Time elapsed: 00:00:01.039s\n[09/13/21 04:23:38] I main\n[09/13/21 04:23:38] I main    ╭═════════════════════════════════ P2 ══════════════════════════════════╮\n[09/13/21 04:23:38] I main    ║ Paste line number                                                     ║\n[09/13/21 04:23:38] I main    ╰═══════════════════════════════════════════════════════════════════════╯\n[09/13/21 04:23:38] I main    P2: Workdir: \'.pipen/mypipeline/p2\'\n[09/13/21 04:23:38] I main    P2: <<< [\'P1\']\n[09/13/21 04:23:38] I main    P2: >>> [END]\n[09/13/21 04:23:38] I verbose P2: size: 1\n[09/13/21 04:23:38] I verbose P2: [0/0] in.infile:\n                      /home/pwwang/github/pipen/.pipen/mypipeline/p1/0/output/intermediate.txt\n[09/13/21 04:23:38] I verbose P2: [0/0] out.outfile:\n                      /home/pwwang/github/pipen/mypipeline_results/P2/result.txt\n[09/13/21 04:23:40] I verbose P2: Time elapsed: 00:00:02.074s\n[09/13/21 04:23:40] I main\n\n                PIPEN-0: 100%|████████████████████████████████████████| 2/2 [00:04<00:00, 0.56 procs/s]\n```\n\n```shell\n> cat ./mypipeline_results/P2/result.txt\n1       1\n2       2\n3       3\n```\n\n## Examples\n\nSee more examples at `examples/` and a more realcase example at:\nhttps://github.com/pwwang/pipen-report/tree/master/example\n\n## Plugin gallery\n\nPlugins make `pipen` even better.\n\n- [`pipen-verbose`][15]: Add verbosal information in logs for pipen.\n- [`pipen-lock`][25]: Process lock for pipen to prevent multiple runs at the same time.\n- [`pipen-report`][16]: Generate report for pipen\n- [`pipen-filters`][17]: Add a set of useful filters for pipen templates.\n- [`pipen-diagram`][18]: Draw pipeline diagrams for pipen\n- [`pipen-annotate`][26]: Use docstring to annotate pipen processes\n- [`pipen-args`][19]: Command line argument parser for pipen\n- [`pipen-dry`][20]: Dry runner for pipen pipelines\n- [`pipen-cli-init`][21]: A pipen CLI plugin to create a pipen project (pipeline)\n- [`pipen-cli-run`][22]: A pipen cli plugin to run a process or a pipeline\n- [`pipen-cli-config`][27]: UI wizard to generate configuration for pipen pipelines\n- [`pipen-cli-require`][24]: A pipen cli plugin check the requirements of a pipeline\n\n\n[1]: https://pwwang.github.io/pipen\n[2]: https://pwwang.github.io/pipen/CHANGELOG\n[3]: https://pwwang.github.io/pipen/examples\n[4]: https://pwwang.github.io/pipen/api/pipen\n[5]: https://img.shields.io/librariesio/release/pypi/pipen?style=flat-square\n[6]: https://img.shields.io/pypi/v/pipen?style=flat-square\n[7]: https://pypi.org/project/pipen/\n[8]: https://img.shields.io/github/v/tag/pwwang/pipen?style=flat-square\n[9]: https://github.com/pwwang/pipen\n[10]: https://img.shields.io/github/actions/workflow/status/pwwang/pipen/build.yml?style=flat-square\n[11]: https://img.shields.io/github/actions/workflow/status/pwwang/pipen/docs.yml?label=docs&style=flat-square\n[12]: https://img.shields.io/codacy/grade/cf1c6c97e5c4480386a05b42dec10c6e?style=flat-square\n[13]: https://app.codacy.com/gh/pwwang/pipen\n[14]: https://img.shields.io/codacy/coverage/cf1c6c97e5c4480386a05b42dec10c6e?style=flat-square\n[15]: https://github.com/pwwang/pipen-verbose\n[16]: https://github.com/pwwang/pipen-report\n[17]: https://github.com/pwwang/pipen-filters\n[18]: https://github.com/pwwang/pipen-diagram\n[19]: https://github.com/pwwang/pipen-args\n[20]: https://github.com/pwwang/pipen-dry\n[21]: https://github.com/pwwang/pipen-cli-init\n[22]: https://github.com/pwwang/pipen-cli-run\n[23]: https://libraries.io/github/pwwang/pipen#repository_dependencies\n[24]: https://github.com/pwwang/pipen-cli-require\n[25]: https://github.com/pwwang/pipen-lock\n[26]: https://github.com/pwwang/pipen-annotate\n[27]: https://github.com/pwwang/pipen-cli-config\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pipen-0.7.3/PKG-INFO` & `pipen-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: pipen
-Version: 0.7.3
+Version: 0.8.0
 Summary: A pipeline framework for python
 Home-page: https://github.com/pwwang/pipen
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argx (>=0.2,<0.3)
 Requires-Dist: cached-property (>=1,<2)
 Requires-Dist: enlighten (>=1,<2)
 Requires-Dist: liquidpy (>=0.8,<0.9)
-Requires-Dist: pandas (>=1.3,<2.0)
+Requires-Dist: pandas (>=1.4,<2.0)
 Requires-Dist: pipda (>=0.11,<0.12)
 Requires-Dist: python-simpleconf[toml] (>=0.5,<0.6)
-Requires-Dist: python-slugify (>=8,<9)
-Requires-Dist: varname (<0.11) ; python_version < "3.8"
-Requires-Dist: varname (>=0.11,<0.12) ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: varname (>=0.11,<0.12)
 Requires-Dist: xqute (>=0.1,<0.2)
 Project-URL: Repository, https://github.com/pwwang/pipen
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="./pipen.png" width="320px">
```

