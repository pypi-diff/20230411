# Comparing `tmp/ninjapie-1.1.0.tar.gz` & `tmp/ninjapie-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjapie-1.1.0.tar", last modified: Mon Apr 10 06:38:42 2023, max compression
+gzip compressed data, was "ninjapie-1.2.0.tar", last modified: Tue Apr 11 07:41:10 2023, max compression
```

## Comparing `ninjapie-1.1.0.tar` & `ninjapie-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-10 06:38:42.496231 ninjapie-1.1.0/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    17987 2023-03-26 07:31:08.000000 ninjapie-1.1.0/LICENSE
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-10 06:38:42.496231 ninjapie-1.1.0/PKG-INFO
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     6139 2023-04-09 11:30:25.000000 ninjapie-1.1.0/README.md
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-10 06:38:42.496231 ninjapie-1.1.0/ninjapie/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)      169 2023-04-10 06:20:47.000000 ninjapie-1.1.0/ninjapie/__init__.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     5045 2023-04-10 06:32:28.000000 ninjapie-1.1.0/ninjapie/__main__.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27728 2023-04-09 16:36:42.000000 ninjapie-1.1.0/ninjapie/env.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    19340 2023-04-09 15:57:25.000000 ninjapie-1.1.0/ninjapie/generator.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     3894 2023-04-09 16:06:55.000000 ninjapie-1.1.0/ninjapie/path.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       22 2023-04-10 06:36:28.000000 ninjapie-1.1.0/ninjapie/version.py
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-10 06:38:42.496231 ninjapie-1.1.0/ninjapie.egg-info/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27518 2023-04-10 06:38:42.000000 ninjapie-1.1.0/ninjapie.egg-info/PKG-INFO
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)      312 2023-04-10 06:38:42.000000 ninjapie-1.1.0/ninjapie.egg-info/SOURCES.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)        1 2023-04-10 06:38:42.000000 ninjapie-1.1.0/ninjapie.egg-info/dependency_links.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       52 2023-04-10 06:38:42.000000 ninjapie-1.1.0/ninjapie.egg-info/entry_points.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       20 2023-04-10 06:38:42.000000 ninjapie-1.1.0/ninjapie.egg-info/top_level.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     1338 2023-04-10 06:36:28.000000 ninjapie-1.1.0/pyproject.toml
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       38 2023-04-10 06:38:42.496231 ninjapie-1.1.0/setup.cfg
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-11 07:41:10.533646 ninjapie-1.2.0/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    17987 2023-03-26 07:31:08.000000 ninjapie-1.2.0/LICENSE
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27709 2023-04-11 07:41:10.533646 ninjapie-1.2.0/PKG-INFO
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     6330 2023-04-10 08:16:09.000000 ninjapie-1.2.0/README.md
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-11 07:41:10.533646 ninjapie-1.2.0/ninjapie/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)      169 2023-04-10 06:43:40.000000 ninjapie-1.2.0/ninjapie/__init__.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     5045 2023-04-10 06:43:40.000000 ninjapie-1.2.0/ninjapie/__main__.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    28191 2023-04-10 16:28:24.000000 ninjapie-1.2.0/ninjapie/env.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    19502 2023-04-11 07:40:23.000000 ninjapie-1.2.0/ninjapie/generator.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     3894 2023-04-09 16:06:55.000000 ninjapie-1.2.0/ninjapie/path.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       22 2023-04-11 07:40:56.000000 ninjapie-1.2.0/ninjapie/version.py
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-11 07:41:10.533646 ninjapie-1.2.0/ninjapie.egg-info/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27709 2023-04-11 07:41:10.000000 ninjapie-1.2.0/ninjapie.egg-info/PKG-INFO
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)      312 2023-04-11 07:41:10.000000 ninjapie-1.2.0/ninjapie.egg-info/SOURCES.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)        1 2023-04-11 07:41:10.000000 ninjapie-1.2.0/ninjapie.egg-info/dependency_links.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       52 2023-04-11 07:41:10.000000 ninjapie-1.2.0/ninjapie.egg-info/entry_points.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       20 2023-04-11 07:41:10.000000 ninjapie-1.2.0/ninjapie.egg-info/top_level.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     1338 2023-04-11 07:40:56.000000 ninjapie-1.2.0/pyproject.toml
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       38 2023-04-11 07:41:10.533646 ninjapie-1.2.0/setup.cfg
```

### Comparing `ninjapie-1.1.0/LICENSE` & `ninjapie-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjapie-1.1.0/PKG-INFO` & `ninjapie-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjapie
-Version: 1.1.0
+Version: 1.2.0
 Summary: Ninja-based build system with a Python API
 Author-email: Nils Asmussen <nils.asmussen@barkhauseninstitut.org>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -351,14 +351,17 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/ninjapie.svg)](https://badge.fury.io/py/ninjapie)
+![pylint](https://github.com/Barkhausen-Institut/Ninjapie/actions/workflows/pylint.yml/badge.svg)
+
 Ninjapie
 ========
 
 Ninjapie is a tool for automating the building of software. It builds upon [Ninja](https://ninja-build.org) and provides a Python API to describe the build. The basic idea is to take the flexibility and simplicity of [SCons](https://scons.org) and combine it with the performance of Ninja.
 
 # Why Ninjapie?
```

### Comparing `ninjapie-1.1.0/README.md` & `ninjapie-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[![PyPI version](https://badge.fury.io/py/ninjapie.svg)](https://badge.fury.io/py/ninjapie)
+![pylint](https://github.com/Barkhausen-Institut/Ninjapie/actions/workflows/pylint.yml/badge.svg)
+
 Ninjapie
 ========
 
 Ninjapie is a tool for automating the building of software. It builds upon [Ninja](https://ninja-build.org) and provides a Python API to describe the build. The basic idea is to take the flexibility and simplicity of [SCons](https://scons.org) and combine it with the performance of Ninja.
 
 # Why Ninjapie?
```

### Comparing `ninjapie-1.1.0/ninjapie/__main__.py` & `ninjapie-1.2.0/ninjapie/__main__.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.1.0/ninjapie/env.py` & `ninjapie-1.2.0/ninjapie/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,26 +240,36 @@
         ... gen.write_to_file()
         And the `build.py` in the subdirectory `sub`:
         >>> def build(gen, env):
         ...     env.static_lib(gen, out='sub', ins=['sub.c'])
 
         This example would produce `libsub.a` in the subdirectory and use it to produce the `hello`
         executable in the root directory.
+
+        Parameters
+        ----------
+        :param gen: the generator
+        :param dir: the subdirectory to enter
+
+        Returns
+        -------
+        The return value of the build function in the subdirectory
         """
 
         old_cwd = self.cur_dir
         self._cwd.path += '/' + dir
 
         gen._add_build_file(self.cur_dir + '/build.py')
 
         mod_path = self.cur_dir[2:].replace('/', '.')
         sub = importlib.import_module(mod_path + '.build')
-        sub.build(gen, self)
+        res = sub.build(gen, self)
 
         self._cwd.path = old_cwd
+        return res
 
     def glob(self, gen: Generator, pattern: str) -> list[SourcePath]:
         """
         Produces a list of files that match the given pattern
 
         The pattern uses the same syntax as the Python function `glob.glob`. For example, '*.c'
         produces a list of all C files in the current directory. Since the `recursive` argument to
@@ -269,14 +279,23 @@
         Note that globbing has the side effect that the required build steps might change on added
         or removed files. For that reason, Ninjapie records the glob patterns and regenerates the
         ninja build file whenever any file is added or removed. In other words, using `Env.glob` is
         a trade-off between more convenience and faster builds, because Ninjapie needs to perform
         additional checks for globs. Note that this also means that *only* this function should be
         used for globbing, because all other ways bypass Ninjapie and therefore lead to potentially
         outdated ninja build files.
+
+        Parameters
+        ----------
+        :param gen: the generator
+        :param pattern: the pattern for globbing
+
+        Returns
+        -------
+        The list of found files as `SourcePath` objects
         """
 
         pat = SourcePath.new(self, pattern)
         gen._add_glob(pat)
         files = glob(pat, recursive=True)
         return [SourcePath(f) for f in files]
 
@@ -618,15 +637,15 @@
         The input files can be all file types that `Env.objs` supports.
 
         Parameters
         ----------
         :param gen: the generator
         :param out: the output file
         :param ins: the list of input files
-        :param libs: the list of libraries that the executable should be linked against
+        :param libs: the list of library names that the executable should be linked against
         :param deps: the additional list of dependencies
 
         Variables
         ---------
         :param `CC`: the tool name (e.g., 'gcc')
         :param `LINKFLAGS`: the flags (e.g., ['-march=rv64imafdc'])
         :param `LIBPATH`: the paths to search libraries in (e.g., ['lib'])
@@ -648,15 +667,15 @@
         The input files can be all file types that `Env.objs` supports.
 
         Parameters
         ----------
         :param gen: the generator
         :param out: the output file
         :param ins: the list of input files
-        :param libs: the list of libraries that the executable should be linked against
+        :param libs: the list of library names that the executable should be linked against
         :param deps: the additional list of dependencies
 
         Variables
         ---------
         :param `CXX`: the tool name (e.g., 'g++')
         :param `LINKFLAGS`: the flags (e.g., ['-march=rv64imafdc'])
         :param `LIBPATH`: the paths to search libraries in (e.g., ['lib'])
```

### Comparing `ninjapie-1.1.0/ninjapie/generator.py` & `ninjapie-1.2.0/ninjapie/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,16 +255,20 @@
         :param rule: The `Rule` object to add
         """
 
         assert edge.rule in self._rules
 
         if self._debug:
             for ex_edge in self._build_edges:
+                # skip edges that don't have a calltrace (e.g., the always-rebuild rule)
+                if ex_edge.calltrace is None:
+                    continue
+
                 for out in ex_edge.outs:
-                    assert out not in ex_edge.outs, \
+                    assert out not in edge.outs, \
                         "Output '{}' is already produced by the build edge added here:\n{}".format(
                             out, ''.join(traceback.format_list(ex_edge.calltrace)))
             edge.calltrace = traceback.extract_stack()
 
         self._rules[edge.rule].refs += 1
         self._build_edges.append(edge)
```

### Comparing `ninjapie-1.1.0/ninjapie/path.py` & `ninjapie-1.2.0/ninjapie/path.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.1.0/ninjapie.egg-info/PKG-INFO` & `ninjapie-1.2.0/ninjapie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjapie
-Version: 1.1.0
+Version: 1.2.0
 Summary: Ninja-based build system with a Python API
 Author-email: Nils Asmussen <nils.asmussen@barkhauseninstitut.org>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -351,14 +351,17 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/ninjapie.svg)](https://badge.fury.io/py/ninjapie)
+![pylint](https://github.com/Barkhausen-Institut/Ninjapie/actions/workflows/pylint.yml/badge.svg)
+
 Ninjapie
 ========
 
 Ninjapie is a tool for automating the building of software. It builds upon [Ninja](https://ninja-build.org) and provides a Python API to describe the build. The basic idea is to take the flexibility and simplicity of [SCons](https://scons.org) and combine it with the performance of Ninja.
 
 # Why Ninjapie?
```

### Comparing `ninjapie-1.1.0/pyproject.toml` & `ninjapie-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ninjapie"
-version = "1.1.0"
+version = "1.2.0"
 description = "Ninja-based build system with a Python API"
 readme = "README.md"
 authors = [{ name = "Nils Asmussen", email = "nils.asmussen@barkhauseninstitut.org" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -30,15 +30,15 @@
 [tool.setuptools]
 include-package-data = false
 
 [tool.setuptools.packages.find]
 exclude = ["coverage*", "tests*"]
 
 [tool.bumpver]
-current_version = "1.1.0"
+current_version = "1.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}."
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

