# Comparing `tmp/nbdefense_jupyter-1.0.2.tar.gz` & `tmp/nbdefense_jupyter-1.0.3.tar.gz`

## Comparing `nbdefense_jupyter-1.0.2.tar` & `nbdefense_jupyter-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/package.json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/_version.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/handlers.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/package.json
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/package.json.orig
--rw-r--r--   0        0        0    16110 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/plugin.json
--rw-r--r--   0        0        0    51556 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/117.e6844c28c0311e09d7d5.js
--rw-r--r--   0        0        0    13996 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/239.1c003b0dfd58bc7823a8.js
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/355.e71f4acc9570680d68e9.js
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/452.26450d70ddf6735bc3a7.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/452.26450d70ddf6735bc3a7.js.LICENSE.txt
--rw-r--r--   0        0        0   157457 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/500.97d1a5336e530d36f1c4.js
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/502.ab49aeea7a0fb1ad88e8.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/502.ab49aeea7a0fb1ad88e8.js.LICENSE.txt
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/654.0b96d4d60115144c75b2.js
--rw-r--r--   0        0        0    18496 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/676.6137834929c84786225d.js
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/747.5ffca1b512bb6d3e1574.js
--rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/remoteEntry.5411c638713e214194c0.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/style.js
--rw-r--r--   0        0        0    12463 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/.gitignore
--rw-r--r--   0        0        0    10754 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/LICENSE
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/README.md
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    17166 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/package.json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/_version.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/handlers.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/package.json
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/package.json.orig
+-rw-r--r--   0        0        0    16110 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/plugin.json
+-rw-r--r--   0        0        0    51556 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/117.e6844c28c0311e09d7d5.js
+-rw-r--r--   0        0        0    13996 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/239.1c003b0dfd58bc7823a8.js
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/355.e71f4acc9570680d68e9.js
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/452.26450d70ddf6735bc3a7.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/452.26450d70ddf6735bc3a7.js.LICENSE.txt
+-rw-r--r--   0        0        0   157457 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/500.97d1a5336e530d36f1c4.js
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/502.ab49aeea7a0fb1ad88e8.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/502.ab49aeea7a0fb1ad88e8.js.LICENSE.txt
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/654.0b96d4d60115144c75b2.js
+-rw-r--r--   0        0        0    18496 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/676.6137834929c84786225d.js
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/747.5ffca1b512bb6d3e1574.js
+-rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/remoteEntry.a4d194721ddf3be27f37.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/style.js
+-rw-r--r--   0        0        0    12463 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/.gitignore
+-rw-r--r--   0        0        0    10754 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/README.md
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    15877 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/PKG-INFO
```

### Comparing `nbdefense_jupyter-1.0.2/package.json` & `nbdefense_jupyter-1.0.3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'1.0.3'"}*

```diff
@@ -139,9 +139,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.2"
+    "version": "1.0.3"
 }
```

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/__init__.py` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/handlers.py` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/handlers.py`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/package.json` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9758597883597885%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.a4d194721ddf3be27f37.js'}}",*

 * * "'version'": "'1.0.3'"}*

```diff
@@ -68,15 +68,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.5411c638713e214194c0.js",
+            "load": "static/remoteEntry.a4d194721ddf3be27f37.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "nbdefense_jupyter"
                 },
@@ -144,9 +144,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.2"
+    "version": "1.0.3"
 }
```

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/package.json.orig` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'1.0.3'"}*

```diff
@@ -139,9 +139,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.2"
+    "version": "1.0.3"
 }
```

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/plugin.json` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/plugin.json`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/117.e6844c28c0311e09d7d5.js` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/117.e6844c28c0311e09d7d5.js`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/239.1c003b0dfd58bc7823a8.js` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/239.1c003b0dfd58bc7823a8.js`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/452.26450d70ddf6735bc3a7.js` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/452.26450d70ddf6735bc3a7.js`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/500.97d1a5336e530d36f1c4.js` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/500.97d1a5336e530d36f1c4.js`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/502.ab49aeea7a0fb1ad88e8.js` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/502.ab49aeea7a0fb1ad88e8.js`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/676.6137834929c84786225d.js` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/676.6137834929c84786225d.js`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/747.5ffca1b512bb6d3e1574.js` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/747.5ffca1b512bb6d3e1574.js`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/remoteEntry.5411c638713e214194c0.js` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/remoteEntry.a4d194721ddf3be27f37.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -123,15 +123,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (u("date-fns", "2.29.3", (() => w.e(500).then((() => () => w(500))))), u("nbdefense-jupyter", "1.0.2", (() => Promise.all([w.e(239), w.e(271), w.e(117)]).then((() => () => w(117))))), u("react-animate-height", "0", (() => Promise.all([w.e(271), w.e(452)]).then((() => () => w(452))))), u("react-use-websocket", "3.0.0", (() => Promise.all([w.e(676), w.e(271)]).then((() => () => w(676))))), u("use-event-callback", "0.1.0", (() => Promise.all([w.e(271), w.e(355)]).then((() => () => w(355)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("date-fns", "2.29.3", (() => w.e(500).then((() => () => w(500))))), u("nbdefense-jupyter", "1.0.3", (() => Promise.all([w.e(239), w.e(271), w.e(117)]).then((() => () => w(117))))), u("react-animate-height", "0", (() => Promise.all([w.e(271), w.e(452)]).then((() => () => w(452))))), u("react-use-websocket", "3.0.0", (() => Promise.all([w.e(676), w.e(271)]).then((() => () => w(676))))), u("use-event-callback", "0.1.0", (() => Promise.all([w.e(271), w.e(355)]).then((() => () => w(355)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `nbdefense_jupyter-1.0.2/nbdefense_jupyter/labextension/static/third-party-licenses.json` & `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.2/.gitignore` & `nbdefense_jupyter-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.2/LICENSE` & `nbdefense_jupyter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.2/pyproject.toml` & `nbdefense_jupyter-1.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,15 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
-dependencies = [
-    "nbdefense==1.0.3"
-]
+dependencies = ["nbdefense==1.0.4"]
 dynamic = ["version", "description", "authors", "urls", "keywords"]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 dev = ["black==22.8.0", "pre-commit==2.20.0", "jupyterlab>=3.1,<4.0.0"]
 
 [tool.hatch.version]
```

### Comparing `nbdefense_jupyter-1.0.2/PKG-INFO` & `nbdefense_jupyter-1.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdefense_jupyter
-Version: 1.0.2
+Version: 1.0.3
 Summary: NB Defense Jupyter Lab Extension
 Project-URL: Homepage, https://protectai.com
 Project-URL: Bug Tracker, https://protectai.com/contact-us
 Project-URL: Repository, https://github.com/protectai/nbdefense-jupyter.git
 Author-email: ProtectAI <support@protectai.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -205,140 +205,52 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.7.1
-Requires-Dist: nbdefense==1.0.3
+Requires-Dist: nbdefense==1.0.4
 Provides-Extra: dev
 Requires-Dist: black==22.8.0; extra == 'dev'
 Requires-Dist: jupyterlab<4.0.0,>=3.1; extra == 'dev'
 Requires-Dist: pre-commit==2.20.0; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
-# nbdefense_jupyter
+# 🛡️ NB Defense Jupyter Lab Extension
 
-The NBDefense Jupyter extension
+[![Build](https://github.com/protectai/nbdefense-jupyter/actions/workflows/build.yml/badge.svg)](https://github.com/protectai/nbdefense-jupyter/actions/workflows/build.yml)
+[![Test](https://github.com/protectai/nbdefense-jupyter/actions/workflows/test.yml/badge.svg)](https://github.com/protectai/nbdefense-jupyter/actions/workflows/test.yml)
+[![License: Apache 2.0](https://img.shields.io/crates/l/apa)](https://opensource.org/license/apache-2-0/)
 
-This extension is composed of a Python package named `nbdefense_jupyter`
-for the server extension and a NPM package named `nbdefense-jupyter`
-for the frontend extension.
-
-## Requirements
-
-- JupyterLab >= 3.0
-
-## Install
-
-To install the extension, execute:
+## 🏃‍♀️ Quick Start
 
 ```bash
 pip install nbdefense_jupyter
-```
-
-If you are planning on using the PII module you will need to install `en_core_web_trf`
-
-```bash
-python -m spacy download en_core_web_trf
-```
-
-Enable the extension
-
-```bash
 jupyter server extension enable nbdefense_jupyter
 ```
 
-Start (or restart) the Jupyter Lab Server
+## 🙋‍♂️ What is the NB Defense Jupyter Lab Extension?
 
-```bash
-jupyter lab
-```
+Brought to you by Protect AI, NB Defense Jupyter Lab Extension (JLE) is an open source tool that encourages you to think about security throughout every step of your machine learning development process. You can use nbdefense to scan for [Secrets](https://nbdefense.ai/supported-scans/detecting-secrets), [Personally Identifiable Information (PII)](https://nbdefense.ai/supported-scans/detecting-PII), [Common Vulnerabilities and Exposures(CVE)](https://nbdefense.ai/supported-scans/detecting-CVEs), and [Licenses](https://nbdefense.ai/supported-scans/detecting-licenses) in your notebook files.
 
-## Uninstall
+The NB Defense Jupyter Lab Extension depends on our [CLI/SDK](https://github.com/protectai/nbdefense) repository Visit our [documentation](https://nbdefense.ai), or the repository below to learn more.
 
-To remove the extension, execute:
-
-```bash
-pip uninstall nbdefense_jupyter
-```
+- [NB Defense Repository](https://github.com/protectai/nbdefense)
 
-## Troubleshoot
+## 📄 Documentation
 
-If you are seeing the frontend extension, but it is not working, check
-that the server extension is enabled:
+For more details and [documentation](https://nbdefense.ai) visit these links:
 
-```bash
-jupyter server extension list
-```
+- [Documentation](https://nbdefense.ai)
 
-If the server extension is installed and enabled, but you are not seeing
-the frontend extension, check the frontend extension is installed:
+- [Getting Started on a Local Machine](https://nbdefense.ai/getting-started/jupyter-lab-extension)
+- [Getting Started on with Cloud Services](https://nbdefense.ai/getting-started/cloud-services)
 
-```bash
-jupyter labextension list
-```
+## 💪 Contributing
 
-## Contributing
-
-### Development install
-
-Note: You will need NodeJS to build the extension package.
-
-The `jlpm` command is JupyterLab's pinned version of
-[yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
-`yarn` or `npm` in lieu of `jlpm` below.
-
-```bash
-# Clone the repo to your local environment
-# Change directory to the nbdefense_jupyter directory
-# Install package in development mode
-pip install -e .
-# Link your development version of the extension with JupyterLab
-jupyter labextension develop . --overwrite
-# Server extension must be manually installed in develop mode
-jupyter server extension enable nbdefense_jupyter
-# Rebuild extension Typescript source after making changes
-jlpm build
-```
-
-You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
-
-```bash
-# Watch the source directory in one terminal, automatically rebuilding when needed
-jlpm watch
-# Run JupyterLab in another terminal
-jupyter lab
-```
-
-With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
-
-By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
-
-```bash
-jupyter lab build --minimize=False
-```
-
-### Development uninstall
-
-```bash
-# Server extension must be manually disabled in develop mode
-jupyter server extension disable nbdefense_jupyter
-pip uninstall nbdefense_jupyter
-```
+Welcome to the team! We are open to contributions and working with the community to make notebooks safer for everyone.
 
-In development mode, you will also need to remove the symlink created by `jupyter labextension develop`
-command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
-folder is located. Then you can remove the symlink named `nbdefense-jupyter` within that folder.
-
-### Updating the nbdefense dependency
-
-> **Note:** We should automate this process in the future
-
-1. Download the new release's wheel file from the S3 bucket
-2. Rename the release to follow this format: `nbdefense-{VERSION}-py2.py3-none-any.whl`
-3. Copy the file to the `nbdefense_cli` directory
-4. Update the dependency in the `pyproject.toml` file to match the new filename
-5. Re-run `pip install -e .`
+If you would like to contribute, please visit [CONTRIBUTING.md](https://github.com/protectai/nbdefense-jupyter/blob/main/CONTRIBUTING.md) to get started as a developer, or to suggest bug fixes, improvements, or new features follow [this link](https://nbdefense.ai/faq) to our FAQ page.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

