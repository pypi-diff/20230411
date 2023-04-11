# Comparing `tmp/deep_agent-0.1.dev0.tar.gz` & `tmp/deep_agent-0.2.dev0.tar.gz`

## Comparing `deep_agent-0.1.dev0.tar` & `deep_agent-0.2.dev0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 deep_agent-0.1.dev0/.gitignore
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 deep_agent-0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 deep_agent-0.1.dev0/../../README.md
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 deep_agent-0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 deep_agent-0.2.dev0/.gitignore
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 deep_agent-0.2.dev0/pyproject.toml
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 deep_agent-0.2.dev0/../../README.md
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 deep_agent-0.2.dev0/PKG-INFO
```

### Comparing `deep_agent-0.1.dev0/pyproject.toml` & `deep_agent-0.2.dev0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 dependencies = []
-version = "0.1-dev"
+version = "0.2-dev"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "src/deep",
 ]
 
 [tool.hatch.build.targets.wheel]
```

### Comparing `deep_agent-0.1.dev0/PKG-INFO` & `deep_agent-0.2.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-agent
-Version: 0.1.dev0
+Version: 0.2.dev0
 Summary: DEEP Python Protobuf
 Author-email: Ben Donnelly <b.w.donnelly1@gmail.com>
 License-Expression: Apache-2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

