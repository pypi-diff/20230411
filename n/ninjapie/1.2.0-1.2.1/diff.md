# Comparing `tmp/ninjapie-1.2.0.tar.gz` & `tmp/ninjapie-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjapie-1.2.0.tar", last modified: Tue Apr 11 07:41:10 2023, max compression
+gzip compressed data, was "ninjapie-1.2.1.tar", last modified: Tue Apr 11 17:16:00 2023, max compression
```

## Comparing `ninjapie-1.2.0.tar` & `ninjapie-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-11 07:41:10.533646 ninjapie-1.2.0/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    17987 2023-03-26 07:31:08.000000 ninjapie-1.2.0/LICENSE
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27709 2023-04-11 07:41:10.533646 ninjapie-1.2.0/PKG-INFO
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     6330 2023-04-10 08:16:09.000000 ninjapie-1.2.0/README.md
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-11 07:41:10.533646 ninjapie-1.2.0/ninjapie/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)      169 2023-04-10 06:43:40.000000 ninjapie-1.2.0/ninjapie/__init__.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     5045 2023-04-10 06:43:40.000000 ninjapie-1.2.0/ninjapie/__main__.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    28191 2023-04-10 16:28:24.000000 ninjapie-1.2.0/ninjapie/env.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    19502 2023-04-11 07:40:23.000000 ninjapie-1.2.0/ninjapie/generator.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     3894 2023-04-09 16:06:55.000000 ninjapie-1.2.0/ninjapie/path.py
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       22 2023-04-11 07:40:56.000000 ninjapie-1.2.0/ninjapie/version.py
-drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-11 07:41:10.533646 ninjapie-1.2.0/ninjapie.egg-info/
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27709 2023-04-11 07:41:10.000000 ninjapie-1.2.0/ninjapie.egg-info/PKG-INFO
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)      312 2023-04-11 07:41:10.000000 ninjapie-1.2.0/ninjapie.egg-info/SOURCES.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)        1 2023-04-11 07:41:10.000000 ninjapie-1.2.0/ninjapie.egg-info/dependency_links.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       52 2023-04-11 07:41:10.000000 ninjapie-1.2.0/ninjapie.egg-info/entry_points.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       20 2023-04-11 07:41:10.000000 ninjapie-1.2.0/ninjapie.egg-info/top_level.txt
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)     1338 2023-04-11 07:40:56.000000 ninjapie-1.2.0/pyproject.toml
--rw-r--r--   0 hrniels   (1000) hrniels   (1000)       38 2023-04-11 07:41:10.533646 ninjapie-1.2.0/setup.cfg
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-11 17:16:00.393218 ninjapie-1.2.1/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    17987 2023-03-26 07:31:08.000000 ninjapie-1.2.1/LICENSE
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27709 2023-04-11 17:16:00.393218 ninjapie-1.2.1/PKG-INFO
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     6330 2023-04-10 08:16:09.000000 ninjapie-1.2.1/README.md
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-11 17:16:00.393218 ninjapie-1.2.1/ninjapie/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)      169 2023-04-10 06:43:40.000000 ninjapie-1.2.1/ninjapie/__init__.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     5087 2023-04-11 17:15:38.000000 ninjapie-1.2.1/ninjapie/__main__.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    28191 2023-04-10 16:28:24.000000 ninjapie-1.2.1/ninjapie/env.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    19502 2023-04-11 07:40:23.000000 ninjapie-1.2.1/ninjapie/generator.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     3894 2023-04-09 16:06:55.000000 ninjapie-1.2.1/ninjapie/path.py
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       22 2023-04-11 17:15:52.000000 ninjapie-1.2.1/ninjapie/version.py
+drwxr-xr-x   0 hrniels   (1000) hrniels   (1000)        0 2023-04-11 17:16:00.393218 ninjapie-1.2.1/ninjapie.egg-info/
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)    27709 2023-04-11 17:16:00.000000 ninjapie-1.2.1/ninjapie.egg-info/PKG-INFO
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)      312 2023-04-11 17:16:00.000000 ninjapie-1.2.1/ninjapie.egg-info/SOURCES.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)        1 2023-04-11 17:16:00.000000 ninjapie-1.2.1/ninjapie.egg-info/dependency_links.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       52 2023-04-11 17:16:00.000000 ninjapie-1.2.1/ninjapie.egg-info/entry_points.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       29 2023-04-11 17:16:00.000000 ninjapie-1.2.1/ninjapie.egg-info/top_level.txt
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)     1338 2023-04-11 17:15:52.000000 ninjapie-1.2.1/pyproject.toml
+-rw-r--r--   0 hrniels   (1000) hrniels   (1000)       38 2023-04-11 17:16:00.393218 ninjapie-1.2.1/setup.cfg
```

### Comparing `ninjapie-1.2.0/LICENSE` & `ninjapie-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjapie-1.2.0/PKG-INFO` & `ninjapie-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjapie
-Version: 1.2.0
+Version: 1.2.1
 Summary: Ninja-based build system with a Python API
 Author-email: Nils Asmussen <nils.asmussen@barkhauseninstitut.org>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `ninjapie-1.2.0/README.md` & `ninjapie-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ninjapie-1.2.0/ninjapie/__main__.py` & `ninjapie-1.2.1/ninjapie/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,26 +64,26 @@
             reconf = True
 
     # run configure if not done before or it's required
     if reconf or not os.path.isfile(build_file):
         try:
             # run build.py, but don't write *.pyc files
             subprocess.check_call(['python3', '-B', 'build.py'])
-        except Exception:  # pylint: disable=W0718
+        except (Exception, KeyboardInterrupt):  # pylint: disable=W0718
             return 1
 
         # store new list of files from globs
         new_files = all_files(build_dir)
         with open(all_files_path, 'w', encoding='utf-8') as file:
             file.write(new_files)
 
     # now build everything with ninja
     try:
         subprocess.check_call(['ninja', '-f', build_file] + ninja_args, stdout=sys.stderr.buffer)
-    except Exception:  # pylint: disable=W0718
+    except (Exception, KeyboardInterrupt):  # pylint: disable=W0718
         # ensure that we regenerate the build.ninja next time. Since ninja does not accept the
         # build.ninja, it will also not detect changes our build files in order to regenerate it.
         # Therefore, force a regenerate next time by removing the file.
         os.remove(all_files_path)
         return 1
 
     return 0
```

### Comparing `ninjapie-1.2.0/ninjapie/env.py` & `ninjapie-1.2.1/ninjapie/env.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.2.0/ninjapie/generator.py` & `ninjapie-1.2.1/ninjapie/generator.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.2.0/ninjapie/path.py` & `ninjapie-1.2.1/ninjapie/path.py`

 * *Files identical despite different names*

### Comparing `ninjapie-1.2.0/ninjapie.egg-info/PKG-INFO` & `ninjapie-1.2.1/ninjapie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjapie
-Version: 1.2.0
+Version: 1.2.1
 Summary: Ninja-based build system with a Python API
 Author-email: Nils Asmussen <nils.asmussen@barkhauseninstitut.org>
 License: 		    GNU GENERAL PUBLIC LICENSE
         		       Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `ninjapie-1.2.0/pyproject.toml` & `ninjapie-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ninjapie"
-version = "1.2.0"
+version = "1.2.1"
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
-current_version = "1.2.0"
+current_version = "1.2.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}."
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

