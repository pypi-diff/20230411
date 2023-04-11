# Comparing `tmp/edwh-0.3.3.tar.gz` & `tmp/edwh-0.4.1.tar.gz`

## Comparing `edwh-0.3.3.tar` & `edwh-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 edwh-0.3.3/CHANGELOG.md
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 edwh-0.3.3/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.3.3/src/edwh/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.3/src/edwh/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 edwh-0.3.3/src/edwh/cli.py
--rw-r--r--   0        0        0    16936 2020-02-02 00:00:00.000000 edwh-0.3.3/src/edwh/tasks.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.3.3/tests/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.3.3/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.3.3/LICENSE.txt
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.3.3/README.md
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 edwh-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 edwh-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 edwh-0.4.1/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh-0.4.1/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh-0.4.1/src/edwh/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.4.1/src/edwh/__init__.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 edwh-0.4.1/src/edwh/cli.py
+-rw-r--r--   0        0        0    16612 2020-02-02 00:00:00.000000 edwh-0.4.1/src/edwh/tasks.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 edwh-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 edwh-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 edwh-0.4.1/README.md
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 edwh-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 edwh-0.4.1/PKG-INFO
```

### Comparing `edwh-0.3.3/CHANGELOG.md` & `edwh-0.4.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `edwh-0.3.3/src/edwh/cli.py` & `edwh-0.4.1/src/edwh/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 
 discovered_plugins = entry_points(group='edwh.tasks')
 for plugin in discovered_plugins:
     plugin_module = plugin.load()
     plugin_collection = Collection.from_module(plugin_module)
     collection.add_collection(plugin_collection, plugin.name)
 
-import os
-print('Discovered plugins:',[_.value.split('.')[0] for _ in discovered_plugins])
+# print('Discovered plugins:',[_.value.split('.')[0] for _ in discovered_plugins])
 
 old_path = sys.path[:]
 
 for path in ['.', '..', '../..']:
     path = pathlib.Path(path)
     sys.path = [str(path)] + old_path
     try:
@@ -35,11 +34,8 @@
         collection.add_collection(local, 'local')
         break
     except ImportError as e:
         if 'No module named \'tasks\'' not in str(e):
             raise e
 sys.path = old_path
 
-
-
-
 program = Program(namespace=collection, version=__version__)
```

### Comparing `edwh-0.3.3/src/edwh/tasks.py` & `edwh-0.4.1/src/edwh/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,15 @@
     import tomlkit
     from dataclasses import dataclass, field
     from pathlib import Path
     from collections import defaultdict, OrderedDict
 
 except ImportError as e:
     if sys.argv[0].split("/")[-1] in ("inv", "invoke"):
-        print(
-            "WARNING: this tasks.py works best using the edwh command instead of using inv[oke] directly.\n"
-        )
+        print("WARNING: this tasks.py works best using the edwh command instead of using inv[oke] directly.\n")
     print("ImportError:", e)
     exit(1)
 
 
 def confirm(prompt: str, default=False) -> bool:
     allowed = {"y", "1"}
     if default:
@@ -44,17 +42,15 @@
 class TomlConfig:
     config: dict
     all_services: list[str]
     celeries: list[str]
     services_minimal: list[str]
     services_log: list[str]
     dotenv_path: Path
-    __loaded: "TomlConfig" = field(
-        init=False, default=None
-    )  # cache using class instance singleton
+    __loaded: "TomlConfig" = field(init=False, default=None)  # cache using class instance singleton
 
     @classmethod
     def load(cls):
         """
         Load config toml file, raising an error if it does not exist.
 
         Since this file should be in .git error suppression is not needed.
@@ -171,17 +167,15 @@
     """
     Test if key is in .env file path, appends prompted or default value if missing.
     """
     config = TomlConfig.load()
     env = read_dotenv()
     if key not in env:
         with config.dotenv_path.open(mode="r+") as env_file:
-            response = input(
-                f"Enter value for {key} ({comment})\n default=`{default}`: "
-            )
+            response = input(f"Enter value for {key} ({comment})\n default=`{default}`: ")
             value = response.strip() or default
             if prefix:
                 value = prefix + value
             if postfix:
                 value += postfix
             env_file.seek(0, 2)
             env_file.write(f"\n{key.upper()}={value}\n")
@@ -286,40 +280,32 @@
 
 # noinspection PyUnusedLocal
 @task(help=dict(find="search for this specific setting"))
 def settings(ctx, find=None):
     """
     Show all settings in .env file or search for a specific setting using -f/--find.
     """
-    rows = [
-        (k, v)
-        for k, v in read_dotenv().items()
-        if find is None or find.upper() in k.upper() or find in v
-    ]
+    rows = [(k, v) for k, v in read_dotenv().items() if find is None or find.upper() in k.upper() or find in v]
     print(tabulate.tabulate(rows, headers=["Setting", "Value"]))
 
 
 @task(aliases=tuple(["volume"]))
 def volumes(ctx):
     """
     Show container and volume names.
 
     Based on `docker-compose ps -q` ids and `docker inspect` output.
     """
     lines = []
-    for container_id in (
-        ctx.run("docker-compose ps -q", hide=True, warn=True).stdout.strip().split("\n")
-    ):
+    for container_id in ctx.run("docker-compose ps -q", hide=True, warn=True).stdout.strip().split("\n"):
         ran = ctx.run(f"docker inspect {container_id}", hide=True, warn=True)
         if ran.ok:
             info = json.loads(ran.stdout)
             container = info[0]["Name"]
-            for volume in [
-                _["Name"] for _ in info[0]["Mounts"] if _["Type"] == "volume"
-            ]:
+            for volume in [_["Name"] for _ in info[0]["Mounts"] if _["Type"] == "volume"]:
                 lines.append(dict(container=container, volume=volume))
         else:
             print(ran.stderr)
 
     print(tabulate.tabulate(lines, headers="keys"))
 
 
@@ -356,21 +342,17 @@
 
     if build:
         ctx.run(f"docker-compose build {services_ls}")
     if quickest:
         ctx.run(f"docker-compose restart {services_ls}")
     else:
         ctx.run(f"docker-compose stop -t {stop_timeout}  {services_ls}")
-        ctx.run(
-            f"docker-compose up {'--renew-anon-volumes --build' if clean else ''} -d {services_ls}"
-        )
+        ctx.run(f"docker-compose up {'--renew-anon-volumes --build' if clean else ''} -d {services_ls}")
     if "py4web" in services_ls:
-        ctx.run(
-            f"docker-compose run --rm migrate invoke -r /shared_code/edwh/core/backend -c support update-opengraph"
-        )
+        ctx.run(f"docker-compose run --rm migrate invoke -r /shared_code/edwh/core/backend -c support update-opengraph")
     if tail:
         ctx.run(f"docker-compose logs --tail=10 -f {services_ls}")
 
 
 @task(
     iterable=["service"],
     help=dict(
@@ -378,17 +360,15 @@
         quiet="Only show container ids. Useful for scripting.",
     ),
 )
 def ps(ctx, quiet=False, service=None):
     """
     Show process status of services.
     """
-    ctx.run(
-        f'docker-compose ps {"-q" if quiet else ""} {" ".join(service_names(service or []))}'
-    )
+    ctx.run(f'docker-compose ps {"-q" if quiet else ""} {" ".join(service_names(service or []))}')
 
 
 @task(
     aliases=tuple(["log"]),
     iterable=["service"],
     help={
         "follow": "Keep scrolling with the output.",
@@ -408,31 +388,27 @@
     if service:
         cmdline.extend(service_names(service))
     ctx.run(" ".join(cmdline))
 
 
 @task(
     iterable=["service"],
-    help=dict(
-        service="Service to stop, can be used multiple times, handles wildcards."
-    ),
+    help=dict(service="Service to stop, can be used multiple times, handles wildcards."),
 )
 def stop(ctx, service=None):
     """
     Stops services using docker-compose stop.
     """
     service = service_names(service or [])
     ctx.run(f"docker-compose stop {' '.join(service)}")
 
 
 @task(
     iterable=["service"],
-    help=dict(
-        service="Service to stop, can be used multiple times, handles wildcards."
-    ),
+    help=dict(service="Service to stop, can be used multiple times, handles wildcards."),
 )
 def down(ctx, service=None):
     """
     Stops services using docker-compose down.
     """
     service = service_names(service or [])
     ctx.run(f"docker-compose down {' '.join(service)}")
@@ -455,43 +431,37 @@
 
     try:
         # noinspection PyUnresolvedReferences
         import edwh_pipcompile_plugin as pcl
 
         with_compile = True
     except ImportError:
-        print(
-            "`edwh-pipcompile-plugin` not found, unable to compile requirements.in files."
-        )
+        print("`edwh-pipcompile-plugin` not found, unable to compile requirements.in files.")
         print("Install with `pipx inject edwh edwh-pipcompile-plugin`")
         print()
         print("possible files to compile:")
         for req in reqs:
             print("  ", req)
         with_compile = False
 
     if with_compile:
         for idx, req in enumerate(reqs, 1):
             reqtxt = req.parent / "requirements.txt"
             print(
                 f"{idx}/{len(reqs)}: working on {req}",
             )
             if (not reqtxt.exists()) or (reqtxt.stat().st_ctime < req.stat().st_ctime):
-                print(
-                    "outdated" if reqtxt.exists() else "requirements.txt doesn't exist."
-                )
+                print("outdated" if reqtxt.exists() else "requirements.txt doesn't exist.")
                 if yes or confirm(f"recompile {req}? [Yn]", default=True):
                     pcl.compile(ctx, str(req.parent))
             else:
                 print("still current")
     else:
         print("Compilation of requirements.in files skipped.")
-    if yes or (
-        not with_compile and confirm("Build docker images? [yN]", default=False)
-    ):
+    if yes or (not with_compile and confirm("Build docker images? [yN]", default=False)):
         ctx.run("docker-compose build")
 
 
 @task(
     help=dict(
         service="Service to rebuild, can be used multiple times, handles wildcards.",
         force_rebuild="uses --no-cache option for docker-compose build",
@@ -506,18 +476,15 @@
     """
     Downs ALL services, then rebuilds services using docker-compose build.
     """
     if service is None:
         service = []
     ctx.run("docker-compose down")
     services = service_names(service)
-    ctx.run(
-        f"docker-compose build {'--no-cache' if force_rebuild else ''} "
-        + " ".join(services)
-    )
+    ctx.run(f"docker-compose build {'--no-cache' if force_rebuild else ''} " + " ".join(services))
 
 
 @task()
 def docs(ctx, reinstall=False):
     """
     Local hosted mkdocs documentation.
```

### Comparing `edwh-0.3.3/LICENSE.txt` & `edwh-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh-0.3.3/README.md` & `edwh-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `edwh-0.3.3/pyproject.toml` & `edwh-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh-0.3.3/PKG-INFO` & `edwh-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh
-Version: 0.3.3
+Version: 0.4.1
 Summary: Education Warehouse maintenance tools
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>, Romy Schöller <romy.s@educationwarehouse.nl>, Sven Keimpema <sven.k@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

