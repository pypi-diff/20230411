# Comparing `tmp/kfp-tekton-1.6.4.tar.gz` & `tmp/kfp-tekton-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-tekton-1.6.4.tar", last modified: Wed Mar 22 20:00:30 2023, max compression
+gzip compressed data, was "kfp-tekton-1.6.5.tar", last modified: Tue Apr 11 19:49:28 2023, max compression
```

## Comparing `kfp-tekton-1.6.4.tar` & `kfp-tekton-1.6.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-03-22 20:00:30.508252 kfp-tekton-1.6.4/
--rw-r--r--   0 tommyli    (501) staff       (20)    11889 2023-03-22 20:00:30.507705 kfp-tekton-1.6.4/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)    16444 2023-03-22 19:58:35.000000 kfp-tekton-1.6.4/README.md
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-03-22 20:00:30.496012 kfp-tekton-1.6.4/kfp_tekton/
--rw-r--r--   0 tommyli    (501) staff       (20)      713 2023-03-22 19:58:35.000000 kfp-tekton-1.6.4/kfp_tekton/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)    30584 2023-03-20 18:35:30.000000 kfp-tekton-1.6.4/kfp_tekton/_client.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-03-22 20:00:30.506701 kfp-tekton-1.6.4/kfp_tekton/compiler/
--rw-r--r--   0 tommyli    (501) staff       (20)      675 2023-02-21 19:36:36.000000 kfp-tekton-1.6.4/kfp_tekton/compiler/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)    44521 2023-02-21 19:36:36.000000 kfp-tekton-1.6.4/kfp_tekton/compiler/_data_passing_rewriter.py
--rw-r--r--   0 tommyli    (501) staff       (20)     7091 2023-03-20 18:35:30.000000 kfp-tekton-1.6.4/kfp_tekton/compiler/_k8s_helper.py
--rw-r--r--   0 tommyli    (501) staff       (20)    32108 2023-03-17 18:34:11.000000 kfp-tekton-1.6.4/kfp_tekton/compiler/_op_to_template.py
--rw-r--r--   0 tommyli    (501) staff       (20)    30933 2023-03-20 18:35:30.000000 kfp-tekton-1.6.4/kfp_tekton/compiler/_tekton_handler.py
--rw-r--r--   0 tommyli    (501) staff       (20)    99548 2023-03-20 18:35:30.000000 kfp-tekton-1.6.4/kfp_tekton/compiler/compiler.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4354 2023-02-21 19:36:36.000000 kfp-tekton-1.6.4/kfp_tekton/compiler/main.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4088 2023-03-17 18:33:39.000000 kfp-tekton-1.6.4/kfp_tekton/compiler/pipeline_utils.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2071 2023-02-21 19:36:36.000000 kfp-tekton-1.6.4/kfp_tekton/compiler/yaml_utils.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1311 2023-03-20 18:35:30.000000 kfp-tekton-1.6.4/kfp_tekton/k8s_client_helper.py
--rw-r--r--   0 tommyli    (501) staff       (20)    17417 2023-03-20 18:35:30.000000 kfp-tekton-1.6.4/kfp_tekton/tekton.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-03-22 20:00:30.498929 kfp-tekton-1.6.4/kfp_tekton.egg-info/
--rw-r--r--   0 tommyli    (501) staff       (20)    11889 2023-03-22 20:00:30.000000 kfp-tekton-1.6.4/kfp_tekton.egg-info/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)      645 2023-03-22 20:00:30.000000 kfp-tekton-1.6.4/kfp_tekton.egg-info/SOURCES.txt
--rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-03-22 20:00:30.000000 kfp-tekton-1.6.4/kfp_tekton.egg-info/dependency_links.txt
--rw-r--r--   0 tommyli    (501) staff       (20)      107 2023-03-22 20:00:30.000000 kfp-tekton-1.6.4/kfp_tekton.egg-info/entry_points.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       49 2023-03-22 20:00:30.000000 kfp-tekton-1.6.4/kfp_tekton.egg-info/requires.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       11 2023-03-22 20:00:30.000000 kfp-tekton-1.6.4/kfp_tekton.egg-info/top_level.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       38 2023-03-22 20:00:30.508423 kfp-tekton-1.6.4/setup.cfg
--rw-r--r--   0 tommyli    (501) staff       (20)     7465 2023-03-22 19:58:35.000000 kfp-tekton-1.6.4/setup.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-04-11 19:49:28.868767 kfp-tekton-1.6.5/
+-rw-r--r--   0 tommyli    (501) staff       (20)    11889 2023-04-11 19:49:28.868376 kfp-tekton-1.6.5/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)    16444 2023-04-11 19:48:11.000000 kfp-tekton-1.6.5/README.md
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-04-11 19:49:28.856151 kfp-tekton-1.6.5/kfp_tekton/
+-rw-r--r--   0 tommyli    (501) staff       (20)      713 2023-04-11 19:48:11.000000 kfp-tekton-1.6.5/kfp_tekton/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    30584 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/_client.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-04-11 19:49:28.867515 kfp-tekton-1.6.5/kfp_tekton/compiler/
+-rw-r--r--   0 tommyli    (501) staff       (20)      675 2023-02-21 19:36:36.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    44521 2023-02-21 19:36:36.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/_data_passing_rewriter.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     7091 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/_k8s_helper.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    32108 2023-03-17 18:34:11.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/_op_to_template.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    30933 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/_tekton_handler.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    99548 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/compiler.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4279 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/main.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4088 2023-03-17 18:33:39.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/pipeline_utils.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2071 2023-02-21 19:36:36.000000 kfp-tekton-1.6.5/kfp_tekton/compiler/yaml_utils.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1311 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/k8s_client_helper.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    17417 2023-04-07 17:42:53.000000 kfp-tekton-1.6.5/kfp_tekton/tekton.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-04-11 19:49:28.858796 kfp-tekton-1.6.5/kfp_tekton.egg-info/
+-rw-r--r--   0 tommyli    (501) staff       (20)    11889 2023-04-11 19:49:28.000000 kfp-tekton-1.6.5/kfp_tekton.egg-info/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)      645 2023-04-11 19:49:28.000000 kfp-tekton-1.6.5/kfp_tekton.egg-info/SOURCES.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-04-11 19:49:28.000000 kfp-tekton-1.6.5/kfp_tekton.egg-info/dependency_links.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)      107 2023-04-11 19:49:28.000000 kfp-tekton-1.6.5/kfp_tekton.egg-info/entry_points.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       49 2023-04-11 19:49:28.000000 kfp-tekton-1.6.5/kfp_tekton.egg-info/requires.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       11 2023-04-11 19:49:28.000000 kfp-tekton-1.6.5/kfp_tekton.egg-info/top_level.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       38 2023-04-11 19:49:28.868882 kfp-tekton-1.6.5/setup.cfg
+-rw-r--r--   0 tommyli    (501) staff       (20)     7465 2023-04-11 19:48:11.000000 kfp-tekton-1.6.5/setup.py
```

### Comparing `kfp-tekton-1.6.4/PKG-INFO` & `kfp-tekton-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfp-tekton
-Version: 1.6.4
+Version: 1.6.5
 Summary: Tekton Compiler for Kubeflow Pipelines
 Home-page: https://github.com/kubeflow/kfp-tekton/
 Author: kubeflow.org
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -83,15 +83,15 @@
   * `kfp_tekton.TektonClient.create_run_from_pipeline_package` runs a local
     pipeline package on Kubeflow Pipelines.
 
 
 <h2><a id="project-prerequisites">Project Prerequisites</a></h2>
 
  - Python: `3.7` or later
- - Tekton: [`v0.44.0`](https://github.com/tektoncd/pipeline/releases/tag/v0.44.0) or [later](https://github.com/tektoncd/pipeline/releases/latest)
+ - Tekton: [`v0.44.2`](https://github.com/tektoncd/pipeline/releases/tag/v0.44.2) or [later](https://github.com/tektoncd/pipeline/releases/latest)
  - Tekton CLI: [`0.29.1`](https://github.com/tektoncd/cli/releases/tag/v0.29.1)
  - Kubeflow Pipelines: [KFP with Tekton backend](https://github.com/kubeflow/kfp-tekton/blob/master/guides/kfp_tekton_install.md)
 
 Follow the instructions for [installing project prerequisites](https://github.com/kubeflow/kfp-tekton/blob/master/sdk/python/README.md#development-prerequisites)
 and take note of some important caveats.
```

### Comparing `kfp-tekton-1.6.4/README.md` & `kfp-tekton-1.6.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,16 @@
 The source code of the `kfp-tekton` compiler was created as an extension of the [`Kubeflow Pipelines SDK Compiler`](https://github.com/kubeflow/pipelines/tree/sdk/release-1.8/sdk/python/kfp/compiler).
 This approach allowed us to leverage much of the existing [Kubeflow Pipelines Python SDK code](https://www.kubeflow.org/docs/pipelines/sdk/sdk-overview/#sdk-packages),
 like the DSL and components packages, but "override" or "replace" those parts of the compiler code required to generate
 the Tekton YAML instead of Argo YAML. Since the KFP SDK was not designed and implemented to easily be extended,
 _monkey-patching_ was used to replace non-class methods and functions at runtime.
 
 In order for the _monkey patch_ to work properly, the `kfp-tekton` compiler source code has to be aligned with a
-specific version of the `kfp` SDK compiler. As of now the `kfp-tekton` SDK version is `1.6.4` which is aligned with KFP
-SDK version [`1.8.19`](https://pypi.org/project/kfp/1.8.19/).
+specific version of the `kfp` SDK compiler. As of now the `kfp-tekton` SDK version is `1.6.5` which is aligned with KFP
+SDK version [`1.8.20`](https://pypi.org/project/kfp/1.8.20/).
 
 
 ## Adding New Code
 
 The Python package structure as well as the module names and method signatures closely mirror those of the
 [`Kubeflow Pipelines Python SDK`](https://github.com/kubeflow/pipelines/tree/master/sdk/python).
 This helps keeping track of all the code that had to modified and will make merging (some of) the code back into KFP or
```

### Comparing `kfp-tekton-1.6.4/kfp_tekton/__init__.py` & `kfp-tekton-1.6.5/kfp_tekton/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.6.4'
+__version__ = '1.6.5'
 
 from ._client import TektonClient  # noqa F401
 from .k8s_client_helper import env_from_secret  # noqa F401
```

### Comparing `kfp-tekton-1.6.4/kfp_tekton/_client.py` & `kfp-tekton-1.6.5/kfp_tekton/_client.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.4/kfp_tekton/compiler/__init__.py` & `kfp-tekton-1.6.5/kfp_tekton/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.4/kfp_tekton/compiler/_data_passing_rewriter.py` & `kfp-tekton-1.6.5/kfp_tekton/compiler/_data_passing_rewriter.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.4/kfp_tekton/compiler/_k8s_helper.py` & `kfp-tekton-1.6.5/kfp_tekton/compiler/_k8s_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.4/kfp_tekton/compiler/_op_to_template.py` & `kfp-tekton-1.6.5/kfp_tekton/compiler/_op_to_template.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.4/kfp_tekton/compiler/_tekton_handler.py` & `kfp-tekton-1.6.5/kfp_tekton/compiler/_tekton_handler.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.4/kfp_tekton/compiler/compiler.py` & `kfp-tekton-1.6.5/kfp_tekton/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.4/kfp_tekton/compiler/main.py` & `kfp-tekton-1.6.5/kfp_tekton/compiler/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import os
 import sys
 
 import kfp.compiler.main as kfp_compiler_main
 from kfp_tekton.compiler.pipeline_utils import TektonPipelineConf
 
 from . import TektonCompiler
-from .. import __version__
 
 
 def parse_arguments():
   """Parse command line arguments."""
 
   parser = argparse.ArgumentParser()
   parser.add_argument('--py',
@@ -82,15 +81,14 @@
     _compile_pipeline_function(pipeline_funcs, function_name, output_path, type_check, tekton_pipeline_conf)
   finally:
     del sys.path[0]
     sys.modules.pop(os.path.splitext(filename)[0])
 
 
 def main():
-    print(f"KFP-Tekton Compiler {__version__}")
     args = parse_arguments()
     if ((args.py is None and args.package is None) or
         (args.py is not None and args.package is not None)):
         raise ValueError('Either --py or --package is needed but not both.')
     if args.py:
         tekton_pipeline_conf = TektonPipelineConf()
         tekton_pipeline_conf.set_tekton_inline_spec(True)
```

### Comparing `kfp-tekton-1.6.4/kfp_tekton/compiler/pipeline_utils.py` & `kfp-tekton-1.6.5/kfp_tekton/compiler/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.4/kfp_tekton/compiler/yaml_utils.py` & `kfp-tekton-1.6.5/kfp_tekton/compiler/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.4/kfp_tekton/k8s_client_helper.py` & `kfp-tekton-1.6.5/kfp_tekton/k8s_client_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.4/kfp_tekton/tekton.py` & `kfp-tekton-1.6.5/kfp_tekton/tekton.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.4/kfp_tekton.egg-info/PKG-INFO` & `kfp-tekton-1.6.5/kfp_tekton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfp-tekton
-Version: 1.6.4
+Version: 1.6.5
 Summary: Tekton Compiler for Kubeflow Pipelines
 Home-page: https://github.com/kubeflow/kfp-tekton/
 Author: kubeflow.org
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -83,15 +83,15 @@
   * `kfp_tekton.TektonClient.create_run_from_pipeline_package` runs a local
     pipeline package on Kubeflow Pipelines.
 
 
 <h2><a id="project-prerequisites">Project Prerequisites</a></h2>
 
  - Python: `3.7` or later
- - Tekton: [`v0.44.0`](https://github.com/tektoncd/pipeline/releases/tag/v0.44.0) or [later](https://github.com/tektoncd/pipeline/releases/latest)
+ - Tekton: [`v0.44.2`](https://github.com/tektoncd/pipeline/releases/tag/v0.44.2) or [later](https://github.com/tektoncd/pipeline/releases/latest)
  - Tekton CLI: [`0.29.1`](https://github.com/tektoncd/cli/releases/tag/v0.29.1)
  - Kubeflow Pipelines: [KFP with Tekton backend](https://github.com/kubeflow/kfp-tekton/blob/master/guides/kfp_tekton_install.md)
 
 Follow the instructions for [installing project prerequisites](https://github.com/kubeflow/kfp-tekton/blob/master/sdk/python/README.md#development-prerequisites)
 and take note of some important caveats.
```

### Comparing `kfp-tekton-1.6.4/kfp_tekton.egg-info/SOURCES.txt` & `kfp-tekton-1.6.5/kfp_tekton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfp-tekton-1.6.4/setup.py` & `kfp-tekton-1.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 # =============================================================================
 # To install the kfp_tekton project run:
 #
 #    $ pip3 install -e .
 #
 # To create a distribution for PyPi run:
 #
-#    $ export KFP_TEKTON_VERSION=1.6.4-rc1
+#    $ export KFP_TEKTON_VERSION=1.6.5-rc1
 #    $ python3 setup.py sdist
 #    $ twine check dist/kfp-tekton-${KFP_TEKTON_VERSION/-rc/rc}.tar.gz
 #    $ twine upload --repository pypi dist/kfp-tekton-${KFP_TEKTON_VERSION/-rc/rc}.tar.gz
 #
 #   ... or:
 #
-#    $ make distribution KFP_TEKTON_VERSION=1.6.4-rc1
+#    $ make distribution KFP_TEKTON_VERSION=1.6.5-rc1
 #
 # =============================================================================
 
 import logging
 import re
 import sys
 
@@ -55,15 +55,15 @@
 logger = logging.getLogger("kfp_tekton/setup.py")
 logger.setLevel(logging.INFO)
 
 
 # NOTICE, after any updates to the following, ./requirements.in should be updated
 # accordingly.
 REQUIRES = [
-    "kfp>=1.8.10,<1.8.20",
+    "kfp>=1.8.10,<1.8.21",
     "kfp-tekton-server-api>=1.5.0"
 ]
 
 TESTS_REQUIRE = [
     'pytest',
 ]
```

