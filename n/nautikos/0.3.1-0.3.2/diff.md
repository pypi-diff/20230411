# Comparing `tmp/nautikos-0.3.1.tar.gz` & `tmp/nautikos-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautikos-0.3.1.tar", max compression
+gzip compressed data, was "nautikos-0.3.2.tar", max compression
```

## Comparing `nautikos-0.3.1.tar` & `nautikos-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-03-21 07:42:17.427920 nautikos-0.3.1/nautikos/__init__.py
--rw-r--r--   0        0        0     1333 2023-04-11 15:12:06.664571 nautikos-0.3.1/nautikos/cli.py
--rw-r--r--   0        0        0     4171 2023-04-11 15:12:06.789634 nautikos-0.3.1/nautikos/manifests.py
--rw-r--r--   0        0        0     3214 2023-04-11 14:40:08.893216 nautikos-0.3.1/nautikos/nautikos.py
--rw-r--r--   0        0        0       80 2023-03-24 10:25:48.952431 nautikos-0.3.1/nautikos/yaml.py
--rw-r--r--   0        0        0      952 2023-04-11 15:11:24.851096 nautikos-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3730 2023-04-11 08:03:55.985291 nautikos-0.3.1/README.md
--rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 nautikos-0.3.1/setup.py
--rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 nautikos-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-21 07:42:17.427920 nautikos-0.3.2/nautikos/__init__.py
+-rw-r--r--   0        0        0     1333 2023-04-11 15:12:06.664571 nautikos-0.3.2/nautikos/cli.py
+-rw-r--r--   0        0        0     4171 2023-04-11 15:12:06.789634 nautikos-0.3.2/nautikos/manifests.py
+-rw-r--r--   0        0        0     3214 2023-04-11 14:40:08.893216 nautikos-0.3.2/nautikos/nautikos.py
+-rw-r--r--   0        0        0       80 2023-03-24 10:25:48.952431 nautikos-0.3.2/nautikos/yaml.py
+-rw-r--r--   0        0        0     1291 2023-04-11 15:22:48.004820 nautikos-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3730 2023-04-11 08:03:55.985291 nautikos-0.3.2/README.md
+-rw-r--r--   0        0        0     4563 1970-01-01 00:00:00.000000 nautikos-0.3.2/setup.py
+-rw-r--r--   0        0        0     4481 1970-01-01 00:00:00.000000 nautikos-0.3.2/PKG-INFO
```

### Comparing `nautikos-0.3.1/nautikos/cli.py` & `nautikos-0.3.2/nautikos/cli.py`

 * *Files identical despite different names*

### Comparing `nautikos-0.3.1/nautikos/manifests.py` & `nautikos-0.3.2/nautikos/manifests.py`

 * *Files identical despite different names*

### Comparing `nautikos-0.3.1/nautikos/nautikos.py` & `nautikos-0.3.2/nautikos/nautikos.py`

 * *Files identical despite different names*

### Comparing `nautikos-0.3.1/pyproject.toml` & `nautikos-0.3.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 [tool.poetry]
 name = "nautikos"
-version = "0.3.1"
+version = "0.3.2"
 description = "A CD tool for updating image tags in Kubernetes manifests"
 authors = ["Jan Hein de Jong <janhein.dejong@gmail.com>"]
 readme = "README.md"
+license = "MIT"
+homepage = "https://www.github.com/janheindejong/nautikos"
+keywords = ["kubernetes", "devops", "cicd", "kustomize", "gitops"]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Topic :: Software Development",
+    "Topic :: Software Development :: Build Tools", 
+    "Operating System :: OS Independent"
+]
 
 [tool.poetry.scripts]
 nautikos = "nautikos.cli:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = "^0.7.0"
```

### Comparing `nautikos-0.3.1/README.md` & `nautikos-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nautikos-0.3.1/setup.py` & `nautikos-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 ['ruamel-yaml>=0.17.21,<0.18.0', 'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['nautikos = nautikos.cli:app']}
 
 setup_kwargs = {
     'name': 'nautikos',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'A CD tool for updating image tags in Kubernetes manifests',
     'long_description': "# Nautikos \n\n*A lightweight CI/CD tool for updating image tags in Kubernetes manifests.* \n\n[![PyPI version](https://badge.fury.io/py/nautikos.svg)](https://badge.fury.io/py/nautikos)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Python versions](https://img.shields.io/pypi/pyversions/nautikos)]()\n\n## Rationale\n\nA GitOps CI/CD process usually uses a deployment or ops repo containing Kubernetes manifests for multiple services and environments. Tools like *Argo-CD* or *Flux* then track these repo's, and apply any changes to the cluster. When a new image of an application is created, you want the corresponding tags to be updated in the manifests. Doing this manually is error prone. Having to write logic in every repo or pipeline to perform this is tedious. \n\nThis is where Nautikos comes in. \n\n## Installation \n\n```bash\npip install nautikos\n```\n\n## Basic usage \n\nNautikos is configured through a YAML-file (`./nautikos.yaml`), that specifies where the manifests for the different images and environments can be found: \n\n```yaml\nenvironments: \n- name: prod \n  manifests: \n  - path: prod/app1/deployment.yaml  # Path relative to configuration file\n    type: kubernetes  # Type can be 'kubernetes' or 'kustomize'\n    labels:  # Optional specification of labels for more granular control\n    - app1\n    - refs/heads/main\n  - path: prod/app2/kustomize.yaml\n    type: kustomize\n- name: dev\n  manifests: \n  - path: dev/app1/deployment.yaml\n    type: kubernetes\n    labels: \n    - app1\n    - refs/heads/dev\n  - path: dev/app3/feature-A/deployment.yaml\n    type: kubernetes\n    labels: \n    - app1\n    - refs/heads/feature-A\n```\n\nNext, you can run Nautikos to update the image tags of specific images in different environments.\n\n```bash\nnautikos my-repo 1.2.3  # Updates all occurences of `my-repo` to `1.2.3` in all manifests\nnautikos --env prod my-repo 2.3.4  # Updates all occurences of `my-repo` to `2.3.4` in `prod/app1/deployment.yaml` and `prod/app2/deployment`\nnautikos --env dev --labels app1 my-repo 4.5.6  # Updates all occurences of `my-repo` to `4.5.6` in `dev/app1/deployment.yaml`\nnautikos --labels 'app1,refs/heads/main' my-repo 5.6.7  # Updates all occurences of `my-repo` to `5.6.7` in `prod/app1/deployment.yaml`\n```\n\n## Supported tools\n\nThe tool works with standard **Kubernetes** manifests and **Kustomize** - **Helm** might be added later. Each have their own format for defining image tags. \n\n```yaml\n# Kubernetes manifests\nspec:\n  template:\n    spec:\n      containers:\n      - image: some-repository:tag\n\n# Kustomize\nimages: \n- name: some-repository\n  newTag: tag \n```\n\n## Advanced usage\n\nNautikos takes several options: \n\n* `--dry-run`: prints the modified files to stdout, but doesn't edit in place \n* `--config config-file.yaml`: path to config YAML, default is `./nautikos.yaml`\n\n## Alternatives \n\nThere are basically three alternatives to do the same thing: \n\n* **Update manifests manually** - of course this works, but this is not really proper CD\n* **Write your own bash scripts in a pipeline using a tool like `sed` or `yq`** - This works, but having to write this logic for every project is tedious. \n* **Use a tool like [Argo-CD Image updater](https://argocd-image-updater.readthedocs.io/en/stable/)** - very nice, but a bit heavy-weight, not very actively developed, and doesn't seem to support Azure Container Registry. \n\n## Notes \n\nMultiple YAML docs in one file is not yet supported. \n\n## Dependencies \n\n* **`typer`** - for creating a CLI \n* **`ruamel.yaml`** - for handling YAML files while maintaining ordering and comments\n",
     'author': 'Jan Hein de Jong',
     'author_email': 'janhein.dejong@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://www.github.com/janheindejong/nautikos',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `nautikos-0.3.1/PKG-INFO` & `nautikos-0.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 Metadata-Version: 2.1
 Name: nautikos
-Version: 0.3.1
+Version: 0.3.2
 Summary: A CD tool for updating image tags in Kubernetes manifests
+Home-page: https://www.github.com/janheindejong/nautikos
+License: MIT
+Keywords: kubernetes,devops,cicd,kustomize,gitops
 Author: Jan Hein de Jong
 Author-email: janhein.dejong@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Build Tools
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # Nautikos 
 
 *A lightweight CI/CD tool for updating image tags in Kubernetes manifests.*
```

