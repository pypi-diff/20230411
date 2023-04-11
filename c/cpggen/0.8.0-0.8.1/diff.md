# Comparing `tmp/cpggen-0.8.0.tar.gz` & `tmp/cpggen-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-0.8.0.tar", max compression
+gzip compressed data, was "cpggen-0.8.1.tar", max compression
```

## Comparing `cpggen-0.8.0.tar` & `cpggen-0.8.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-09 21:17:58.868180 cpggen-0.8.0/LICENSE
--rw-r--r--   0        0        0     6474 2023-04-09 21:17:58.868180 cpggen-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-04-09 21:17:58.872180 cpggen-0.8.0/cpggen/__init__.py
--rw-r--r--   0        0        0    12106 2023-04-09 21:17:58.872180 cpggen-0.8.0/cpggen/cli.py
--rw-r--r--   0        0        0    18921 2023-04-09 21:17:58.872180 cpggen-0.8.0/cpggen/executor.py
--rw-r--r--   0        0        0      731 2023-04-09 21:17:58.872180 cpggen-0.8.0/cpggen/logger.py
--rw-r--r--   0        0        0     9682 2023-04-09 21:17:58.872180 cpggen-0.8.0/cpggen/utils.py
--rw-r--r--   0        0        0     1245 2023-04-09 21:17:58.872180 cpggen-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     7802 1970-01-01 00:00:00.000000 cpggen-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 06:29:33.544823 cpggen-0.8.1/LICENSE
+-rw-r--r--   0        0        0     6570 2023-04-11 06:29:33.544823 cpggen-0.8.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 06:29:33.548823 cpggen-0.8.1/cpggen/__init__.py
+-rw-r--r--   0        0        0    12884 2023-04-11 06:29:33.548823 cpggen-0.8.1/cpggen/cli.py
+-rw-r--r--   0        0        0    22431 2023-04-11 06:29:33.548823 cpggen-0.8.1/cpggen/executor.py
+-rw-r--r--   0        0        0      746 2023-04-11 06:29:33.548823 cpggen-0.8.1/cpggen/logger.py
+-rw-r--r--   0        0        0    10065 2023-04-11 06:29:33.548823 cpggen-0.8.1/cpggen/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-11 06:29:33.548823 cpggen-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7898 1970-01-01 00:00:00.000000 cpggen-0.8.1/PKG-INFO
```

### Comparing `cpggen-0.8.0/LICENSE` & `cpggen-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-0.8.0/README.md` & `cpggen-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - cpggen with Python 3.10
 - cdxgen with Node.js 18
 - cdxgen binary plugins
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.8.0/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.8.1/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v0.8.0/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v0.8.1/cpggen.exe
 .\cpggen.exe --help
 ```
 
 ### OCI Artifacts via ORAS cli
 
 Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
 
@@ -172,14 +172,15 @@
 | CPGGEN_CONTAINER_CPU    | CPU units to use in container execution mode. Default computed    |
 | CPGGEN_CONTAINER_MEMORY | Memory units to use in container execution mode. Default computed |
 | CPGGEN_MEMORY           | Heap memory to use for frontends. Default computed                |
 | AT_DEBUG_MODE           | Set to debug to enable debug logging                              |
 | CPG_EXPORT              | Set to true to export CPG graphs in dot format                    |
 | CPG_EXPORT_REPR         | Graph to export. Default all                                      |
 | CPG_EXPORT_FORMAT       | Export format. Default dot                                        |
+| SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI      |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
 - name: Upload cpg
```

### Comparing `cpggen-0.8.0/cpggen/cli.py` & `cpggen-0.8.1/cpggen/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import argparse
 import json
 import os
 import shutil
 import signal
 import tempfile
 from multiprocessing import Pool
-from pathlib import Path
+from pathlib import Path, PurePath
 
 from quart import Quart, request
 
 from cpggen import executor, utils
 from cpggen.logger import LOG, console
 
 try:
@@ -38,19 +38,15 @@
     Constructs command line arguments for the scanner
     """
     parser = argparse.ArgumentParser(description="CPG Generator")
     parser.add_argument(
         "-i", "--src", dest="src", help="Source directory or url", default=os.getcwd()
     )
     parser.add_argument(
-        "-o",
-        "--out-dir",
-        dest="cpg_out_dir",
-        help="CPG output directory",
-        default=os.path.join(os.getcwd(), "cpg_out"),
+        "-o", "--out-dir", dest="cpg_out_dir", help="CPG output directory"
     )
     parser.add_argument(
         "-l",
         "--lang",
         dest="language",
         help="Optional. CPG language frontend to use. Auto-detects by default.",
         choices=[
@@ -138,15 +134,14 @@
         default=os.getenv("CPG_EXPORT_FORMAT", "dot"),
         dest="export_format",
         choices=["neo4jcsv", "graphml", "graphson", "dot"],
         help="Export format",
     )
     parser.add_argument(
         "--export-out-dir",
-        default=os.path.join(os.getcwd(), "export_out"),
         dest="export_out_dir",
         help="Export output directoru",
     )
     return parser.parse_args()
 
 
 @app.get("/")
@@ -156,15 +151,15 @@
 
 def run_server(args):
     console.print(product_logo, style="info")
     console.print(f"cpggen server running on {args.server_host}:{args.server_port}")
     app.run(
         host=args.server_host,
         port=args.server_port,
-        debug=True if os.getenv("AT_DEBUG_MODE") == "debug" else False,
+        debug=True if os.getenv("AT_DEBUG_MODE") in ("debug", "true", "1") else False,
         use_reloader=False,
     )
 
 
 @app.route("/cpg", methods=["GET", "POST"])
 async def generate_cpg():
     q = request.args
@@ -294,22 +289,31 @@
                                 except Exception:
                                     # Ignore remove errors
                                     pass
                             os.makedirs(export_out_dir, exist_ok=True)
                         except Exception:
                             # Ignore errors
                             pass
+                        cpg_path = manifest_obj["cpg"]
+                        # In case of GitHub action we need to fix the cpg_path to prefix GITHUB_WORKSPACE
+                        # since the manifest would only have relative path
+                        if os.getenv("GITHUB_WORKSPACE") and not cpg_path.startswith(
+                            os.getenv("GITHUB_WORKSPACE")
+                        ):
+                            cpg_path = os.path.join(
+                                os.getenv("GITHUB_WORKSPACE"), cpg_path
+                            )
                         LOG.debug(
-                            f"""Exporting CPG for the app {manifest_obj["app"]} to {app_export_out_dir}"""
+                            f"""Exporting CPG for the app {manifest_obj["app"]} from {cpg_path} to {app_export_out_dir}"""
                         )
                         pool.apply_async(
                             executor.exec_tool,
                             (
                                 "export",
-                                manifest_obj["cpg"],
+                                cpg_path,
                                 app_export_out_dir,
                                 cpg_out_dir,
                                 joern_home,
                                 use_container,
                                 False,
                                 {
                                     "export_repr": export_repr,
@@ -324,16 +328,23 @@
 
 
 def main():
     print(product_logo)
     args = build_args()
     if args.server_mode:
         return run_server(args)
-    src = args.src
+    src = str(PurePath(args.src))
     cpg_out_dir = args.cpg_out_dir
+    if not cpg_out_dir and src:
+        cpg_out_dir = os.path.join(src, "cpg_out")
+    cpg_out_dir = str(PurePath(cpg_out_dir))
+    export_out_dir = args.export_out_dir
+    if not export_out_dir and src:
+        export_out_dir = os.path.join(src, "export_out")
+    export_out_dir = str(PurePath(export_out_dir))
     languages = args.language
     joern_home = args.joern_home
     use_container = args.use_container
     if joern_home and not os.path.exists(joern_home):
         if utils.check_command("docker") or utils.check_command("podman"):
             use_container = True
         else:
@@ -370,15 +381,15 @@
         export_cpg(
             src,
             cpg_out_dir,
             joern_home=joern_home,
             use_container=use_container,
             export_repr=args.export_repr,
             export_format=args.export_format,
-            export_out_dir=args.export_out_dir,
+            export_out_dir=export_out_dir,
         )
     if is_temp_dir:
         try:
             shutil.rmtree(src)
         except Exception:
             # Ignore cleanup errors
             pass
```

### Comparing `cpggen-0.8.0/cpggen/executor.py` & `cpggen-0.8.1/cpggen/executor.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,17 +8,21 @@
 from psutil._common import bytes2human
 from rich.progress import Progress
 
 from cpggen.logger import DEBUG, LOG, console
 from cpggen.utils import (
     check_command,
     find_csharp_artifacts,
+    find_files,
     find_go_mods,
+    find_gradle_files,
     find_java_artifacts,
     find_makefiles,
+    find_pom_files,
+    find_sbt_files,
 )
 
 runtimeValues = {}
 svmem = psutil.virtual_memory()
 max_memory = bytes2human(getattr(svmem, "available"), format="%(value).0f%(symbol)s")
 cpu_count = str(psutil.cpu_count())
 
@@ -58,29 +62,40 @@
     "jar": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar -nojsp -nb --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
     "jar-with-blocklist": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar -nojsp --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
     "scala": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar -nojsp -nb --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar -nb --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp-with-blocklist": "java -Xmx%(memory)s -jar /usr/local/bin/java2cpg.jar --experimental-langs scala -su -o %(cpg_out)s %(uber_jar)s",
     "sbom": "cdxgen -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
     "export": "joern-export --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
+    "qwiet": "sl analyze --tag app.group=%(group)s --app %(app)s-%(language)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
 }
 
 build_tools_map = {
     "csharp": ["dotnet", "build"],
     "java": {
         "maven": [
             get("MVN_CMD", "mvn"),
             "compile",
             "package",
             "-Dmaven.test.skip=true",
         ],
-        "gradle": [get("GRADLE_CMD", "gradle"), "build"],
+        "gradle": [get("GRADLE_CMD", "%(gradle_cmd)s"), "build"],
         "sbt": ["sbt", "compile"],
     },
-    "android": {"gradle": [get("GRADLE_CMD", "gradle"), "compileDebugSources"]},
+    "jar": {
+        "maven": [
+            get("MVN_CMD", "mvn"),
+            "compile",
+            "package",
+            "-Dmaven.test.skip=true",
+        ],
+        "gradle": [get("GRADLE_CMD", "%(gradle_cmd)s"), "jar"],
+        "sbt": ["sbt", "stage"],
+    },
+    "android": {"gradle": [get("GRADLE_CMD", "%(gradle_cmd)s"), "compileDebugSources"]},
     "kotlin": {
         "maven": [
             get("MVN_CMD", "mvn"),
             "compile",
             "package",
             "-Dmaven.test.skip=true",
         ],
@@ -88,96 +103,126 @@
     },
     "scala": ["sbt", "stage"],
     "nodejs": {
         "npm": ["npm", "install", "--prefer-offline", "--no-audit", "--progress=false"],
         "yarn": ["yarn", "install"],
         "rush": ["rush", "install", "--bypass-policy", "--no-link"],
     },
-    "go": ["go", "build", "./..."],
+    "go": {
+        "go": ["go", "build", "./..."],
+        "make": ["make", "build"],
+    },
     "php": {
         "init": ["composer", "init", "--quiet"],
         "install": ["composer", "install", "-n", "--ignore-platform-reqs"],
         "update": ["composer", "update", "-n", "--ignore-platform-reqs"],
         "autoload": ["composer", "dump-autoload", "-o"],
     },
     "make": ["make", "build"],
 }
 
 
-def do_go_build(src, env):
-    go_mods = find_go_mods(src)
-    makes = find_makefiles(src)
-    build_args = build_tools_map["go"]
-    for gmod in go_mods:
-        base_dir = os.path.dirname(gmod)
-        try:
-            LOG.debug(f"Executing {' '.join(build_args)} in {base_dir}")
-            subprocess.run(
-                build_args,
-                stdout=subprocess.DEVNULL,
-                stderr=subprocess.DEVNULL,
-                cwd=base_dir,
-                env=env,
-                check=False,
-                shell=False,
-                encoding="utf-8",
-            )
-        except Exception as e:
-            LOG.debug(e)
-    build_args = build_tools_map["make"]
-    for make in makes:
-        base_dir = os.path.dirname(make)
-        try:
-            LOG.debug(f"Executing {' '.join(build_args)} in {base_dir}")
-            subprocess.run(
-                build_args,
-                stdout=subprocess.DEVNULL,
-                stderr=subprocess.DEVNULL,
-                cwd=base_dir,
-                env=env,
-                check=False,
-                shell=False,
-                encoding="utf-8",
+def qwiet_analysis(app_manifest, cwd, env):
+    try:
+        LOG.info(f"Submitting {app_manifest['app']} for Qwiet.AI analysis")
+        build_args = cpg_tools_map["qwiet"]
+        build_args = build_args % dict(**app_manifest)
+        LOG.debug(f"Executing {build_args}")
+        cp = subprocess.run(
+            build_args.split(" "),
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            cwd=cwd,
+            env=env,
+            check=False,
+            shell=False,
+            encoding="utf-8",
+        )
+        if cp:
+            if LOG.isEnabledFor(DEBUG) and cp.stdout:
+                LOG.debug(cp.stdout)
+            if cp.returncode and cp.stderr:
+                LOG.info(cp.stderr)
+            else:
+                LOG.info(f"{app_manifest['app']} uploaded successfully")
+    except Exception as e:
+        LOG.error(e)
+
+
+def do_x_build(src, env, build_artefacts, tool_lang):
+    for k, v in build_artefacts.items():
+        build_sets = build_tools_map.get(tool_lang)
+        if isinstance(build_sets, dict):
+            build_args = build_tools_map[tool_lang][k]
+        else:
+            build_args = build_sets
+        for afile in v:
+            base_dir = os.path.dirname(afile)
+            build_args_str = " ".join(build_args)
+            if "%(" in build_args_str:
+                gradle_cmd = "gradle"
+                if os.path.exists(os.path.join(base_dir, "gradlew")):
+                    gradle_cmd = "gradlew"
+                    try:
+                        os.chmod(os.path.join(base_dir, "gradlew"), 0o755)
+                    except Exception:
+                        # Ignore errors
+                        pass
+                build_args_str = build_args_str % dict(gradle_cmd=gradle_cmd)
+            try:
+                LOG.debug(
+                    f"Executing {build_args_str} in {base_dir}. To speed up this step, cache your project's dependencies using the CI build cache."
+                )
+                cp = subprocess.run(
+                    build_args_str.split(" "),
+                    stdout=subprocess.PIPE,
+                    stderr=subprocess.PIPE,
+                    cwd=base_dir,
+                    env=env,
+                    check=False,
+                    shell=False,
+                    encoding="utf-8",
+                )
+                if cp and LOG.isEnabledFor(DEBUG) and cp.returncode and cp.stderr:
+                    if cp.stderr:
+                        LOG.debug(cp.stderr)
+            except Exception as e:
+                LOG.debug(e)
+
+
+def do_jar_build(src, env):
+    build_artefacts = {
+        "gradle": find_gradle_files(src),
+        "maven": find_pom_files(src),
+        "sbt": find_sbt_files(src),
+    }
+    settings_xmls = find_files(src, "settings.xml", False, False)
+    if settings_xmls:
+        LOG.info(
+            "Maven settings.xml is present in this repo. This usually means that specific maven settings and profiles needs to be passed via the environment variable MVN_ARGS to build this application correctly."
+        )
+        if not os.getenv("AT_DEBUG_MODE"):
+            LOG.info(
+                "Set the environment variable AT_DEBUG_MODE to debug and look for any build errors"
             )
-        except Exception as e:
-            LOG.debug(e)
+    return do_x_build(src, env, build_artefacts, "jar")
+
+
+def do_go_build(src, env):
+    build_artefacts = {"go": find_go_mods(src), "make": find_makefiles(src)}
+    return do_x_build(src, env, build_artefacts, "go")
 
 
 def do_build(tool_lang, src, cwd, env):
-    build_args = None
-    if tool_lang in ("csharp", "scala"):
-        build_args = build_tools_map[tool_lang]
+    if tool_lang in ("csharp",):
+        do_x_build(src, env, {"csharp": find_csharp_artifacts(src)}, "csharp")
+    elif tool_lang in ("jar", "scala"):
+        do_jar_build(src, env)
     elif tool_lang == "go":
         do_go_build(src, env)
-    # For go, we need to detect the go.mod files and attempt build from those directories
-    if build_args:
-        LOG.info(
-            '⚡︎ Attempting to auto build {} "{}"'.format(
-                tool_lang, " ".join(build_args)
-            )
-        )
-        try:
-            cp = subprocess.run(
-                build_args,
-                stdout=subprocess.DEVNULL,
-                stderr=subprocess.DEVNULL,
-                cwd=cwd,
-                env=env,
-                check=False,
-                shell=False,
-                encoding="utf-8",
-            )
-            if cp:
-                if cp.stdout:
-                    LOG.info(cp.stdout)
-                if cp.stderr:
-                    LOG.info(cp.stderr)
-        except Exception as e:
-            LOG.warn("Auto build has failed")
-            LOG.warn(e)
 
 
 def exec_tool(
     tool_lang,
     src,
     cpg_out_dir,
     cwd=None,
@@ -216,20 +261,20 @@
                 return
             uber_jar = ""
             csharp_artifacts = ""
             # For languages like scala, jsp or jar we need to create a uber jar containing all jar, war files from the source directory
             if "uber_jar" in cmd_with_args:
                 stdout = subprocess.PIPE
                 java_artifacts = find_java_artifacts(src)
-                if len(java_artifacts) == 1:
+                if len(java_artifacts):
                     uber_jar = java_artifacts[0]
             if "csharp_artifacts" in cmd_with_args:
                 stdout = subprocess.PIPE
                 csharp_artifacts = find_csharp_artifacts(src)
-                if len(csharp_artifacts) == 1:
+                if len(csharp_artifacts):
                     csharp_artifacts = csharp_artifacts[0]
             if auto_build:
                 do_build(tool_lang, src, cwd, env)
             modules = [src]
             # For go, the modules are based on the presence of go.mod files
             if tool_lang == "go":
                 go_mods = find_go_mods(src)
@@ -300,26 +345,33 @@
                         LOG.warn(
                             f"{lang_cmd} is not found. Ensure the PATH variable in your container image is set to the bin directory of Joern."
                         )
                     return
                 # Is this an Export task?
                 if tool_lang == "export":
                     try:
+                        progress.update(
+                            task, description="Exporting CPG", completed=90, total=100
+                        )
                         cp = subprocess.run(
                             cmd_list_with_args,
                             stdout=stdout,
                             stderr=stderr,
                             cwd=cwd,
                             env=env,
                             check=False,
                             shell=False,
                             encoding="utf-8",
                         )
                         if cp and cp.returncode and cp.stderr:
                             LOG.warn(f"Export CPG has failed for {src}")
+                            if not os.getenv("AT_DEBUG_MODE"):
+                                LOG.info(
+                                    "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
+                                )
                             if cp.stdout:
                                 LOG.info(cp.stdout)
                             if cp.stderr:
                                 LOG.info("------------------------------")
                                 LOG.info(cp.stderr)
                                 LOG.info("------------------------------")
                                 LOG.info(
@@ -328,15 +380,15 @@
                         else:
                             if os.path.exists(src):
                                 LOG.info(
                                     f"CPG {src} successfully exported to {cpg_out_dir}"
                                 )
                             else:
                                 LOG.warn(
-                                    f"Unable to export {src} to {cpg_out_dir}. Try running joern-export manually"
+                                    f"Unable to export {src} to {cpg_out_dir}. Try running joern-export manually using the command {' '.join(cmd_list_with_args)}"
                                 )
                     except Exception:
                         LOG.warn(f"Unable to export {src} to {cpg_out_dir}")
                     progress.update(task, completed=100, total=100)
                     continue
                 LOG.debug(
                     '⚡︎ Generating CPG for the {} app "{}" - "{}"'.format(
@@ -346,27 +398,36 @@
                     )
                 )
                 cwd = amodule
                 if tool_lang in ("binary",):
                     cwd = os.getcwd()
                 # Generate sbom first since this would even download dependencies for java
                 try:
+                    progress.update(
+                        task,
+                        description="Generating SBoM using cdxgen",
+                        completed=10,
+                        total=100,
+                    )
                     subprocess.run(
                         sbom_cmd_list_with_args,
                         stdout=stdout,
                         stderr=stderr,
                         cwd=cwd,
                         env=env,
                         check=False,
                         shell=False,
                         encoding="utf-8",
                     )
                 except Exception:
                     # Ignore sbom generation errors
                     pass
+                progress.update(
+                    task, description="Generating CPG", completed=20, total=100
+                )
                 cp = subprocess.run(
                     cmd_list_with_args,
                     stdout=stdout,
                     stderr=stderr,
                     cwd=cwd,
                     env=env,
                     check=False,
@@ -377,15 +438,14 @@
                     for line in cp.stdout:
                         progress.update(task, completed=5)
                 if cp and LOG.isEnabledFor(DEBUG) and cp.returncode:
                     if cp.stdout:
                         LOG.debug(cp.stdout)
                     if cp.stderr:
                         LOG.debug(cp.stderr)
-                progress.update(task, completed=100, total=100)
                 if os.path.exists(cpg_out):
                     # go2cpg seems to produce a cpg without read permissions
                     try:
                         os.chmod(cpg_out, 0o644)
                     except Exception:
                         # Ignore errors
                         pass
@@ -411,30 +471,43 @@
                         # Let's improve the name for github action
                         if app_base_name == "workspace" and os.getenv(
                             "GITHUB_REPOSITORY"
                         ):
                             app_base_name = os.getenv("GITHUB_REPOSITORY").split("/")[
                                 -1
                             ]
-                        json.dump(
-                            {
-                                "src": amodule,
-                                "group": app_base_name,
-                                "app": f"{app_base_name}-{language}",
-                                "cpg": cpg_out,
-                                "sbom": sbom_out,
-                                "language": language,
-                                "cpg_frontend_invocation": " ".join(cmd_list_with_args),
-                                "sbom_invocation": " ".join(sbom_cmd_list_with_args),
-                            },
-                            mfp,
-                        )
+                        app_manifest = {
+                            "src": amodule,
+                            "group": app_base_name,
+                            "app": f"{app_base_name}-{language}",
+                            "cpg": cpg_out,
+                            "sbom": sbom_out,
+                            "language": language,
+                            "cpg_frontend_invocation": " ".join(cmd_list_with_args),
+                            "sbom_invocation": " ".join(sbom_cmd_list_with_args),
+                        }
+                        if os.getenv("SHIFTLEFT_ACCESS_TOKEN"):
+                            progress.update(
+                                task,
+                                description="Uploading to Qwiet AI for analysis",
+                                completed=90,
+                                total=100,
+                            )
+                            qwiet_analysis(app_manifest, cwd, env)
+                        json.dump(app_manifest, mfp)
                 else:
                     LOG.info(f"CPG {cpg_out} was not generated for {tool_lang}")
+                    if not os.getenv("AT_DEBUG_MODE"):
+                        LOG.info(
+                            "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
+                        )
                     if cp.stdout:
                         LOG.info(cp.stdout)
                     if cp.stderr:
                         LOG.info(cp.stderr)
+                progress.update(task, completed=100, total=100)
         except Exception as e:
-            if task:
-                progress.update(task, completed=20, total=10, visible=False)
+            if not os.getenv("AT_DEBUG_MODE"):
+                LOG.info(
+                    "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
+                )
             LOG.error(e)
```

### Comparing `cpggen-0.8.0/cpggen/logger.py` & `cpggen-0.8.1/cpggen/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,11 +24,11 @@
             console=console, markup=True, show_path=False, enable_link_path=False
         )
     ],
 )
 LOG = logging.getLogger(__name__)
 
 # Set logging level
-if os.getenv("AT_DEBUG_MODE") == "debug":
+if os.getenv("AT_DEBUG_MODE") in ("debug", "true", "1"):
     LOG.setLevel(logging.DEBUG)
 
 DEBUG = logging.DEBUG
```

### Comparing `cpggen-0.8.0/cpggen/utils.py` & `cpggen-0.8.1/cpggen/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     "db_migrations",
     "unittests",
     "unittests_legacy",
     "stubs",
     "mock",
     "mocks",
     "vendor",
+    "instancemode-tests",
+    "integration-tests",
+    "oauth2-tests",
+    "twofactor-tests",
 ]
 
 ignore_files = [
     ".pyc",
     ".gz",
     ".tar",
     ".tar.gz",
@@ -200,14 +204,26 @@
     return find_files(search_dir, "go.mod", False, False)
 
 
 def find_makefiles(search_dir):
     return find_files(search_dir, "Makefile", False, False)
 
 
+def find_gradle_files(search_dir):
+    return find_files(search_dir, "build.gradle", False, False)
+
+
+def find_pom_files(search_dir):
+    return find_files(search_dir, "pom.xml", False, False)
+
+
+def find_sbt_files(search_dir):
+    return find_files(search_dir, "build.sbt", False, False)
+
+
 def check_command(cmd):
     """
     Method to check if command is available
     :return True if command is available in PATH. False otherwise
     """
     try:
         cpath = shutil.which(cmd, mode=os.F_OK | os.X_OK)
```

### Comparing `cpggen-0.8.0/pyproject.toml` & `cpggen-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "0.8.0"
+version = "0.8.1"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-0.8.0/PKG-INFO` & `cpggen-0.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 0.8.0
+Version: 0.8.1
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8,<3.12
@@ -70,23 +70,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - cpggen with Python 3.10
 - cdxgen with Node.js 18
 - cdxgen binary plugins
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.8.0/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.8.1/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v0.8.0/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v0.8.1/cpggen.exe
 .\cpggen.exe --help
 ```
 
 ### OCI Artifacts via ORAS cli
 
 Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
 
@@ -204,14 +204,15 @@
 | CPGGEN_CONTAINER_CPU    | CPU units to use in container execution mode. Default computed    |
 | CPGGEN_CONTAINER_MEMORY | Memory units to use in container execution mode. Default computed |
 | CPGGEN_MEMORY           | Heap memory to use for frontends. Default computed                |
 | AT_DEBUG_MODE           | Set to debug to enable debug logging                              |
 | CPG_EXPORT              | Set to true to export CPG graphs in dot format                    |
 | CPG_EXPORT_REPR         | Graph to export. Default all                                      |
 | CPG_EXPORT_FORMAT       | Export format. Default dot                                        |
+| SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI      |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
 - name: Upload cpg
```

