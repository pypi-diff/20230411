# Comparing `tmp/nautikos-0.3.0.tar.gz` & `tmp/nautikos-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautikos-0.3.0.tar", max compression
+gzip compressed data, was "nautikos-0.3.1.tar", max compression
```

## Comparing `nautikos-0.3.0.tar` & `nautikos-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-03-21 07:42:17.427920 nautikos-0.3.0/nautikos/__init__.py
--rw-r--r--   0        0        0     1217 2023-04-11 13:10:10.379476 nautikos-0.3.0/nautikos/cli.py
--rw-r--r--   0        0        0     4019 2023-04-11 13:10:52.861041 nautikos-0.3.0/nautikos/manifests.py
--rw-r--r--   0        0        0     3525 2023-04-11 12:42:55.258242 nautikos-0.3.0/nautikos/nautikos.py
--rw-r--r--   0        0        0       80 2023-03-24 10:25:48.952431 nautikos-0.3.0/nautikos/yaml.py
--rw-r--r--   0        0        0      952 2023-04-11 13:12:55.736844 nautikos-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3730 2023-04-11 08:03:55.985291 nautikos-0.3.0/README.md
--rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 nautikos-0.3.0/setup.py
--rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 nautikos-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-21 07:42:17.427920 nautikos-0.3.1/nautikos/__init__.py
+-rw-r--r--   0        0        0     1333 2023-04-11 15:12:06.664571 nautikos-0.3.1/nautikos/cli.py
+-rw-r--r--   0        0        0     4171 2023-04-11 15:12:06.789634 nautikos-0.3.1/nautikos/manifests.py
+-rw-r--r--   0        0        0     3214 2023-04-11 14:40:08.893216 nautikos-0.3.1/nautikos/nautikos.py
+-rw-r--r--   0        0        0       80 2023-03-24 10:25:48.952431 nautikos-0.3.1/nautikos/yaml.py
+-rw-r--r--   0        0        0      952 2023-04-11 15:11:24.851096 nautikos-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3730 2023-04-11 08:03:55.985291 nautikos-0.3.1/README.md
+-rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 nautikos-0.3.1/setup.py
+-rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 nautikos-0.3.1/PKG-INFO
```

### Comparing `nautikos-0.3.0/nautikos/cli.py` & `nautikos-0.3.1/nautikos/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,23 @@
     repository: str,
     tag: str,
     env: str = typer.Option(None),
     labels: str = typer.Option(None),
     config: str = typer.Option("nautikos.yaml"),
     dry_run: bool = typer.Option(False, "--dry-run"),
 ):
+    s = f"Updating '{repository}' to '{tag}'"
+    if env:
+        s += f" in '{env}'"
+    else:
+        s += " in all environments"
+    if labels:
+        s += f" with labels '{labels}'"
+    print(s)
+
     nautikos.set_dry_run(dry_run)
     nautikos.load_config(config)
     nautikos.update_manifests(
         repository, tag, environment=env, labels=labels.split(",") if labels else None
     )
 
     # Print modified files
@@ -31,15 +40,12 @@
         if mod.updated:
             count_updated_img += 1
 
     # Determine output
     if len(nautikos.modifications) == 0:
         exit_msg = "ERROR - Didn't find any images to modify"
         exit_code = 1
-    elif count_updated_img == 0:
-        exit_msg = "WARNING - All found images are already up-to-date"
-        exit_code = 0
     else:
-        exit_msg = f"Successfully updated {count_updated_img} occurances of '{repository}' to '{tag}'"  # noqa: E501
+        exit_msg = f"Updated {count_updated_img} out of {len(nautikos.modifications)} discovered occurances of '{repository}' to '{tag}'"  # noqa: E501
         exit_code = 0
     print(exit_msg)
     sys.exit(exit_code)
```

### Comparing `nautikos-0.3.0/nautikos/manifests.py` & `nautikos-0.3.1/nautikos/manifests.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,18 @@
     new: str
 
     @property
     def updated(self) -> bool:
         return self.previous != self.new
 
     def __str__(self) -> str:
-        return f"{self.path} -> modified '{self.repository}' (was '{self.previous}')"
+        if self.updated:
+            return f"{self.path} -> modified '{self.repository}' to '{self.new}' (was '{self.previous}')"  # noqa: E501
+        else:
+            return f"{self.path} -> '{self.repository}' already up-to-date"
 
 
 class AbstractManifest(abc.ABC):
     def __init__(self, path: str | pathlib.Path) -> None:
         self._path = path
         self._modifications: list[Modification] = []
```

### Comparing `nautikos-0.3.0/nautikos/nautikos.py` & `nautikos-0.3.1/nautikos/nautikos.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,26 +56,19 @@
         otherwise all environments are modified.
 
         If label is passed, only manifests with matching label are modified; otherwise
         all manifests in selected environments are modified.
         """
         # Get all relevant environments
         environments = self._get_environments(environment)
-        if len(environments) == 0:
-            raise Exception(f"Oops! No environments found; environment={environment}")
 
         # Get all relevant manifests
         manifests: list[ManifestConfig] = []
         for env in environments:
             manifests += self._get_manifests(env, labels)
-        if len(manifests) == 0:
-            raise Exception(
-                f"Oops!! No manifest found; environment={environment};"
-                f"labels={labels}"
-            )
 
         # Modify manifests
         for manifest_config in manifests:
             manifest = get_manifest(
                 manifest_config["path"],
                 manifest_config["type"],
                 workdir=self._workdir,
```

### Comparing `nautikos-0.3.0/pyproject.toml` & `nautikos-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautikos"
-version = "0.3.0"
+version = "0.3.1"
 description = "A CD tool for updating image tags in Kubernetes manifests"
 authors = ["Jan Hein de Jong <janhein.dejong@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 nautikos = "nautikos.cli:app"
```

### Comparing `nautikos-0.3.0/README.md` & `nautikos-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nautikos-0.3.0/setup.py` & `nautikos-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['ruamel-yaml>=0.17.21,<0.18.0', 'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['nautikos = nautikos.cli:app']}
 
 setup_kwargs = {
     'name': 'nautikos',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'A CD tool for updating image tags in Kubernetes manifests',
     'long_description': "# Nautikos \n\n*A lightweight CI/CD tool for updating image tags in Kubernetes manifests.* \n\n[![PyPI version](https://badge.fury.io/py/nautikos.svg)](https://badge.fury.io/py/nautikos)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Python versions](https://img.shields.io/pypi/pyversions/nautikos)]()\n\n## Rationale\n\nA GitOps CI/CD process usually uses a deployment or ops repo containing Kubernetes manifests for multiple services and environments. Tools like *Argo-CD* or *Flux* then track these repo's, and apply any changes to the cluster. When a new image of an application is created, you want the corresponding tags to be updated in the manifests. Doing this manually is error prone. Having to write logic in every repo or pipeline to perform this is tedious. \n\nThis is where Nautikos comes in. \n\n## Installation \n\n```bash\npip install nautikos\n```\n\n## Basic usage \n\nNautikos is configured through a YAML-file (`./nautikos.yaml`), that specifies where the manifests for the different images and environments can be found: \n\n```yaml\nenvironments: \n- name: prod \n  manifests: \n  - path: prod/app1/deployment.yaml  # Path relative to configuration file\n    type: kubernetes  # Type can be 'kubernetes' or 'kustomize'\n    labels:  # Optional specification of labels for more granular control\n    - app1\n    - refs/heads/main\n  - path: prod/app2/kustomize.yaml\n    type: kustomize\n- name: dev\n  manifests: \n  - path: dev/app1/deployment.yaml\n    type: kubernetes\n    labels: \n    - app1\n    - refs/heads/dev\n  - path: dev/app3/feature-A/deployment.yaml\n    type: kubernetes\n    labels: \n    - app1\n    - refs/heads/feature-A\n```\n\nNext, you can run Nautikos to update the image tags of specific images in different environments.\n\n```bash\nnautikos my-repo 1.2.3  # Updates all occurences of `my-repo` to `1.2.3` in all manifests\nnautikos --env prod my-repo 2.3.4  # Updates all occurences of `my-repo` to `2.3.4` in `prod/app1/deployment.yaml` and `prod/app2/deployment`\nnautikos --env dev --labels app1 my-repo 4.5.6  # Updates all occurences of `my-repo` to `4.5.6` in `dev/app1/deployment.yaml`\nnautikos --labels 'app1,refs/heads/main' my-repo 5.6.7  # Updates all occurences of `my-repo` to `5.6.7` in `prod/app1/deployment.yaml`\n```\n\n## Supported tools\n\nThe tool works with standard **Kubernetes** manifests and **Kustomize** - **Helm** might be added later. Each have their own format for defining image tags. \n\n```yaml\n# Kubernetes manifests\nspec:\n  template:\n    spec:\n      containers:\n      - image: some-repository:tag\n\n# Kustomize\nimages: \n- name: some-repository\n  newTag: tag \n```\n\n## Advanced usage\n\nNautikos takes several options: \n\n* `--dry-run`: prints the modified files to stdout, but doesn't edit in place \n* `--config config-file.yaml`: path to config YAML, default is `./nautikos.yaml`\n\n## Alternatives \n\nThere are basically three alternatives to do the same thing: \n\n* **Update manifests manually** - of course this works, but this is not really proper CD\n* **Write your own bash scripts in a pipeline using a tool like `sed` or `yq`** - This works, but having to write this logic for every project is tedious. \n* **Use a tool like [Argo-CD Image updater](https://argocd-image-updater.readthedocs.io/en/stable/)** - very nice, but a bit heavy-weight, not very actively developed, and doesn't seem to support Azure Container Registry. \n\n## Notes \n\nMultiple YAML docs in one file is not yet supported. \n\n## Dependencies \n\n* **`typer`** - for creating a CLI \n* **`ruamel.yaml`** - for handling YAML files while maintaining ordering and comments\n",
     'author': 'Jan Hein de Jong',
     'author_email': 'janhein.dejong@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `nautikos-0.3.0/PKG-INFO` & `nautikos-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautikos
-Version: 0.3.0
+Version: 0.3.1
 Summary: A CD tool for updating image tags in Kubernetes manifests
 Author: Jan Hein de Jong
 Author-email: janhein.dejong@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

