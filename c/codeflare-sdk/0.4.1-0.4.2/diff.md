# Comparing `tmp/codeflare_sdk-0.4.1.tar.gz` & `tmp/codeflare_sdk-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflare_sdk-0.4.1.tar", max compression
+gzip compressed data, was "codeflare_sdk-0.4.2.tar", max compression
```

## Comparing `codeflare_sdk-0.4.1.tar` & `codeflare_sdk-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2022-11-22 00:48:43.906021 codeflare_sdk-0.4.1/LICENSE
--rw-r--r--   0        0        0     1782 2023-02-03 16:34:59.124401 codeflare_sdk-0.4.1/README.md
--rw-r--r--   0        0        0      728 2023-04-03 21:01:14.229113 codeflare_sdk-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-16 18:31:44.974735 codeflare_sdk-0.4.1/src/codeflare_sdk/__init__.py
--rw-r--r--   0        0        0        0 2022-11-16 19:42:48.730723 codeflare_sdk-0.4.1/src/codeflare_sdk/cluster/__init__.py
--rw-r--r--   0        0        0     4436 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.1/src/codeflare_sdk/cluster/auth.py
--rw-r--r--   0        0        0    18105 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.1/src/codeflare_sdk/cluster/cluster.py
--rw-r--r--   0        0        0     1694 2023-03-06 15:15:54.772713 codeflare_sdk-0.4.1/src/codeflare_sdk/cluster/config.py
--rw-r--r--   0        0        0     2141 2023-03-06 15:15:54.772713 codeflare_sdk-0.4.1/src/codeflare_sdk/cluster/model.py
--rw-r--r--   0        0        0        0 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.1/src/codeflare_sdk/job/__init__.py
--rw-r--r--   0        0        0     6049 2023-03-31 20:32:17.530773 codeflare_sdk-0.4.1/src/codeflare_sdk/job/jobs.py
--rw-r--r--   0        0        0    10292 2022-11-16 18:31:44.978735 codeflare_sdk-0.4.1/src/codeflare_sdk/templates/aw-kuberay.yaml
--rw-r--r--   0        0        0     7781 2022-11-16 18:31:44.978735 codeflare_sdk-0.4.1/src/codeflare_sdk/templates/base-template.yaml
--rw-r--r--   0        0        0     9912 2022-11-16 18:31:44.978735 codeflare_sdk-0.4.1/src/codeflare_sdk/templates/new-template.yaml
--rw-r--r--   0        0        0        0 2022-11-16 19:42:58.205776 codeflare_sdk-0.4.1/src/codeflare_sdk/utils/__init__.py
--rwxr-xr-x   0        0        0    10830 2023-02-02 16:52:21.915294 codeflare_sdk-0.4.1/src/codeflare_sdk/utils/generate_yaml.py
--rw-r--r--   0        0        0     6778 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.1/src/codeflare_sdk/utils/pretty_print.py
--rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 codeflare_sdk-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-11-22 00:48:43.906021 codeflare_sdk-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1852 2023-04-11 19:26:34.779878 codeflare_sdk-0.4.2/README.md
+-rw-r--r--   0        0        0      728 2023-04-11 19:27:21.780203 codeflare_sdk-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-16 18:31:44.974735 codeflare_sdk-0.4.2/src/codeflare_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-16 19:42:48.730723 codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/__init__.py
+-rw-r--r--   0        0        0     4434 2023-04-11 19:26:34.787878 codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/auth.py
+-rw-r--r--   0        0        0    17834 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/cluster.py
+-rw-r--r--   0        0        0     1706 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/config.py
+-rw-r--r--   0        0        0     2141 2023-03-06 15:15:54.772713 codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/model.py
+-rw-r--r--   0        0        0        0 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.2/src/codeflare_sdk/job/__init__.py
+-rw-r--r--   0        0        0     6618 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.2/src/codeflare_sdk/job/jobs.py
+-rw-r--r--   0        0        0    10292 2022-11-16 18:31:44.978735 codeflare_sdk-0.4.2/src/codeflare_sdk/templates/aw-kuberay.yaml
+-rw-r--r--   0        0        0     7782 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.2/src/codeflare_sdk/templates/base-template.yaml
+-rw-r--r--   0        0        0     9910 2023-04-11 19:26:34.788878 codeflare_sdk-0.4.2/src/codeflare_sdk/templates/new-template.yaml
+-rw-r--r--   0        0        0        0 2022-11-16 19:42:58.205776 codeflare_sdk-0.4.2/src/codeflare_sdk/utils/__init__.py
+-rwxr-xr-x   0        0        0    10830 2023-02-02 16:52:21.915294 codeflare_sdk-0.4.2/src/codeflare_sdk/utils/generate_yaml.py
+-rw-r--r--   0        0        0     6778 2023-03-27 14:54:38.071640 codeflare_sdk-0.4.2/src/codeflare_sdk/utils/pretty_print.py
+-rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 codeflare_sdk-0.4.2/PKG-INFO
```

### Comparing `codeflare_sdk-0.4.1/LICENSE` & `codeflare_sdk-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.1/README.md` & `codeflare_sdk-0.4.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -11,30 +11,39 @@
 
 ## Installation
 
 Can be installed via `pip`: `pip install codeflare-sdk`
 
 ## Development
 
-For testing, make sure to have installed:
- - `pytest`, `pytest-mock` (can both be installed with `pip`)
- - The remaining dependencies located in `requirements.txt`
- - To run the unit tests, run `pytest -v tests/unit_test.py`)
- - Any new test functions/scripts can be added into the `tests` folder
-
-NOTE: Functional tests coming soon, will live in `tests/func_test.py`
-
-For checking code coverage while testing:
- - Start by installing `coverage` (can be done via `pip`)
- - Now instead when testing run `coverage run -m --source=src pytest tests/unit_test.py`
- - To then view a code coverage report w/ missing lines, run `coverage report -m`
-
-For formatting:
- - Currently using black v22.3.0 for format checking
- - To install, run `pip install black==22.3.0`
- - To check file formatting, in top-level dir run `black --check .`
-   - To auto-reformat all files, remove the `--check` flag
-   - To reformat an individual file, run `black <filename>`
-
-To build the python package:
- - If poetry is not installed: `pip install poetry`
- - `poetry build`
+### Prerequisites
+
+We recommend using Python 3.9 for development.
+Install development specific dependencies:
+  `$ pip install -r requirements-dev.txt`
+
+Additional dependencies can be found in `requirements.txt`: `$ pip install -r requirements.txt`
+
+### Pre-commit
+
+We use pre-commit to make sure the code is consistently formatted. To make sure that pre-commit is run every time you commit changes, simply run `pre-commit install`
+
+### Testing
+
+- To run the unit tests, run `pytest -v tests/unit_test.py`
+- Any new test functions/scripts can be added into the `tests` folder
+- NOTE: Functional tests coming soon, will live in `tests/func_test.py`
+
+#### Code Coverage
+
+- Run tests with the following command: `coverage run -m --source=src pytest tests/unit_test.py`
+- To then view a code coverage report w/ missing lines, run `coverage report -m`
+
+### Code Formatting
+
+- To check file formatting, in top-level dir run `black --check .`
+- To auto-reformat all files, remove the `--check` flag
+- To reformat an individual file, run `black <filename>`
+
+### Package Build
+
+To build the python package: `$ poetry build`
```

### Comparing `codeflare_sdk-0.4.1/pyproject.toml` & `codeflare_sdk-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codeflare-sdk"
-version = "0.4.1"
+version = "0.4.2"
 description = "Python SDK for codeflare client"
 
 license = "Apache-2.0"
 
 authors = [
     "Michael Clifford <mcliffor@redhat.com>",
     "Mustafa Eyceoz <meyceoz@redhat.com>",
@@ -21,8 +21,8 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 openshift-client = "1.0.18"
 rich = "^12.5"
 ray = {version = "2.1.0", extras = ["default"]}
 kubernetes = "26.1.0"
-codeflare-torchx = "0.5.0.dev5"
+codeflare-torchx = "0.6.0.dev0"
```

### Comparing `codeflare_sdk-0.4.1/src/codeflare_sdk/cluster/auth.py` & `codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 The auth sub-module contains the definitions for the Authentication objects, which represent
 the methods by which a user can authenticate to their cluster(s). The abstract class, `Authentication`,
 contains two required methods `login()` and `logout()`. Users can use one of the existing concrete classes to
-authenticate to their cluster or add their own custom concrete classes here.  
+authenticate to their cluster or add their own custom concrete classes here.
 """
 
 import abc
 import openshift as oc
 from openshift import OpenShiftPythonException
```

### Comparing `codeflare_sdk-0.4.1/src/codeflare_sdk/cluster/cluster.py` & `codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,22 @@
         self.app_wrapper_name = self.app_wrapper_yaml.split(".")[0]
 
     def create_app_wrapper(self):
         """
         Called upon cluster object creation, creates an AppWrapper yaml based on
         the specifications of the ClusterConfiguration.
         """
+
+        if self.config.namespace is None:
+            self.config.namespace = oc.get_project_name()
+            if type(self.config.namespace) is not str:
+                raise TypeError(
+                    f"Namespace {self.config.namespace} is of type {type(self.config.namespace)}. Check your Kubernetes Authentication."
+                )
+
         name = self.config.name
         namespace = self.config.namespace
         min_cpu = self.config.min_cpus
         max_cpu = self.config.max_cpus
         min_memory = self.config.min_memory
         max_memory = self.config.max_memory
         gpu = self.config.gpu
@@ -281,34 +289,14 @@
         if working_dir:
             to_return["working_dir"] = working_dir
         if requirements:
             to_return["requirements"] = requirements
         return to_return
 
 
-def get_current_namespace() -> str:
-    """
-    Returns the user's current working namespace.
-    """
-    try:
-        namespace = oc.invoke("project", ["-q"]).actions()[0].out.strip()
-    except oc.OpenShiftPythonException as osp:  # pragma: no cover
-        error_msg = osp.result.err()
-        if (
-            "do not have rights" in error_msg
-            or "Missing or incomplete configuration" in error_msg
-        ):
-            raise PermissionError(
-                "Action not permitted, have you run auth.login() or cluster.up()?"
-            )
-        else:
-            raise osp
-    return namespace
-
-
 def list_all_clusters(namespace: str, print_to_console: bool = True):
     """
     Returns (and prints by default) a list of all clusters in a given namespace.
     """
     clusters = _get_ray_clusters(namespace)
     if print_to_console:
         pretty_print.print_clusters(clusters)
```

### Comparing `codeflare_sdk-0.4.1/src/codeflare_sdk/cluster/config.py` & `codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,27 +17,28 @@
 which is used to specify resource requirements and other details when creating a
 Cluster object.
 """
 
 from dataclasses import dataclass, field
 from .auth import Authentication
 import pathlib
+import openshift
 
 dir = pathlib.Path(__file__).parent.parent.resolve()
 
 
 @dataclass
 class ClusterConfiguration:
     """
     This dataclass is used to specify resource requirements and other details, and
     is passed in as an argument when creating a Cluster object.
     """
 
     name: str
-    namespace: str = "default"
+    namespace: str = None
     head_info: list = field(default_factory=list)
     machine_types: list = field(default_factory=list)  # ["m4.xlarge", "g4dn.xlarge"]
     min_cpus: int = 1
     max_cpus: int = 1
     min_worker: int = 1
     max_worker: int = 1
     min_memory: int = 2
```

### Comparing `codeflare_sdk-0.4.1/src/codeflare_sdk/cluster/model.py` & `codeflare_sdk-0.4.2/src/codeflare_sdk/cluster/model.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.1/src/codeflare_sdk/job/jobs.py` & `codeflare_sdk-0.4.2/src/codeflare_sdk/job/jobs.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 
 import abc
 from typing import TYPE_CHECKING, Optional, Dict, List
 from pathlib import Path
 
+import openshift as oc
 from torchx.components.dist import ddp
 from torchx.runner import get_runner
 from torchx.specs import AppHandle, parse_app_handle, AppDryRunInfo
 
 if TYPE_CHECKING:
     from ..cluster.cluster import Cluster
 
@@ -56,16 +57,18 @@
         memMB: Optional[int] = None,
         h: Optional[str] = None,
         j: Optional[str] = None,
         env: Optional[Dict[str, str]] = None,
         max_retries: int = 0,
         mounts: Optional[List[str]] = None,
         rdzv_port: int = 29500,
+        rdzv_backend: str = None,
         scheduler_args: Optional[Dict[str, str]] = None,
         image: Optional[str] = None,
+        workspace: Optional[str] = f"file://{Path.cwd()}",
     ):
         if bool(script) == bool(m):  # logical XOR
             raise ValueError(
                 "Exactly one of the following arguments must be defined: [script, m]."
             )
         self.script = script
         self.m = m
@@ -76,18 +79,20 @@
         self.memMB = memMB
         self.h = h
         self.j = j
         self.env: Dict[str, str] = env if env is not None else dict()
         self.max_retries = max_retries
         self.mounts: List[str] = mounts if mounts is not None else []
         self.rdzv_port = rdzv_port
+        self.rdzv_backend = rdzv_backend
         self.scheduler_args: Dict[str, str] = (
             scheduler_args if scheduler_args is not None else dict()
         )
         self.image = image
+        self.workspace = workspace
 
     def _dry_run(self, cluster: "Cluster"):
         j = f"{cluster.config.max_worker}x{max(cluster.config.gpu, 1)}"  # # of proc. = # of gpus
         return torchx_runner.dryrun(
             app=ddp(
                 *self.script_args,
                 script=self.script,
@@ -99,25 +104,31 @@
                 memMB=self.memMB
                 if self.memMB is not None
                 else cluster.config.max_memory * 1024,
                 j=self.j if self.j is not None else j,
                 env=self.env,
                 max_retries=self.max_retries,
                 rdzv_port=self.rdzv_port,
+                rdzv_backend=self.rdzv_backend
+                if self.rdzv_backend is not None
+                else "static",
                 mounts=self.mounts,
             ),
             scheduler=cluster.torchx_scheduler,
             cfg=cluster.torchx_config(**self.scheduler_args),
-            workspace=f"file://{Path.cwd()}",
+            workspace=self.workspace,
         )
 
     def _missing_spec(self, spec: str):
         raise ValueError(f"Job definition missing arg: {spec}")
 
     def _dry_run_no_cluster(self):
+        if self.scheduler_args is not None:
+            if self.scheduler_args.get("namespace") is None:
+                self.scheduler_args["namespace"] = oc.get_project_name()
         return torchx_runner.dryrun(
             app=ddp(
                 *self.script_args,
                 script=self.script,
                 m=self.m,
                 name=self.name if self.name is not None else self._missing_spec("name"),
                 h=self.h,
@@ -134,21 +145,24 @@
                 if self.j is not None
                 else self._missing_spec(
                     "j (`workers`x`procs`)"
                 ),  # # of proc. = # of gpus,
                 env=self.env,  # should this still exist?
                 max_retries=self.max_retries,
                 rdzv_port=self.rdzv_port,  # should this still exist?
+                rdzv_backend=self.rdzv_backend
+                if self.rdzv_backend is not None
+                else "c10d",
                 mounts=self.mounts,
                 image=self.image
                 if self.image is not None
                 else self._missing_spec("image"),
             ),
             scheduler="kubernetes_mcad",
-            cfg=self.scheduler_args if self.scheduler_args is not None else None,
+            cfg=self.scheduler_args,
             workspace="",
         )
 
     def submit(self, cluster: "Cluster" = None) -> "Job":
         return DDPJob(self, cluster)
```

### Comparing `codeflare_sdk-0.4.1/src/codeflare_sdk/templates/aw-kuberay.yaml` & `codeflare_sdk-0.4.2/src/codeflare_sdk/templates/aw-kuberay.yaml`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.1/src/codeflare_sdk/templates/base-template.yaml` & `codeflare_sdk-0.4.2/src/codeflare_sdk/templates/base-template.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -149,8 +149,8 @@
                         command: ["/bin/sh","-c","ray stop"]
                   resources:
                     limits:
                       cpu: "1"
                       memory: "512Mi"
                     requests:
                       cpu: "500m"
-                      memory: "256Mi"
+                      memory: "256Mi"
```

### Comparing `codeflare_sdk-0.4.1/src/codeflare_sdk/templates/new-template.yaml` & `codeflare_sdk-0.4.2/src/codeflare_sdk/templates/new-template.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
                 containers:
                 - name: machine-learning # must consist of lower case alphanumeric characters or '-', and must start and end with an alphanumeric character (e.g. 'my-name',  or '123-abc'
                   image: rayproject/ray:latest
                   env:
                   - name: MY_POD_IP
                     valueFrom:
                       fieldRef:
-                        fieldPath: status.podIP 
+                        fieldPath: status.podIP
                   # environment variables to set in the container.Optional.
                   # Refer to https://kubernetes.io/docs/tasks/inject-data-application/define-environment-variable-container/
                   lifecycle:
                     preStop:
                       exec:
                         command: ["/bin/sh","-c","ray stop"]
                   resources:
@@ -216,8 +216,8 @@
             # allows me to return name of service that Ray operator creates
             odh-ray-cluster-service: deployment-name-head-svc
         spec:
           to:
             kind: Service
             name: deployment-name-head-svc
           port:
-            targetPort: dashboard 
+            targetPort: dashboard
```

### Comparing `codeflare_sdk-0.4.1/src/codeflare_sdk/utils/generate_yaml.py` & `codeflare_sdk-0.4.2/src/codeflare_sdk/utils/generate_yaml.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.1/src/codeflare_sdk/utils/pretty_print.py` & `codeflare_sdk-0.4.2/src/codeflare_sdk/utils/pretty_print.py`

 * *Files identical despite different names*

### Comparing `codeflare_sdk-0.4.1/PKG-INFO` & `codeflare_sdk-0.4.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: codeflare-sdk
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python SDK for codeflare client
 Home-page: https://github.com/project-codeflare/codeflare-sdk
 License: Apache-2.0
 Keywords: codeflare,python,sdk,client,batch,scale
 Author: Michael Clifford
 Author-email: mcliffor@redhat.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: codeflare-torchx (==0.5.0.dev5)
+Requires-Dist: codeflare-torchx (==0.6.0.dev0)
 Requires-Dist: kubernetes (==26.1.0)
 Requires-Dist: openshift-client (==1.0.18)
 Requires-Dist: ray[default] (==2.1.0)
 Requires-Dist: rich (>=12.5,<13.0)
 Project-URL: Repository, https://github.com/project-codeflare/codeflare-sdk
 Description-Content-Type: text/markdown
 
@@ -36,31 +36,40 @@
 
 ## Installation
 
 Can be installed via `pip`: `pip install codeflare-sdk`
 
 ## Development
 
-For testing, make sure to have installed:
- - `pytest`, `pytest-mock` (can both be installed with `pip`)
- - The remaining dependencies located in `requirements.txt`
- - To run the unit tests, run `pytest -v tests/unit_test.py`)
- - Any new test functions/scripts can be added into the `tests` folder
-
-NOTE: Functional tests coming soon, will live in `tests/func_test.py`
-
-For checking code coverage while testing:
- - Start by installing `coverage` (can be done via `pip`)
- - Now instead when testing run `coverage run -m --source=src pytest tests/unit_test.py`
- - To then view a code coverage report w/ missing lines, run `coverage report -m`
-
-For formatting:
- - Currently using black v22.3.0 for format checking
- - To install, run `pip install black==22.3.0`
- - To check file formatting, in top-level dir run `black --check .`
-   - To auto-reformat all files, remove the `--check` flag
-   - To reformat an individual file, run `black <filename>`
-
-To build the python package:
- - If poetry is not installed: `pip install poetry`
- - `poetry build`
+### Prerequisites
+
+We recommend using Python 3.9 for development.
+Install development specific dependencies:
+  `$ pip install -r requirements-dev.txt`
+
+Additional dependencies can be found in `requirements.txt`: `$ pip install -r requirements.txt`
+
+### Pre-commit
+
+We use pre-commit to make sure the code is consistently formatted. To make sure that pre-commit is run every time you commit changes, simply run `pre-commit install`
+
+### Testing
+
+- To run the unit tests, run `pytest -v tests/unit_test.py`
+- Any new test functions/scripts can be added into the `tests` folder
+- NOTE: Functional tests coming soon, will live in `tests/func_test.py`
+
+#### Code Coverage
+
+- Run tests with the following command: `coverage run -m --source=src pytest tests/unit_test.py`
+- To then view a code coverage report w/ missing lines, run `coverage report -m`
+
+### Code Formatting
+
+- To check file formatting, in top-level dir run `black --check .`
+- To auto-reformat all files, remove the `--check` flag
+- To reformat an individual file, run `black <filename>`
+
+### Package Build
+
+To build the python package: `$ poetry build`
```

