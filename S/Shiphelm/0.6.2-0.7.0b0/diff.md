# Comparing `tmp/Shiphelm-0.6.2.tar.gz` & `tmp/Shiphelm-0.7.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shiphelm-0.6.2.tar", last modified: Sat Apr  8 04:15:51 2023, max compression
+gzip compressed data, was "Shiphelm-0.7.0b0.tar", last modified: Tue Apr 11 18:37:00 2023, max compression
```

## Comparing `Shiphelm-0.6.2.tar` & `Shiphelm-0.7.0b0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:15:51.872591 Shiphelm-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-08 04:15:42.000000 Shiphelm-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-08 04:15:42.000000 Shiphelm-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-08 04:15:51.872591 Shiphelm-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-08 04:15:42.000000 Shiphelm-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-08 04:15:42.000000 Shiphelm-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-08 04:15:51.872591 Shiphelm-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-08 04:15:42.000000 Shiphelm-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:15:51.872591 Shiphelm-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:15:51.872591 Shiphelm-0.6.2/src/Shiphelm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-08 04:15:51.000000 Shiphelm-0.6.2/src/Shiphelm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-08 04:15:51.000000 Shiphelm-0.6.2/src/Shiphelm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 04:15:51.000000 Shiphelm-0.6.2/src/Shiphelm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-08 04:15:51.000000 Shiphelm-0.6.2/src/Shiphelm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-08 04:15:51.000000 Shiphelm-0.6.2/src/Shiphelm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:15:51.872591 Shiphelm-0.6.2/src/shiphelm/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-08 04:15:42.000000 Shiphelm-0.6.2/src/shiphelm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-04-08 04:15:42.000000 Shiphelm-0.6.2/src/shiphelm/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-08 04:15:42.000000 Shiphelm-0.6.2/src/shiphelm/helmdocker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-04-08 04:15:42.000000 Shiphelm-0.6.2/src/shiphelm/helmkube.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-08 04:15:42.000000 Shiphelm-0.6.2/src/shiphelm/helmtest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 04:15:51.872591 Shiphelm-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-08 04:15:42.000000 Shiphelm-0.6.2/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:37:00.974612 Shiphelm-0.7.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 18:36:49.000000 Shiphelm-0.7.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-11 18:36:49.000000 Shiphelm-0.7.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-11 18:37:00.974612 Shiphelm-0.7.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-11 18:36:49.000000 Shiphelm-0.7.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 18:36:49.000000 Shiphelm-0.7.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 18:37:00.974612 Shiphelm-0.7.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-11 18:36:49.000000 Shiphelm-0.7.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:37:00.974612 Shiphelm-0.7.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:37:00.974612 Shiphelm-0.7.0b0/src/Shiphelm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-11 18:37:00.000000 Shiphelm-0.7.0b0/src/Shiphelm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-11 18:37:00.000000 Shiphelm-0.7.0b0/src/Shiphelm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:37:00.000000 Shiphelm-0.7.0b0/src/Shiphelm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-11 18:37:00.000000 Shiphelm-0.7.0b0/src/Shiphelm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 18:37:00.000000 Shiphelm-0.7.0b0/src/Shiphelm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:37:00.974612 Shiphelm-0.7.0b0/src/shiphelm/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 18:36:49.000000 Shiphelm-0.7.0b0/src/shiphelm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-11 18:36:49.000000 Shiphelm-0.7.0b0/src/shiphelm/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-11 18:36:49.000000 Shiphelm-0.7.0b0/src/shiphelm/helmdocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-04-11 18:36:49.000000 Shiphelm-0.7.0b0/src/shiphelm/helmkube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-11 18:36:49.000000 Shiphelm-0.7.0b0/src/shiphelm/helmtest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:37:00.974612 Shiphelm-0.7.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-11 18:36:49.000000 Shiphelm-0.7.0b0/tests/test_module1.py
```

### Comparing `Shiphelm-0.6.2/LICENSE` & `Shiphelm-0.7.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.6.2/PKG-INFO` & `Shiphelm-0.7.0b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shiphelm
-Version: 0.6.2
+Version: 0.7.0b0
 Summary: Docker and kubernetes integration library
 Home-page: https://github.com/gameplex-software/shiphelm
 Author: Gameplex Software
 Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,pypi,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,15 @@
 Shiphelm is a Python library for interacting with containers more easily. With Shiphelm, you can:
 
 - Get a list of all running containers
 - Get usage statistics and used ports for a given container by ID
 - Search containers by name or ID
 - Change the open ports of a container
 - Run new containers
-- Work with Docker, Kubernetes
+- Work with Docker, Docker-Swarm, and Kubernetes
 - Use Kubernetes clusters and Docker Swarm
 
 ## Installation
 
 You can install Shiphelm using pip:
 
 ```
@@ -47,27 +47,27 @@
 ```
 PyPI: [https://pypi.org/project/Shiphelm/]()
 
 GitHub Releases [https://github.com/Gameplex-Software/ShipHelm/releases]()
 
 ## Docker usage
 
-This code will allow you to manage the local docker daemon
+This code will allow you to manage the local container engine
 
 ```
-from shiphelm.helmdocker import helmdocker
+from shiphelm.helm import helm
 
-hd = helmdocker() # create an instance of helmdocker
+hd = helm.helm() # create an instance of helm
 ```
 
-This code will allow you to manage any remote docker daemon
+This code will allow you to manage any compatible remote container engine
 ```
-from shiphelm.helmdocker import helmdocker
+from shiphelm.helm import helm
 
-hd = helmdocker('tcp://remote-docker-host:2375') # create an instance of helmdocker for romote management
+hd = helm.reomte_connect('tcp://remote-docker-host:2375') # create an instance of helmdocker for romote management
 ```
 
 ### Get a List of Running Containers
 
 ```
 running_containers = hd.get_running_containers()
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Shiphelm Version: 0.6.2 Summary: Docker and
+Metadata-Version: 2.1 Name: Shiphelm Version: 0.7.0b0 Summary: Docker and
 kubernetes integration library Home-page: https://github.com/gameplex-software/
 shiphelm Author: Gameplex Software Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,pypi,package Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
@@ -12,22 +12,22 @@
 LICENSE
  [https://user-images.githubusercontent.com/34868944/223447636-3e17dee3-ccdf-
                           44cc-8d42-91378ced6708.png]
 # Shiphelm Shiphelm is a Python library for interacting with containers more
 easily. With Shiphelm, you can: - Get a list of all running containers - Get
 usage statistics and used ports for a given container by ID - Search containers
 by name or ID - Change the open ports of a container - Run new containers -
-Work with Docker, Kubernetes - Use Kubernetes clusters and Docker Swarm ##
-Installation You can install Shiphelm using pip: ``` pip install shiphelm ```
-PyPI: [https://pypi.org/project/Shiphelm/]() GitHub Releases [https://
-github.com/Gameplex-Software/ShipHelm/releases]() ## Docker usage This code
-will allow you to manage the local docker daemon ``` from shiphelm.helmdocker
-import helmdocker hd = helmdocker() # create an instance of helmdocker ``` This
-code will allow you to manage any remote docker daemon ``` from
-shiphelm.helmdocker import helmdocker hd = helmdocker('tcp://remote-docker-
+Work with Docker, Docker-Swarm, and Kubernetes - Use Kubernetes clusters and
+Docker Swarm ## Installation You can install Shiphelm using pip: ``` pip
+install shiphelm ``` PyPI: [https://pypi.org/project/Shiphelm/]() GitHub
+Releases [https://github.com/Gameplex-Software/ShipHelm/releases]() ## Docker
+usage This code will allow you to manage the local container engine ``` from
+shiphelm.helm import helm hd = helm.helm() # create an instance of helm ```
+This code will allow you to manage any compatible remote container engine ```
+from shiphelm.helm import helm hd = helm.reomte_connect('tcp://remote-docker-
 host:2375') # create an instance of helmdocker for romote management ``` ###
 Get a List of Running Containers ``` running_containers =
 hd.get_running_containers() ``` ### Get Stats and Ports for a Container by ID
 ``` container_stats = hd.get_container_stats(container_id) container_ports =
 hd.get_container_ports(container_id) ``` ### Search for Containers by Name ```
 containers_by_name = hd.search_containers(name) ``` ### Change the Ports of a
 Container ``` hd.change_container_ports(container_id, ports) ``` ### Rename a
```

### Comparing `Shiphelm-0.6.2/README.md` & `Shiphelm-0.7.0b0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Shiphelm is a Python library for interacting with containers more easily. With Shiphelm, you can:
 
 - Get a list of all running containers
 - Get usage statistics and used ports for a given container by ID
 - Search containers by name or ID
 - Change the open ports of a container
 - Run new containers
-- Work with Docker, Kubernetes
+- Work with Docker, Docker-Swarm, and Kubernetes
 - Use Kubernetes clusters and Docker Swarm
 
 ## Installation
 
 You can install Shiphelm using pip:
 
 ```
@@ -25,27 +25,27 @@
 ```
 PyPI: [https://pypi.org/project/Shiphelm/]()
 
 GitHub Releases [https://github.com/Gameplex-Software/ShipHelm/releases]()
 
 ## Docker usage
 
-This code will allow you to manage the local docker daemon
+This code will allow you to manage the local container engine
 
 ```
-from shiphelm.helmdocker import helmdocker
+from shiphelm.helm import helm
 
-hd = helmdocker() # create an instance of helmdocker
+hd = helm.helm() # create an instance of helm
 ```
 
-This code will allow you to manage any remote docker daemon
+This code will allow you to manage any compatible remote container engine
 ```
-from shiphelm.helmdocker import helmdocker
+from shiphelm.helm import helm
 
-hd = helmdocker('tcp://remote-docker-host:2375') # create an instance of helmdocker for romote management
+hd = helm.reomte_connect('tcp://remote-docker-host:2375') # create an instance of helmdocker for romote management
 ```
 
 ### Get a List of Running Containers
 
 ```
 running_containers = hd.get_running_containers()
 ```
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
  [https://user-images.githubusercontent.com/34868944/223447636-3e17dee3-ccdf-
                           44cc-8d42-91378ced6708.png]
 # Shiphelm Shiphelm is a Python library for interacting with containers more
 easily. With Shiphelm, you can: - Get a list of all running containers - Get
 usage statistics and used ports for a given container by ID - Search containers
 by name or ID - Change the open ports of a container - Run new containers -
-Work with Docker, Kubernetes - Use Kubernetes clusters and Docker Swarm ##
-Installation You can install Shiphelm using pip: ``` pip install shiphelm ```
-PyPI: [https://pypi.org/project/Shiphelm/]() GitHub Releases [https://
-github.com/Gameplex-Software/ShipHelm/releases]() ## Docker usage This code
-will allow you to manage the local docker daemon ``` from shiphelm.helmdocker
-import helmdocker hd = helmdocker() # create an instance of helmdocker ``` This
-code will allow you to manage any remote docker daemon ``` from
-shiphelm.helmdocker import helmdocker hd = helmdocker('tcp://remote-docker-
+Work with Docker, Docker-Swarm, and Kubernetes - Use Kubernetes clusters and
+Docker Swarm ## Installation You can install Shiphelm using pip: ``` pip
+install shiphelm ``` PyPI: [https://pypi.org/project/Shiphelm/]() GitHub
+Releases [https://github.com/Gameplex-Software/ShipHelm/releases]() ## Docker
+usage This code will allow you to manage the local container engine ``` from
+shiphelm.helm import helm hd = helm.helm() # create an instance of helm ```
+This code will allow you to manage any compatible remote container engine ```
+from shiphelm.helm import helm hd = helm.reomte_connect('tcp://remote-docker-
 host:2375') # create an instance of helmdocker for romote management ``` ###
 Get a List of Running Containers ``` running_containers =
 hd.get_running_containers() ``` ### Get Stats and Ports for a Container by ID
 ``` container_stats = hd.get_container_stats(container_id) container_ports =
 hd.get_container_ports(container_id) ``` ### Search for Containers by Name ```
 containers_by_name = hd.search_containers(name) ``` ### Change the Ports of a
 Container ``` hd.change_container_ports(container_id, ports) ``` ### Rename a
```

### Comparing `Shiphelm-0.6.2/setup.py` & `Shiphelm-0.7.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.6.2/src/Shiphelm.egg-info/PKG-INFO` & `Shiphelm-0.7.0b0/src/Shiphelm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shiphelm
-Version: 0.6.2
+Version: 0.7.0b0
 Summary: Docker and kubernetes integration library
 Home-page: https://github.com/gameplex-software/shiphelm
 Author: Gameplex Software
 Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,pypi,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,15 @@
 Shiphelm is a Python library for interacting with containers more easily. With Shiphelm, you can:
 
 - Get a list of all running containers
 - Get usage statistics and used ports for a given container by ID
 - Search containers by name or ID
 - Change the open ports of a container
 - Run new containers
-- Work with Docker, Kubernetes
+- Work with Docker, Docker-Swarm, and Kubernetes
 - Use Kubernetes clusters and Docker Swarm
 
 ## Installation
 
 You can install Shiphelm using pip:
 
 ```
@@ -47,27 +47,27 @@
 ```
 PyPI: [https://pypi.org/project/Shiphelm/]()
 
 GitHub Releases [https://github.com/Gameplex-Software/ShipHelm/releases]()
 
 ## Docker usage
 
-This code will allow you to manage the local docker daemon
+This code will allow you to manage the local container engine
 
 ```
-from shiphelm.helmdocker import helmdocker
+from shiphelm.helm import helm
 
-hd = helmdocker() # create an instance of helmdocker
+hd = helm.helm() # create an instance of helm
 ```
 
-This code will allow you to manage any remote docker daemon
+This code will allow you to manage any compatible remote container engine
 ```
-from shiphelm.helmdocker import helmdocker
+from shiphelm.helm import helm
 
-hd = helmdocker('tcp://remote-docker-host:2375') # create an instance of helmdocker for romote management
+hd = helm.reomte_connect('tcp://remote-docker-host:2375') # create an instance of helmdocker for romote management
 ```
 
 ### Get a List of Running Containers
 
 ```
 running_containers = hd.get_running_containers()
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Shiphelm Version: 0.6.2 Summary: Docker and
+Metadata-Version: 2.1 Name: Shiphelm Version: 0.7.0b0 Summary: Docker and
 kubernetes integration library Home-page: https://github.com/gameplex-software/
 shiphelm Author: Gameplex Software Author-email: info@gameplexsoftware.com
 Keywords: SkiffUI,pypi,package Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
@@ -12,22 +12,22 @@
 LICENSE
  [https://user-images.githubusercontent.com/34868944/223447636-3e17dee3-ccdf-
                           44cc-8d42-91378ced6708.png]
 # Shiphelm Shiphelm is a Python library for interacting with containers more
 easily. With Shiphelm, you can: - Get a list of all running containers - Get
 usage statistics and used ports for a given container by ID - Search containers
 by name or ID - Change the open ports of a container - Run new containers -
-Work with Docker, Kubernetes - Use Kubernetes clusters and Docker Swarm ##
-Installation You can install Shiphelm using pip: ``` pip install shiphelm ```
-PyPI: [https://pypi.org/project/Shiphelm/]() GitHub Releases [https://
-github.com/Gameplex-Software/ShipHelm/releases]() ## Docker usage This code
-will allow you to manage the local docker daemon ``` from shiphelm.helmdocker
-import helmdocker hd = helmdocker() # create an instance of helmdocker ``` This
-code will allow you to manage any remote docker daemon ``` from
-shiphelm.helmdocker import helmdocker hd = helmdocker('tcp://remote-docker-
+Work with Docker, Docker-Swarm, and Kubernetes - Use Kubernetes clusters and
+Docker Swarm ## Installation You can install Shiphelm using pip: ``` pip
+install shiphelm ``` PyPI: [https://pypi.org/project/Shiphelm/]() GitHub
+Releases [https://github.com/Gameplex-Software/ShipHelm/releases]() ## Docker
+usage This code will allow you to manage the local container engine ``` from
+shiphelm.helm import helm hd = helm.helm() # create an instance of helm ```
+This code will allow you to manage any compatible remote container engine ```
+from shiphelm.helm import helm hd = helm.reomte_connect('tcp://remote-docker-
 host:2375') # create an instance of helmdocker for romote management ``` ###
 Get a List of Running Containers ``` running_containers =
 hd.get_running_containers() ``` ### Get Stats and Ports for a Container by ID
 ``` container_stats = hd.get_container_stats(container_id) container_ports =
 hd.get_container_ports(container_id) ``` ### Search for Containers by Name ```
 containers_by_name = hd.search_containers(name) ``` ### Change the Ports of a
 Container ``` hd.change_container_ports(container_id, ports) ``` ### Rename a
```

### Comparing `Shiphelm-0.6.2/src/shiphelm/helm.py` & `Shiphelm-0.7.0b0/src/shiphelm/helm.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,59 +10,59 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ----------------------------------------------------------------------------
 
-try:
-    from . import helmdocker, helmkube
-except:
-    print("Error: Shiphelm cannot be run from source!")
-    exit()
+import helmdocker, helmkube
 from kubernetes import client
 from typing import TYPE_CHECKING
 import docker
+import tkinter as tk
+from tkinter import ttk
 
 #Fix name conflict between docker nad kubernetes client
 kubeclient = client
 
 #Fix editor auto completes that are broken by the dynamic functions
 if TYPE_CHECKING:
     from . import helmdocker, helmkube
     from helmdocker import helmdocker
     from helmdocker import *
     from helmkube import helmkube
     from helmkube import *
 
 class helm:
-    def __init__():
+    def __init__(self, engine=None):
         helm.engine = helm.set_engine_auto()
         helm.get_helm_client()
 
     def set_engine_auto():
         helm.engine = None
         try:
             v1 = kubeclient.CoreV1Api()
+            api = v1.CoreV1Api()
             helm.engine = "kubernetes"
-            v1.list_pod_for_all_namespaces(watch = False)
+            namespaces = api.list_namespace().items
             print("Found Kubernetes engine on local system using Kubernetes container engine")
         except:
+            pass
+        if not helm.engine:
             try:
                 docker.from_env()
-                print("Found Docker engine on local system using Kubernetes container engine")
+                print("Found Docker engine on local system using Docker container engine")
                 helm.engine = "docker"
             except:
-                pass
-
-        if not helm.engine:
-            print("[Error] Could not locate kubernetes or docker locally, this could be due to the current user permissions or an incompatible engine.")
+                print("[Debug] No compatible engine found, prompting for remote connection")
+                helm.remote_popup()
+                print("Popup got engine data:", helm.engineAddress, helm.engineType)
 
         return helm.engine
-
+    
     def set_engine_manual(engine_select):
         helm.engine = None
         if engine_select == "docker":
             try:
                 docker.from_env()
                 helm.engine = "docker"
             except Exception as e:
@@ -74,22 +74,48 @@
             except Exception as e:
                 print("Error connecting to Kubernetes daemon this could be due to the current user permissions or an incompatible engine. The error is as follows:", e)
         else:
             print("Invalid engine", engine_select, ". Supported options are 'docker' or 'kubernetes'")
 
         return helm.engine
     
+    def remote_popup():
+        # Create a popup window
+        window = tk.Tk()
+        window.title("Remote Address")
+
+        # Create a label and text input field for the remote address
+        tk.Label(window, text="Remote Address:").grid(row=0, column=0)
+        remote_address = tk.Entry(window)
+        remote_address.grid(row=0, column=1)
+
+        # Create a label and dropdown menu for the options
+        tk.Label(window, text="Options:").grid(row=1, column=0)
+        options = ttk.Combobox(window, values=["Option 1", "Option 2", "Option 3"])
+        options.current(0)
+        options.grid(row=1, column=1)
+
+        # Add a button to submit the inputs
+        submit_button = tk.Button(window, text="Submit")
+        submit_button.grid(row=2, column=1)
+
+        # Return values
+        helm.engineAddress = remote_address
+        helm.engineType = options.get()
+
+        # Start the event loop
+        window.mainloop()
+
     def add_methods(cls):
         methods = [m for m in dir(cls) if not m.startswith("__") and callable(getattr(cls, m))]
-        print(methods)
 
         for method in methods:
             setattr(helm, method, getattr(cls, method))
 
     def get_helm_client():
         print("Selected engine for runner:", helm.engine)
         if helm.engine == "docker":
             helm.add_methods(helmdocker.helmdocker)
             return helmdocker.helmdocker()
         elif helm.engine == "kubernetes":
             helm.add_methods(helmkube.helmkube)
-            return helmkube.helmkube()
+            return helmkube.helmkube()
```

### Comparing `Shiphelm-0.6.2/src/shiphelm/helmdocker.py` & `Shiphelm-0.7.0b0/src/shiphelm/helmdocker.py`

 * *Files identical despite different names*

### Comparing `Shiphelm-0.6.2/src/shiphelm/helmkube.py` & `Shiphelm-0.7.0b0/src/shiphelm/helmkube.py`

 * *Files identical despite different names*

