# Comparing `tmp/dapp-runner-0.1.0a1.tar.gz` & `tmp/dapp-runner-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapp-runner-0.1.0a1.tar", max compression
+gzip compressed data, was "dapp-runner-0.1.1.tar", max compression
```

## Comparing `dapp-runner-0.1.0a1.tar` & `dapp-runner-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     7652 2023-02-23 09:53:16.068012 dapp-runner-0.1.0a1/LICENSE
--rw-r--r--   0        0        0    10333 2023-02-23 09:53:16.068012 dapp-runner-0.1.0a1/README.md
--rw-r--r--   0        0        0       59 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/__init__.py
--rw-r--r--   0        0        0     3694 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/__main__.py
--rw-r--r--   0        0        0     3024 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/_util.py
--rw-r--r--   0        0        0      168 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/descriptor/__init__.py
--rw-r--r--   0        0        0     4687 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/descriptor/base.py
--rw-r--r--   0        0        0     1452 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/descriptor/config.py
--rw-r--r--   0        0        0     8510 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/descriptor/dapp.py
--rw-r--r--   0        0        0      948 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/descriptor/parser.py
--rw-r--r--   0        0        0     2577 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/log.py
--rw-r--r--   0        0        0     5407 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/runner/__init__.py
--rw-r--r--   0        0        0      116 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/runner/error.py
--rw-r--r--   0        0        0      743 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/runner/infile.py
--rw-r--r--   0        0        0      904 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/runner/payload.py
--rw-r--r--   0        0        0    14085 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/runner/runner.py
--rw-r--r--   0        0        0     5044 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/runner/service.py
--rw-r--r--   0        0        0     2295 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/runner/streams.py
--rw-r--r--   0        0        0      458 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/dapp_runner/singleton.py
--rw-r--r--   0        0        0     4893 2023-02-23 09:53:16.072012 dapp-runner-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0    11748 1970-01-01 00:00:00.000000 dapp-runner-0.1.0a1/setup.py
--rw-r--r--   0        0        0    11670 1970-01-01 00:00:00.000000 dapp-runner-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/LICENSE
+-rw-r--r--   0        0        0    10333 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/README.md
+-rw-r--r--   0        0        0       59 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/__init__.py
+-rw-r--r--   0        0        0     3694 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/__main__.py
+-rw-r--r--   0        0        0     3024 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/_util.py
+-rw-r--r--   0        0        0      168 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/descriptor/__init__.py
+-rw-r--r--   0        0        0     4687 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/descriptor/base.py
+-rw-r--r--   0        0        0     1452 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/descriptor/config.py
+-rw-r--r--   0        0        0     8510 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/descriptor/dapp.py
+-rw-r--r--   0        0        0      948 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/descriptor/parser.py
+-rw-r--r--   0        0        0     2576 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/log.py
+-rw-r--r--   0        0        0     5407 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/runner/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/runner/error.py
+-rw-r--r--   0        0        0      743 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/runner/infile.py
+-rw-r--r--   0        0        0      904 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/runner/payload.py
+-rw-r--r--   0        0        0    14085 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/runner/runner.py
+-rw-r--r--   0        0        0     5044 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/runner/service.py
+-rw-r--r--   0        0        0     2295 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/runner/streams.py
+-rw-r--r--   0        0        0      458 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/dapp_runner/singleton.py
+-rw-r--r--   0        0        0     4893 2023-04-11 16:32:12.927675 dapp-runner-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11750 1970-01-01 00:00:00.000000 dapp-runner-0.1.1/setup.py
+-rw-r--r--   0        0        0    11672 1970-01-01 00:00:00.000000 dapp-runner-0.1.1/PKG-INFO
```

### Comparing `dapp-runner-0.1.0a1/LICENSE` & `dapp-runner-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/README.md` & `dapp-runner-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/dapp_runner/__main__.py` & `dapp-runner-0.1.1/dapp_runner/__main__.py`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/dapp_runner/_util.py` & `dapp-runner-0.1.1/dapp_runner/_util.py`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/dapp_runner/descriptor/base.py` & `dapp-runner-0.1.1/dapp_runner/descriptor/base.py`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/dapp_runner/descriptor/config.py` & `dapp-runner-0.1.1/dapp_runner/descriptor/config.py`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/dapp_runner/descriptor/dapp.py` & `dapp-runner-0.1.1/dapp_runner/descriptor/dapp.py`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/dapp_runner/descriptor/parser.py` & `dapp-runner-0.1.1/dapp_runner/descriptor/parser.py`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/dapp_runner/log.py` & `dapp-runner-0.1.1/dapp_runner/log.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 """Python logging configuration for the `dapp-runner`."""
 import logging
 import warnings
 from typing import Optional
 
-from yapapi import __version__ as yapapi_version
-from yapapi.log import _YagnaDatetimeFormatter  # noqa
-
 logger = logging.getLogger(__name__)
 
 LOG_CRITICAL = "CRITICAL"
 LOG_FATAL = "FATAL"
 LOG_ERROR = "ERROR"
 LOG_WARN = "WARN"
 LOG_WARNING = "WARNING"
@@ -43,14 +40,16 @@
     format_: str = "[%(asctime)s %(levelname)s %(name)s] %(message)s",
 ):
     """Enable the logger.
 
     By default, it outputs `INFO` level logs to stderr and `DEBUG` level logs
     for `yapapi` and the REST APIs to the specified log file.
     """
+    from yapapi import __version__ as yapapi_version
+    from yapapi.log import _YagnaDatetimeFormatter
 
     api_log_level = api_log_level or file_log_level
 
     if enable_warnings:
         # capture only warnings coming from yapapi
         warnings.filterwarnings("once", module="yapapi")
         warnings.filterwarnings("once", module="dapp_runner")
```

### Comparing `dapp-runner-0.1.0a1/dapp_runner/runner/__init__.py` & `dapp-runner-0.1.1/dapp_runner/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/dapp_runner/runner/infile.py` & `dapp-runner-0.1.1/dapp_runner/runner/infile.py`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/dapp_runner/runner/payload.py` & `dapp-runner-0.1.1/dapp_runner/runner/payload.py`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/dapp_runner/runner/runner.py` & `dapp-runner-0.1.1/dapp_runner/runner/runner.py`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/dapp_runner/runner/service.py` & `dapp-runner-0.1.1/dapp_runner/runner/service.py`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/dapp_runner/runner/streams.py` & `dapp-runner-0.1.1/dapp_runner/runner/streams.py`

 * *Files identical despite different names*

### Comparing `dapp-runner-0.1.0a1/pyproject.toml` & `dapp-runner-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapp-runner"
-version = "0.1.0a1"
+version = "0.1.1"
 description = "Golem dapp-runner - a high-level interface for running decentralized applications using the Golem Network."
 authors = ["Golem Factory <contact@golem.network>"]
 license = "LGPL-3.0"
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Environment :: Console",
   "Intended Audience :: Developers",
@@ -28,15 +28,15 @@
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 appdirs = "^1.4"
 click = "^7.0"  # requires bump to goth's dependencies https://github.com/golemfactory/goth/issues/605
-dpath = "^2.0"
+dpath = "~2.0.8"
 pyyaml = "^5.0"  # requires bump to goth's dependencies https://github.com/golemfactory/goth/issues/605
 shortuuid = "^1.0"
 ansicolors = "^1.1.8"
 networkx = "^2.8"
 yapapi = "^0.10.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `dapp-runner-0.1.0a1/setup.py` & `dapp-runner-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['ansicolors>=1.1.8,<2.0.0',
  'appdirs>=1.4,<2.0',
  'click>=7.0,<8.0',
- 'dpath>=2.0,<3.0',
+ 'dpath>=2.0.8,<2.1.0',
  'networkx>=2.8,<3.0',
  'pyyaml>=5.0,<6.0',
  'shortuuid>=1.0,<2.0',
  'yapapi>=0.10.0,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['dapp-runner = dapp_runner.__main__:_cli']}
 
 setup_kwargs = {
     'name': 'dapp-runner',
-    'version': '0.1.0a1',
+    'version': '0.1.1',
     'description': 'Golem dapp-runner - a high-level interface for running decentralized applications using the Golem Network.',
     'long_description': '# Golem dApp Runner\n\n`dapp-runner` is a utility that allows you to run decentralized applications on [Golem](https://www.golem.network/).\nIt uses simple application descriptors expressed in `yaml`, similar to those used by\ntools like `docker-compose`.\n\n`dapp-runner` runs alongside the [Golem daemon](https://github.com/golemfactory/yagna)\nand uses [yapapi](https://github.com/golemfactory/yapapi), Golem\'s Python high-level API\nto communicate with it. As opposed to using plain `yapapi` though, deployment of\napplications on Golem using `dapp-runner` requires no code and no experience in Python.\n\n### GAP-16 / Multi-service application deployment framework\n\nIn its present form, the `dapp-runner` constitutes an initial reference implementation\nof the multi-service application deployment framework described in\n[GAP-16](https://github.com/golemfactory/golem-architecture/pull/39).\n\nFollowing features of the framework are currently supported:\n\n* Descriptor "Apply" operation\n* Single-YAML package support\n* Merging descriptor files\n* GAOM explicit dependency syntax\n* GAOM object dependency graph *[currently limited to the services\' explicit dependency syntax]*\n\n### Relationship with `dapp-manager`\n\nWhile the `dapp-runner` is perfectly capable of running decentralized apps on its own, we are also\nproviding a separate tool to facilitate running and managing multiple applications on a single\nmachine, namely, the [dapp-manager](https://github.com/golemfactory/dapp-manager/).\n\ndApp Manager keeps track of the launched apps and allows you to easily query their output streams.\nIt uses the `dapp-runner` as its back-end and both require the yagna daemon to communicate with the\nrest of the Golem Network.\n\n## Quick start\n\n### Yagna daemon\n\nTo run Golem apps, `dapp-runner` requires a properly configured yagna daemon.\nIn the future, you\'ll be able to provision apps using external supervisor machines\nwhich will run a yagna daemon on your behalf.\n\nFor now, please follow the ["Requestor development: a quick primer"](https://handbook.golem.network/requestor-tutorials/flash-tutorial-of-requestor-development)\ntutorial and ensure that your `yagna` is up and running. Only the first part of this\ntutorial is required - you don\'t need to run the blender example.\n\nMost importantly, make sure you have set the `YAGNA_APPKEY` in your evironment, e.g. with:\n\n```bash\nexport YAGNA_APPKEY=insert-your-32-char-app-key-here\n```\n\nor, on Windows:\n\n```bash\nset YAGNA_APPKEY=insert-your-32-char-app-key-here\n```\n\nand if you don\'t know what your app-key is, you can always query `yagna` with:\n\n```bash\nyagna app-key list\n```\n\n### Python environment\n\nFirst, ensure you have Python 3.8 or later:\n\n```bash\npython3 --version\n```\n\n[ depending on the platform, it may be just `python` instead of `python3` ]\n\nIf your Python version is older, consider using [pyenv](https://github.com/pyenv/pyenv-installer).\n\nOnce your python interpreter reports a version 3.8 or later, you can set-up your virtual\nenvironment:\n\n```bash\npython3 -m venv ~/.envs/dapp-runner\nsource ~/.envs/dapp-runner/bin/activate\n```\n\nor, if you\'re on Windows:\n\n```shell\npython -m venv --clear %HOMEDRIVE%%HOMEPATH%\\.envs\\dapp-runner\n%HOMEDRIVE%%HOMEPATH%\\.envs\\dapp-runner\\Scripts\\activate.bat\n```\n\n### DApp runner\n\n#### Clone the repository\n\n```bash\ngit clone --recurse-submodules https://github.com/golemfactory/dapp-runner.git\n```\n\n#### Install the dependencies\n\n```bash\ncd dapp-runner\npip install -U pip poetry\npoetry install\n```\n\n#### Run an example application\n\nMake sure your `yagna` daemon is running,\nyou have initialized the payment driver with `yagna payment init --sender`,\nand that you have set the `YAGNA_APPKEY` environment variable.\n\nThen run:\n\n```bash\ndapp-runner start --config configs/default.yaml dapp-store/apps/webapp.yaml\n```\n\nYou should see the application being deployed on the Golem Network and once it\'s up,\nyou\'ll be greeted with:\n\n```shell\n{"http": {"local_proxy_address": "http://localhost:8080"}}\n```\n\nYou can connect to [this address](http://localhost:8080) using your local browser,\nand you\'ll see our minimalistic web application example running.\n\nPress Ctrl-C in the terminal where you ran `dapp-runner` to initiate its shutdown.\n\n## Application descriptor\n\nAs mentioned above, the decentralized applications that are deployed on Golem by the\n`dapp-runner` are described in `yaml` files, conforming to the schema\ndescribed in [GAP-16](https://github.com/golemfactory/golem-architecture/pull/39).\n\n### Example descriptor\n\nHere\'s an example application descriptor (`http-proxy.yaml`), that provisions a single\ninstance of a simple, static website served with `nginx`:\n\n```yaml\npayloads:\n  nginx:\n    runtime: "vm"\n    params:\n      image_hash: "16ad039c00f60a48c76d0644c96ccba63b13296d140477c736512127"\nnodes:\n  http:\n    payload: "nginx"\n    init:\n        - ["/docker-entrypoint.sh"]\n        - ["/bin/chmod", "a+x", "/"]\n        - ["/bin/sh", "-c", \'echo "Hello from inside Golem!" > /usr/share/nginx/html/index.html\']\n        - ["/bin/rm", "/var/log/nginx/access.log", "/var/log/nginx/error.log"]\n        - ["/usr/sbin/nginx"]\n    http_proxy:\n      ports:\n        - "80"  # specify just the remote port, allow the local port to be automatically chosen\n```\n\n#### Web application\n\nAnd here\'s an example of a slightly more complex application (`webapp.yaml`), that uses\ntwo kinds of services and explicitly connects them within a specified network:\n\n```yaml\npayloads:\n  db:\n    runtime: "vm"\n    params:\n      image_hash: "85021afecf51687ecae8bdc21e10f3b11b82d2e3b169ba44e177340c"\n  http:\n    runtime: "vm"\n    params:\n      image_hash: "c37c1364f637c199fe710ca62241ff486db92c875b786814c6030aa1"\nnodes:\n  db:\n    payload: "db"\n    init:\n      - ["/bin/run_rqlite.sh"]\n    network: "default"\n    ip:\n      - "192.168.0.2"\n  http:\n    payload: "http"\n    init:\n      - ["/bin/bash", "-c", "cd /webapp && python app.py --db-address 192.168.0.2 --db-port 4001 initdb"]\n      - ["/bin/bash", "-c", "cd /webapp && python app.py --db-address 192.168.0.2 --db-port 4001 run > /webapp/out 2> /webapp/err &"]\n    http_proxy:\n      ports:\n        - "5000"  # specify just the remote port, allow the local port to be automatically chosen\n    network: "default"\n    ip:\n      - "192.168.0.3"\n    depends_on:\n      - "db"\nnetworks:\n  default:\n    ip: "192.168.0.0/24"\n```\n\n#### Implicit properties\n\n##### The `networks` definition and the `vpn` capability\n\nAs can be seen in the `http_proxy` example above, the `networks` definition can be omitted.\n\nAdding a `http_proxy` element to a `nodes` entry, causes the `dapp-runner` to implicitly\nadd the `networks` object with a default of a single IPv4 network. Additionally, it adds\nthe `vpn` capability to the requested parameters of the deployed `vm` runtime.\n\n***Note:*** The `networks` and `capabilities` objects will only be implicitly added if\nthey are not already present in the descriptor. If the application specifies any of\nthose objects, it is assumed that the application authors know what they\'re doing.\n\n##### The `manifest-support` capability\n\nSimilarly, specifying the payload as `vm/manifest` implicitly adds `manifest-support` to\nthe requested `capabilities` for the runtime.\n\n***Note:*** Again, this is only done if the `payload.params` doesn\'t already contain the\n`capabilities` object.\n\n## Usage\n\nCurrently, the `dapp-runner` implements a single CLI command, `start`:\n\n```shell\nUsage: dapp-runner start [OPTIONS] DESCRIPTORS...\n```\n\nwhich allows the following options:\n\n```shell\n  -d, --data PATH    Path to the data file.\n  -l, --log PATH     Path to the log file.\n  -s, --state PATH   Path to the state file.\n  --stdout PATH      Redirect stdout to the specified file.\n  --stderr PATH      Redirect stderr to the specified file.\n  -c, --config PATH  Path to the file containing yagna-specific config.\n                     [required]\n  --silent\n  --help             Show this message and exit.\n```\n\nThe `--data`, `--log`, `--state`, `--stdout`, and `--stderr` arguments specify the\nlocations of files to which the respective streams are written. If unspecified, all\nstreams are written to the console which the `dapp-runner` is invoked from.\n\n### Streams\n\n#### Data\n\nThe `data` stream consists of JSON-formatted output of specific components that are run\nas part of the services. Currently it carries the command execution events from\nexescript commands, e.g.:\n\n```json\n{"db": {"0": [{"command": {"run": {"entry_point": "/bin/run_rqlite.sh", "args": [], "capture": {"stdout": {"stream": {}}, "stderr": {"stream": {}}}}}, "success": true, "stdout": null, "stderr": null}]}}\n```\n\nand the parameters of any started instances of Local HTTP proxies:\n\n```json\n{"http": {"local_proxy_address": "http://localhost:8080"}}\n```\n\nThe keys in the outermost dictionaries refer to names of service cluster as specified in\nthe `yaml` descriptor file. For exescript commands, the secondary layer\'s keys refer to\nindices of instances within the specific cluster.\n\n#### State\n\nThe `state` stream consists of JSON-formatted descriptions of the state of the dapp\nafter each state change, e.g.:\n\n```json\n{"db": {"0": "running"}, "http": {"0": "starting"}}\n```\n\nHere, again, the keys in the topmost dictionary refer to the names of service clusters\ndefined in the `yaml` descriptor file and the secondary layer\'s keys refer to indices\nof specific instances.\n\n#### Log\n\nThe `log` stream is a text stream of log messages emitted from `dapp-runner`.\n\n#### Stdout / Stderr\n\nFinally, `stdout` and `stderr` refer to the standard output streams of the `dapp-runner`\nscript.\n\n### Config\n\nThis is a mandatory argument, specifying a path to a `yaml` file containing a\ndescription of a configuration to connect to your `yagna` daemon, e.g.:\n\n```yaml\nyagna:\n  app_key: "$YAGNA_APPKEY"\n  subnet_tag: "devnet-beta"\n\npayment:\n  budget: 1.0  # GLM\n  driver: "erc20"\n  network: "rinkeby"\n```\n\n### Descriptors\n\nOne or more application descriptors, as specified in the\n["Application descriptor"](#application-descriptor) section above.\n\nIf more than one `yaml` descriptor file is given, all of the `yaml` files are merged\ninto one descriptor before being processed further by the `dapp-runner`. The files\nare merged using a deep-merge strategy with contents of each subsequent `yaml` file\noverriding the colliding keys of the former ones.\n',
     'author': 'Golem Factory',
     'author_email': 'contact@golem.network',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/golemfactory/dapp-runner',
```

### Comparing `dapp-runner-0.1.0a1/PKG-INFO` & `dapp-runner-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapp-runner
-Version: 0.1.0a1
+Version: 0.1.1
 Summary: Golem dapp-runner - a high-level interface for running decentralized applications using the Golem Network.
 Home-page: https://github.com/golemfactory/dapp-runner
 License: LGPL-3.0
 Author: Golem Factory
 Author-email: contact@golem.network
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Distributed Computing
 Requires-Dist: ansicolors (>=1.1.8,<2.0.0)
 Requires-Dist: appdirs (>=1.4,<2.0)
 Requires-Dist: click (>=7.0,<8.0)
-Requires-Dist: dpath (>=2.0,<3.0)
+Requires-Dist: dpath (>=2.0.8,<2.1.0)
 Requires-Dist: networkx (>=2.8,<3.0)
 Requires-Dist: pyyaml (>=5.0,<6.0)
 Requires-Dist: shortuuid (>=1.0,<2.0)
 Requires-Dist: yapapi (>=0.10.0,<0.11.0)
 Project-URL: Repository, https://github.com/golemfactory/dapp-runner
 Description-Content-Type: text/markdown
```

