# Comparing `tmp/gardener-component-model-0.0.9.tar.gz` & `tmp/gardener-component-model-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gardener-component-model-0.0.9.tar", last modified: Tue Oct 27 13:09:24 2020, max compression
+gzip compressed data, was "gardener-component-model-0.0.90.tar", last modified: Tue Apr 11 13:53:52 2023, max compression
```

## Comparing `gardener-component-model-0.0.9.tar` & `gardener-component-model-0.0.90.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 13:09:24.019292 gardener-component-model-0.0.9/
--rw-r--r--   0 root         (0) root         (0)      202 2020-10-27 13:09:24.019292 gardener-component-model-0.0.9/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 13:09:24.019292 gardener-component-model-0.0.9/gardener_component_model.egg-info/
--rw-r--r--   0 root         (0) root         (0)      202 2020-10-27 13:09:23.000000 gardener-component-model-0.0.9/gardener_component_model.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      296 2020-10-27 13:09:23.000000 gardener-component-model-0.0.9/gardener_component_model.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-10-27 13:09:23.000000 gardener-component-model-0.0.9/gardener_component_model.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2020-10-27 13:09:23.000000 gardener-component-model-0.0.9/gardener_component_model.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2020-10-27 13:09:23.000000 gardener-component-model-0.0.9/gardener_component_model.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 13:09:24.019292 gardener-component-model-0.0.9/gci/
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-27 13:07:51.000000 gardener-component-model-0.0.9/gci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5099 2020-10-27 13:07:51.000000 gardener-component-model-0.0.9/gci/componentmodel.py
--rw-r--r--   0 root         (0) root         (0)     1957 2020-10-27 13:07:51.000000 gardener-component-model-0.0.9/gci/oci.py
--rw-r--r--   0 root         (0) root         (0)       38 2020-10-27 13:09:24.023292 gardener-component-model-0.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      880 2020-10-27 13:07:51.000000 gardener-component-model-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:53:52.321206 gardener-component-model-0.0.90/
+-rw-r--r--   0 root         (0) root         (0)      126 2023-04-11 13:53:52.321206 gardener-component-model-0.0.90/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:53:52.321206 gardener-component-model-0.0.90/gardener_component_model.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      126 2023-04-11 13:53:52.000000 gardener-component-model-0.0.90/gardener_component_model.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      338 2023-04-11 13:53:52.000000 gardener-component-model-0.0.90/gardener_component_model.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 13:53:52.000000 gardener-component-model-0.0.90/gardener_component_model.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-11 13:53:52.000000 gardener-component-model-0.0.90/gardener_component_model.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-11 13:53:52.000000 gardener-component-model-0.0.90/gardener_component_model.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:53:52.321206 gardener-component-model-0.0.90/gci/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-04-11 13:53:18.000000 gardener-component-model-0.0.90/gci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-04-11 13:53:19.000000 gardener-component-model-0.0.90/gci/component-descriptor.json-schema.yaml
+-rw-r--r--   0 root         (0) root         (0)    17809 2023-04-11 13:53:18.000000 gardener-component-model-0.0.90/gci/componentmodel.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2023-04-11 13:53:18.000000 gardener-component-model-0.0.90/gci/oci.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-11 13:53:52.321206 gardener-component-model-0.0.90/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      942 2023-04-11 13:53:18.000000 gardener-component-model-0.0.90/setup.py
```

### Comparing `gardener-component-model-0.0.9/setup.py` & `gardener-component-model-0.0.90/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,13 +22,13 @@
             yield line
 
 
 setuptools.setup(
     name='gardener-component-model',
     version=version(),
     description='Gardener Component Model',
-    python_requires='>=3.8.*',
+    python_requires='>=3.9',
     packages=setuptools.find_packages(),
+    package_data={'gci': ['component-descriptor.json-schema.yaml']},
     install_requires=list(requirements()),
-    entry_points={
-    },
+    entry_points={},
 )
```

