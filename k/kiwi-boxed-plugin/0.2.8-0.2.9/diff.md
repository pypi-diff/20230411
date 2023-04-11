# Comparing `tmp/kiwi_boxed_plugin-0.2.8.tar.gz` & `tmp/kiwi_boxed_plugin-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kiwi_boxed_plugin-0.2.8.tar", last modified: Mon Apr 19 09:21:34 2021, max compression
+gzip compressed data, was "dist/kiwi_boxed_plugin-0.2.9.tar", last modified: Wed May  5 13:04:22 2021, max compression
```

## Comparing `kiwi_boxed_plugin-0.2.8.tar` & `kiwi_boxed_plugin-0.2.9.tar`

### file list

```diff
@@ -1,46 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-19 09:21:34.000000 kiwi_boxed_plugin-0.2.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-19 09:21:34.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-19 09:21:33.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1282 2021-04-19 09:21:33.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1098 2021-04-19 09:21:34.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-19 09:21:33.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2021-04-19 09:21:33.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       72 2021-04-19 09:21:33.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       18 2021-04-19 09:21:33.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      152 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/.bumpversion.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-19 09:21:34.000000 kiwi_boxed_plugin-0.2.8/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-19 09:21:34.000000 kiwi_boxed_plugin-0.2.8/doc/build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-19 09:21:34.000000 kiwi_boxed_plugin-0.2.8/doc/build/man/
--rw-r--r--   0 root         (0) root         (0)     4240 2021-04-19 09:21:12.000000 kiwi_boxed_plugin-0.2.8/doc/build/man/kiwi::system::boxbuild.8
--rw-rw-rw-   0 root         (0) root         (0)      727 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/.virtualenv.dev-requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)    35149 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-19 09:21:34.000000 kiwi_boxed_plugin-0.2.8/package/
--rw-rw-rw-   0 root         (0) root         (0)      235 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/package/python-kiwi_boxed_plugin.changes
--rw-rw-rw-   0 root         (0) root         (0)      324 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/package/python-kiwi_boxed_plugin-rpmlintrc
--rw-rw-rw-   0 root         (0) root         (0)     3753 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/package/python-kiwi_boxed_plugin-spec-template
--rw-r--r--   0 root         (0) root         (0)     1282 2021-04-19 09:21:34.000000 kiwi_boxed_plugin-0.2.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      417 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     2454 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/tox.ini
--rw-rw-rw-   0 root         (0) root         (0)      423 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1988 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      456 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/.virtualenv.requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-19 09:21:34.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/
--rw-rw-rw-   0 root         (0) root         (0)     4241 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     6259 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/box_download.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      899 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/version.py
--rw-rw-rw-   0 root         (0) root         (0)     2482 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/plugin_config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-19 09:21:34.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/utils/
--rw-rw-rw-   0 root         (0) root         (0)     2945 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/utils/dir_files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-19 09:21:34.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2998 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/config/kiwi_boxed_plugin.yml
--rw-rw-rw-   0 root         (0) root         (0)     5717 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/box_build.py
--rw-rw-rw-   0 root         (0) root         (0)     2368 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/plugin_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2950 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/box_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-19 09:21:34.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8085 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/tasks/system_boxbuild.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2021-04-19 09:21:34.000000 kiwi_boxed_plugin-0.2.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1652 2021-04-19 09:20:50.000000 kiwi_boxed_plugin-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1652 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/package/
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/package/python-kiwi_boxed_plugin-rpmlintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/package/python-kiwi_boxed_plugin.changes
+-rw-r--r--   0 runner    (1001) docker     (121)     3753 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/package/python-kiwi_boxed_plugin-spec-template
+-rw-r--r--   0 runner    (1001) docker     (121)      417 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      727 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/.virtualenv.dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      456 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/.virtualenv.requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2372 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1282 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1988 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     1282 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/
+-rw-r--r--   0 runner    (1001) docker     (121)     6259 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/box_download.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     2945 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/utils/dir_files.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/config/
+-rw-r--r--   0 runner    (1001) docker     (121)     2998 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/config/kiwi_boxed_plugin.yml
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6537 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/box_build.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 13:04:22.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)     8299 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/tasks/system_boxbuild.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/plugin_config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4259 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2950 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/box_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2368 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/plugin_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1454 2021-05-05 13:03:49.000000 kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/exceptions.py
```

### Comparing `kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin.egg-info/PKG-INFO` & `kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwi-boxed-plugin
-Version: 0.2.8
+Version: 0.2.9
 Summary: KIWI - Boxed Build Plugin
 Home-page: https://github.com/OSInside/kiwi-boxed-plugin
 Author: Marcus Schaefer
 Author-email: ms@suse.com
 License: GPLv3+
 Download-URL: https://download.opensuse.org/repositories/Virtualization:/Appliances:/Builder
 Description: KIWI - Boxed Build Plugin
```

### Comparing `kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin.egg-info/SOURCES.txt` & `kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 setup.cfg
 setup.py
 tox.ini
-doc/build/man/kiwi::system::boxbuild.8
 kiwi_boxed_plugin/__init__.py
 kiwi_boxed_plugin/box_build.py
 kiwi_boxed_plugin/box_config.py
 kiwi_boxed_plugin/box_download.py
 kiwi_boxed_plugin/defaults.py
 kiwi_boxed_plugin/exceptions.py
 kiwi_boxed_plugin/plugin_config.py
```

### Comparing `kiwi_boxed_plugin-0.2.8/.virtualenv.dev-requirements.txt` & `kiwi_boxed_plugin-0.2.9/.virtualenv.dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `kiwi_boxed_plugin-0.2.8/LICENSE` & `kiwi_boxed_plugin-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwi_boxed_plugin-0.2.8/package/python-kiwi_boxed_plugin-spec-template` & `kiwi_boxed_plugin-0.2.9/package/python-kiwi_boxed_plugin-spec-template`

 * *Files identical despite different names*

### Comparing `kiwi_boxed_plugin-0.2.8/PKG-INFO` & `kiwi_boxed_plugin-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwi_boxed_plugin
-Version: 0.2.8
+Version: 0.2.9
 Summary: KIWI - Boxed Build Plugin
 Home-page: https://github.com/OSInside/kiwi-boxed-plugin
 Author: Marcus Schaefer
 Author-email: ms@suse.com
 License: GPLv3+
 Download-URL: https://download.opensuse.org/repositories/Virtualization:/Appliances:/Builder
 Description: KIWI - Boxed Build Plugin
```

### Comparing `kiwi_boxed_plugin-0.2.8/tox.ini` & `kiwi_boxed_plugin-0.2.9/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -106,8 +106,7 @@
 # PyPi upload
 [testenv:release]
 deps = {[testenv]deps}
 skip_install = True
 usedevelop = True
 commands =
     python setup.py sdist
-    twine upload --skip-existing --non-interactive --config-file ./.pypirc dist/*
```

### Comparing `kiwi_boxed_plugin-0.2.8/Makefile` & `kiwi_boxed_plugin-0.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/defaults.py` & `kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def get_plugin_config_file():
         return resource_filename(
             'kiwi_boxed_plugin', 'config/kiwi_boxed_plugin.yml'
         )
 
     @staticmethod
     def get_local_box_cache_dir():
-        return '/var/tmp/kiwi/boxes'
+        return f'{os.environ.get("HOME")}/.kiwi_boxes'
 
     @staticmethod
     def get_qemu_generic_setup():
         return [
             '-nographic',
             '-nodefaults',
             '-snapshot'
```

### Comparing `kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/box_download.py` & `kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/box_download.py`

 * *Files identical despite different names*

### Comparing `kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/version.py` & `kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with kiwi-boxed-build.  If not, see <http://www.gnu.org/licenses/>
 #
 """
 Global version information used in kiwi-boxed-build and the package
 """
-__version__ = '0.2.8'
+__version__ = '0.2.9'
 __githash__ = '$Format:%H$'
```

### Comparing `kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/plugin_config_schema.py` & `kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/plugin_config_schema.py`

 * *Files identical despite different names*

### Comparing `kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/utils/dir_files.py` & `kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/utils/dir_files.py`

 * *Files identical despite different names*

### Comparing `kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/config/kiwi_boxed_plugin.yml` & `kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/config/kiwi_boxed_plugin.yml`

 * *Files identical despite different names*

### Comparing `kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/box_build.py` & `kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/box_build.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,32 +21,40 @@
 from kiwi.path import Path
 
 from kiwi_boxed_plugin.box_download import BoxDownload
 from kiwi_boxed_plugin.defaults import Defaults
 
 import kiwi_boxed_plugin.defaults as runtime
 
+from kiwi_boxed_plugin.exceptions import KiwiBoxPluginQEMUBinaryNotFound
+
 log = logging.getLogger('kiwi')
 
 
 class BoxBuild:
     """
     **Implements boxbuild command**
 
     Implements an interface to run a kiwi build box using
     the KVM virtualization platform
 
-    :param string boxname: name of the box from kiwi_boxed_plugin.yml
-    :param string arch: arch name for box
+    :param str boxname: name of the box from kiwi_boxed_plugin.yml
+    :param str ram: amount of main memory to use for the box
+    :param str smp: number of CPUs to use in the SMP setup for the box
+    :param str arch: arch name for box
+    :param str machine: machine emulaton type for the box
+    :param str cpu: CPU emulation type
+    :param str sharing_backend: guest/host sharing backend type
     """
     def __init__(
-        self, boxname, ram=None, arch=None, machine=None,
+        self, boxname, ram=None, smp=None, arch=None, machine=None,
         cpu='host', sharing_backend='9p'
     ):
         self.ram = ram
+        self.smp = smp
         self.cpu = cpu
         self.machine = machine
         self.arch = arch or platform.machine()
         self.box = BoxDownload(boxname, arch)
         self.sharing_backend = sharing_backend
 
     def run(
@@ -100,16 +108,21 @@
         if self.machine:
             vm_machine.append(self.machine)
         if self.arch == 'x86_64':
             # KVM is only present for Intel and AMD
             vm_machine.append('accel=kvm')
         vm_machine.append('-cpu')
         vm_machine.append(self.cpu)
+        qemu_binary = self._find_qemu_call_binary()
+        if not qemu_binary:
+            raise KiwiBoxPluginQEMUBinaryNotFound(
+                f'No QEMU binary for {self.arch} found'
+            )
         vm_run = [
-            'qemu-system-{0}'.format(self.arch),
+            qemu_binary,
             '-m', format(self.ram or vm_setup.ram)
         ] + vm_machine + [
         ] + Defaults.get_qemu_generic_setup() + [
             '-kernel', vm_setup.kernel,
             '-append', '"{0}"'.format(' '.join(vm_append))
         ] + Defaults.get_qemu_storage_setup(vm_setup.system, snapshot) + \
             Defaults.get_qemu_network_setup() + \
@@ -128,15 +141,15 @@
                     'memory-backend-file', self.ram or vm_setup.ram, '/dev/shm'
                 ),
                 '-numa', 'node,memdev=mem'
             ]
         if vm_setup.initrd:
             vm_run += ['-initrd', vm_setup.initrd]
         if vm_setup.smp:
-            vm_run += ['-smp', format(vm_setup.smp)]
+            vm_run += ['-smp', format(self.smp or vm_setup.smp)]
         os.environ['TMPDIR'] = Defaults.get_local_box_cache_dir()
         log.debug(
             'Set TMPDIR: {0}'.format(os.environ['TMPDIR'])
         )
         log.debug(
             'Calling Qemu: {0}'.format(vm_run)
         )
@@ -154,7 +167,13 @@
     def _pop_arg_param(self, arg):
         arg_index = self.kiwi_build_command.index(arg)
         if arg_index:
             value = self.kiwi_build_command[arg_index + 1]
             del self.kiwi_build_command[arg_index + 1]
             del self.kiwi_build_command[arg_index]
             return value
+
+    def _find_qemu_call_binary(self):
+        qemu_by_system = Path.which(f'qemu-system-{self.arch}')
+        if qemu_by_system:
+            return qemu_by_system
+        return Path.which('qemu-kvm') if self.arch == 'x86_64' else None
```

### Comparing `kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/plugin_config.py` & `kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/plugin_config.py`

 * *Files identical despite different names*

### Comparing `kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/exceptions.py` & `kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,7 +36,14 @@
     """
 
 
 class KiwiBoxPluginArchNotFoundError(KiwiError):
     """
     Exception raised if the selected architecture has no configuration
     """
+
+
+class KiwiBoxPluginQEMUBinaryNotFound(KiwiError):
+    """
+    Exception raised if no QEMU binary for the desired architecture
+    could be found
+    """
```

### Comparing `kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/box_config.py` & `kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/box_config.py`

 * *Files identical despite different names*

### Comparing `kiwi_boxed_plugin-0.2.8/kiwi_boxed_plugin/tasks/system_boxbuild.py` & `kiwi_boxed_plugin-0.2.9/kiwi_boxed_plugin/tasks/system_boxbuild.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with kiwi-boxed-build.  If not, see <http://www.gnu.org/licenses/>
 #
 """
 usage: kiwi-ng system boxbuild -h | --help
        kiwi-ng system boxbuild --box=<name>
            [--box-memory=<vmgb>]
+           [--box-smp-cpus=<number>]
            [--box-debug]
            [--kiwi-version=<version>]
            [--shared-path=<path>]
            [--no-update-check]
            [--no-snapshot]
            [--9p-sharing | --virtiofs-sharing]
            [--x86_64 | --aarch64]
@@ -46,14 +47,18 @@
     --list-boxes
         show available build boxes.
 
     --box-memory=<vmgb>
         Number of GBs to reserve as main memory for the virtual
         machine. By default 8GB will be used.
 
+    --box-smp-cpus=<number>
+        Number of CPUs to use in the SMP setup. By default
+        4 CPUs will be used
+
     --no-update-check
         Skip check for available box update. The option has no
         effect if the selected box does not yet exist on the host.
 
     --no-snapshot
         Run box with snapshot mode switched off. This causes the
         box disk file to be modified by the build process and allows
@@ -148,14 +153,15 @@
             )
             keep_open = self.command_args.get('--box-debug')
             kiwi_version = self.command_args.get('--kiwi-version')
             shared_path = self.command_args.get('--shared-path')
             box_build = BoxBuild(
                 boxname=self.command_args.get('--box'),
                 ram=self.command_args.get('--box-memory'),
+                smp=self.command_args.get('--box-smp-cpus'),
                 arch=self._get_box_arch(),
                 machine=self.command_args.get('--machine'),
                 cpu=self.command_args.get('--cpu') or 'host',
                 sharing_backend=self._get_sharing_backend()
             )
             box_build.run(
                 self._validate_kiwi_build_command(),
```

### Comparing `kiwi_boxed_plugin-0.2.8/setup.py` & `kiwi_boxed_plugin-0.2.9/setup.py`

 * *Files identical despite different names*

