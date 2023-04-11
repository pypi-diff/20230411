# Comparing `tmp/fastapi-key-auth-0.8.0.tar.gz` & `tmp/fastapi_key_auth-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-key-auth-0.8.0.tar", max compression
+gzip compressed data, was "fastapi_key_auth-0.9.0.tar", max compression
```

## Comparing `fastapi-key-auth-0.8.0.tar` & `fastapi_key_auth-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2022-09-30 19:05:46.837852 fastapi-key-auth-0.8.0/LICENSE
--rw-r--r--   0        0        0      113 2022-10-31 17:33:57.516610 fastapi-key-auth-0.8.0/fastapi_key_auth/__init__.py
--rw-r--r--   0        0        0       45 2022-09-30 19:05:46.838882 fastapi-key-auth-0.8.0/fastapi_key_auth/dependency/__init__.py
--rw-r--r--   0        0        0      706 2022-10-31 17:32:48.200273 fastapi-key-auth-0.8.0/fastapi_key_auth/dependency/authorizer.py
--rw-r--r--   0        0        0       45 2022-09-30 19:05:46.839750 fastapi-key-auth-0.8.0/fastapi_key_auth/middleware/__init__.py
--rw-r--r--   0        0        0     2734 2022-10-31 17:25:58.118211 fastapi-key-auth-0.8.0/fastapi_key_auth/middleware/authorizer.py
--rw-r--r--   0        0        0     1439 2022-10-31 17:33:57.516743 fastapi-key-auth-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2674 2022-09-30 19:05:46.843490 fastapi-key-auth-0.8.0/readme.md
--rw-r--r--   0        0        0     3560 1970-01-01 00:00:00.000000 fastapi-key-auth-0.8.0/setup.py
--rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 fastapi-key-auth-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-09-30 19:05:46.837852 fastapi_key_auth-0.9.0/LICENSE
+-rw-r--r--   0        0        0      113 2023-02-15 09:00:46.976313 fastapi_key_auth-0.9.0/fastapi_key_auth/__init__.py
+-rw-r--r--   0        0        0       45 2022-09-30 19:05:46.838882 fastapi_key_auth-0.9.0/fastapi_key_auth/dependency/__init__.py
+-rw-r--r--   0        0        0      706 2022-11-01 06:50:51.926069 fastapi_key_auth-0.9.0/fastapi_key_auth/dependency/authorizer.py
+-rw-r--r--   0        0        0       45 2022-09-30 19:05:46.839750 fastapi_key_auth-0.9.0/fastapi_key_auth/middleware/__init__.py
+-rw-r--r--   0        0        0     2734 2022-10-31 17:25:58.118211 fastapi_key_auth-0.9.0/fastapi_key_auth/middleware/authorizer.py
+-rw-r--r--   0        0        0     1462 2023-02-15 09:00:46.976451 fastapi_key_auth-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2676 2023-02-15 08:55:39.147416 fastapi_key_auth-0.9.0/readme.md
+-rw-r--r--   0        0        0     3563 1970-01-01 00:00:00.000000 fastapi_key_auth-0.9.0/setup.py
+-rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 fastapi_key_auth-0.9.0/PKG-INFO
```

### Comparing `fastapi-key-auth-0.8.0/LICENSE` & `fastapi_key_auth-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-key-auth-0.8.0/fastapi_key_auth/dependency/authorizer.py` & `fastapi_key_auth-0.9.0/fastapi_key_auth/dependency/authorizer.py`

 * *Files identical despite different names*

### Comparing `fastapi-key-auth-0.8.0/fastapi_key_auth/middleware/authorizer.py` & `fastapi_key_auth-0.9.0/fastapi_key_auth/middleware/authorizer.py`

 * *Files identical despite different names*

### Comparing `fastapi-key-auth-0.8.0/pyproject.toml` & `fastapi_key_auth-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [tool.poetry]
 name = "fastapi-key-auth"
-version = "0.8.0"
+version = "0.9.0"
 description = "API key validation Middleware"
 authors = ["Benjamin Ramser <legionaerr@googlemail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/iwpnd/fastapi-key-auth"
 repository = "https://github.com/iwpnd/fastapi-key-auth"
 keywords = ["tile38", "async", "client"]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
-fastapi = ">=0.70.0,<0.87.0"
-starlette = "^0.19.0"
+fastapi = ">=0.84.0,<=0.92.0"
+starlette = "^0.25.0"
 
-[tool.poetry.dev-dependencies]
+
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
-pre-commit = "^2.20.0"
-black = "^22.10"
-gitlint = "^0.17.0"
-poethepoet = "^0.16.4"
-isort = "^5.10.1"
+pre-commit = "^2.21.0"
+black = "^23.1"
+gitlint = "^0.18.0"
+poethepoet = "^0.18.1"
+isort = "^5.11.5"
 pytest-cov = "^4.0.0"
 flake8 = "^5.0.4"
-requests = "^2.28.1"
-mypy = "^0.982"
-python-semantic-release = "^7.32.2"
+requests = "^2.28.2"
+mypy = "^1.0"
+python-semantic-release = "^7.33.1"
+httpx = "^0.23.3"
 
 [mypy]
 python_version = 3.7
 ignore_missing_imports = true
 
 
 [tool.semantic_release]
```

### Comparing `fastapi-key-auth-0.8.0/readme.md` & `fastapi_key_auth-0.9.0/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -74,18 +74,18 @@
 
 ```python
 from fastapi import FastAPI
 from fastapi_key_auth import AuthorizerMiddleware
 
 app = FastAPI()
 
-app.add_middleware(AuthorizerMiddleware, public_path=["/ping"], key_pattern="API_KEY_")
+app.add_middleware(AuthorizerMiddleware, public_paths=["/ping"], key_pattern="API_KEY_")
 
 # optional use regex startswith
-app.add_middleware(AuthorizerMiddleware, public_path=["/ping", "^/users"])
+app.add_middleware(AuthorizerMiddleware, public_paths=["/ping", "^/users"])
 ```
 
 As Dependency
 
 ```python
 from fastapi import FastAPI, Depends
 from fastapi_key_auth import AuthorizerDependency
```

#### html2text {}

```diff
@@ -19,16 +19,16 @@
 ### Built With - [starlette](https://github.com/encode/starlette) - [fastapi]
 (https://github.com/tiangolo/fastapi)  ## Getting Started ### Installation 1.
 Clone and install ```sh git clone https://github.com/iwpnd/fastapi-key-auth.git
 poetry install ``` 2. Install with pip ```sh pip install fastapi-key-auth ```
 3. Install with poetry ```sh poetry add fastapi-key-auth ``` ## Usage As
 Middleware: ```python from fastapi import FastAPI from fastapi_key_auth import
 AuthorizerMiddleware app = FastAPI() app.add_middleware(AuthorizerMiddleware,
-public_path=["/ping"], key_pattern="API_KEY_") # optional use regex startswith
-app.add_middleware(AuthorizerMiddleware, public_path=["/ping", "^/users"]) ```
+public_paths=["/ping"], key_pattern="API_KEY_") # optional use regex startswith
+app.add_middleware(AuthorizerMiddleware, public_paths=["/ping", "^/users"]) ```
 As Dependency ```python from fastapi import FastAPI, Depends from
 fastapi_key_auth import AuthorizerDependency authorizer = AuthorizerDependency
 (key_pattern="API_KEY_") # either globally or in a router app = FastAPI
 (dependencies=[Depends(authorizer)]) ``` ## License Distributed under the MIT
 License. See `LICENSE` for more information.  ## Contact Benjamin Ramser -
 [@imwithpanda](https://twitter.com/imwithpanda) - ahoi@iwpnd.pw Project Link:
 [https://github.com/iwpnd/fastapi-key-auth](https://github.com/iwpnd/fastapi-
```

### Comparing `fastapi-key-auth-0.8.0/setup.py` & `fastapi_key_auth-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
  'fastapi_key_auth.dependency',
  'fastapi_key_auth.middleware']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fastapi>=0.70.0,<0.87.0', 'starlette>=0.19.0,<0.20.0']
+['fastapi>=0.84.0,<=0.92.0', 'starlette>=0.25.0,<0.26.0']
 
 setup_kwargs = {
     'name': 'fastapi-key-auth',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'API key validation Middleware',
-    'long_description': '<br />\n<p align="center">\n  <h3 align="center">FastAPI-key-auth</h3>\n\n  <p align="center">\n    Secure your FastAPI endpoints using API keys.\n    <br />\n    <a href="https://github.com/iwpnd/fastapi-key-auth/issues">Report Bug</a>\n    ·\n    <a href="https://github.com/iwpnd/fastapi-key-auth/issues">Request Feature</a>\n  </p>\n</p>\n\n<!-- TABLE OF CONTENTS -->\n<details open="open">\n  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>\n  <ol>\n    <li>\n      <a href="#about-the-project">About The Project</a>\n      <ul>\n        <li><a href="#built-with">Built With</a></li>\n      </ul>\n    </li>\n    <li>\n      <a href="#getting-started">Getting Started</a>\n      <ul>\n        <li><a href="#installation">Installation</a></li>\n      </ul>\n    </li>\n    <li><a href="#usage">Usage</a></li>\n    <li><a href="#license">License</a></li>\n    <li><a href="#contact">Contact</a></li>\n  </ol>\n</details>\n\n<!-- ABOUT THE PROJECT -->\n\n## About The Project\n\nOn deployment inject API keys authorized to use your service. Every call to a private\nendpoint of your service has to include a `header[\'x-api-key\']` attribute that is\nvalidated against the API keys in your environment.\nIf it is present, a request is authorized. If it is not FastAPI return `401 Unauthorized`.\nUse this either as a middleware, or as Dependency.\n\n### Built With\n\n-   [starlette](https://github.com/encode/starlette)\n-   [fastapi](https://github.com/tiangolo/fastapi)\n\n<!-- GETTING STARTED -->\n\n## Getting Started\n\n### Installation\n\n1. Clone and install\n    ```sh\n    git clone https://github.com/iwpnd/fastapi-key-auth.git\n    poetry install\n    ```\n2. Install with pip\n    ```sh\n    pip install fastapi-key-auth\n    ```\n3. Install with poetry\n    ```sh\n    poetry add fastapi-key-auth\n    ```\n\n## Usage\n\nAs Middleware:\n\n```python\nfrom fastapi import FastAPI\nfrom fastapi_key_auth import AuthorizerMiddleware\n\napp = FastAPI()\n\napp.add_middleware(AuthorizerMiddleware, public_path=["/ping"], key_pattern="API_KEY_")\n\n# optional use regex startswith\napp.add_middleware(AuthorizerMiddleware, public_path=["/ping", "^/users"])\n```\n\nAs Dependency\n\n```python\nfrom fastapi import FastAPI, Depends\nfrom fastapi_key_auth import AuthorizerDependency\n\nauthorizer = AuthorizerDependency(key_pattern="API_KEY_")\n\n# either globally or in a router\napp = FastAPI(dependencies=[Depends(authorizer)])\n```\n\n## License\n\nDistributed under the MIT License. See `LICENSE` for more information.\n\n<!-- CONTACT -->\n\n## Contact\n\nBenjamin Ramser - [@imwithpanda](https://twitter.com/imwithpanda) - ahoi@iwpnd.pw  \nProject Link: [https://github.com/iwpnd/fastapi-key-auth](https://github.com/iwpnd/fastapi-key-auth)\n',
+    'long_description': '<br />\n<p align="center">\n  <h3 align="center">FastAPI-key-auth</h3>\n\n  <p align="center">\n    Secure your FastAPI endpoints using API keys.\n    <br />\n    <a href="https://github.com/iwpnd/fastapi-key-auth/issues">Report Bug</a>\n    ·\n    <a href="https://github.com/iwpnd/fastapi-key-auth/issues">Request Feature</a>\n  </p>\n</p>\n\n<!-- TABLE OF CONTENTS -->\n<details open="open">\n  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>\n  <ol>\n    <li>\n      <a href="#about-the-project">About The Project</a>\n      <ul>\n        <li><a href="#built-with">Built With</a></li>\n      </ul>\n    </li>\n    <li>\n      <a href="#getting-started">Getting Started</a>\n      <ul>\n        <li><a href="#installation">Installation</a></li>\n      </ul>\n    </li>\n    <li><a href="#usage">Usage</a></li>\n    <li><a href="#license">License</a></li>\n    <li><a href="#contact">Contact</a></li>\n  </ol>\n</details>\n\n<!-- ABOUT THE PROJECT -->\n\n## About The Project\n\nOn deployment inject API keys authorized to use your service. Every call to a private\nendpoint of your service has to include a `header[\'x-api-key\']` attribute that is\nvalidated against the API keys in your environment.\nIf it is present, a request is authorized. If it is not FastAPI return `401 Unauthorized`.\nUse this either as a middleware, or as Dependency.\n\n### Built With\n\n-   [starlette](https://github.com/encode/starlette)\n-   [fastapi](https://github.com/tiangolo/fastapi)\n\n<!-- GETTING STARTED -->\n\n## Getting Started\n\n### Installation\n\n1. Clone and install\n    ```sh\n    git clone https://github.com/iwpnd/fastapi-key-auth.git\n    poetry install\n    ```\n2. Install with pip\n    ```sh\n    pip install fastapi-key-auth\n    ```\n3. Install with poetry\n    ```sh\n    poetry add fastapi-key-auth\n    ```\n\n## Usage\n\nAs Middleware:\n\n```python\nfrom fastapi import FastAPI\nfrom fastapi_key_auth import AuthorizerMiddleware\n\napp = FastAPI()\n\napp.add_middleware(AuthorizerMiddleware, public_paths=["/ping"], key_pattern="API_KEY_")\n\n# optional use regex startswith\napp.add_middleware(AuthorizerMiddleware, public_paths=["/ping", "^/users"])\n```\n\nAs Dependency\n\n```python\nfrom fastapi import FastAPI, Depends\nfrom fastapi_key_auth import AuthorizerDependency\n\nauthorizer = AuthorizerDependency(key_pattern="API_KEY_")\n\n# either globally or in a router\napp = FastAPI(dependencies=[Depends(authorizer)])\n```\n\n## License\n\nDistributed under the MIT License. See `LICENSE` for more information.\n\n<!-- CONTACT -->\n\n## Contact\n\nBenjamin Ramser - [@imwithpanda](https://twitter.com/imwithpanda) - ahoi@iwpnd.pw  \nProject Link: [https://github.com/iwpnd/fastapi-key-auth](https://github.com/iwpnd/fastapi-key-auth)\n',
     'author': 'Benjamin Ramser',
     'author_email': 'legionaerr@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/iwpnd/fastapi-key-auth',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['fastapi_key_auth', 'fastapi_key_auth.dependency',
 'fastapi_key_auth.middleware'] package_data = \ {'': ['*']} install_requires =
-\ ['fastapi>=0.70.0,<0.87.0', 'starlette>=0.19.0,<0.20.0'] setup_kwargs =
-{ 'name': 'fastapi-key-auth', 'version': '0.8.0', 'description': 'API key
+\ ['fastapi>=0.84.0,<=0.92.0', 'starlette>=0.25.0,<0.26.0'] setup_kwargs =
+{ 'name': 'fastapi-key-auth', 'version': '0.9.0', 'description': 'API key
 validation Middleware', 'long_description': '
 \n
                                       \n
                           **** FastAPI-key-auth ****
 \n\n
               \n Secure your FastAPI endpoints using API keys.\n
                     \n Report_Bug\n Â·\n Request_Feature\n
@@ -42,17 +42,17 @@
 starlette)\n- [fastapi](https://github.com/tiangolo/fastapi)\n\n\n\n## Getting
 Started\n\n### Installation\n\n1. Clone and install\n ```sh\n git clone https:/
 /github.com/iwpnd/fastapi-key-auth.git\n poetry install\n ```\n2. Install with
 pip\n ```sh\n pip install fastapi-key-auth\n ```\n3. Install with poetry\n
 ```sh\n poetry add fastapi-key-auth\n ```\n\n## Usage\n\nAs Middleware:
 \n\n```python\nfrom fastapi import FastAPI\nfrom fastapi_key_auth import
 AuthorizerMiddleware\n\napp = FastAPI()\n\napp.add_middleware
-(AuthorizerMiddleware, public_path=["/ping"], key_pattern="API_KEY_")\n\n#
+(AuthorizerMiddleware, public_paths=["/ping"], key_pattern="API_KEY_")\n\n#
 optional use regex startswith\napp.add_middleware(AuthorizerMiddleware,
-public_path=["/ping", "^/users"])\n```\n\nAs Dependency\n\n```python\nfrom
+public_paths=["/ping", "^/users"])\n```\n\nAs Dependency\n\n```python\nfrom
 fastapi import FastAPI, Depends\nfrom fastapi_key_auth import
 AuthorizerDependency\n\nauthorizer = AuthorizerDependency
 (key_pattern="API_KEY_")\n\n# either globally or in a router\napp = FastAPI
 (dependencies=[Depends(authorizer)])\n```\n\n## License\n\nDistributed under
 the MIT License. See `LICENSE` for more information.\n\n\n\n##
 Contact\n\nBenjamin Ramser - [@imwithpanda](https://twitter.com/imwithpanda) -
 ahoi@iwpnd.pw \nProject Link: [https://github.com/iwpnd/fastapi-key-auth]
```

### Comparing `fastapi-key-auth-0.8.0/PKG-INFO` & `fastapi_key_auth-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: fastapi-key-auth
-Version: 0.8.0
+Version: 0.9.0
 Summary: API key validation Middleware
 Home-page: https://github.com/iwpnd/fastapi-key-auth
 License: MIT
 Keywords: tile38,async,client
 Author: Benjamin Ramser
 Author-email: legionaerr@googlemail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: fastapi (>=0.70.0,<0.87.0)
-Requires-Dist: starlette (>=0.19.0,<0.20.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fastapi (>=0.84.0,<=0.92.0)
+Requires-Dist: starlette (>=0.25.0,<0.26.0)
 Project-URL: Repository, https://github.com/iwpnd/fastapi-key-auth
 Description-Content-Type: text/markdown
 
 <br />
 <p align="center">
   <h3 align="center">FastAPI-key-auth</h3>
 
@@ -95,18 +96,18 @@
 
 ```python
 from fastapi import FastAPI
 from fastapi_key_auth import AuthorizerMiddleware
 
 app = FastAPI()
 
-app.add_middleware(AuthorizerMiddleware, public_path=["/ping"], key_pattern="API_KEY_")
+app.add_middleware(AuthorizerMiddleware, public_paths=["/ping"], key_pattern="API_KEY_")
 
 # optional use regex startswith
-app.add_middleware(AuthorizerMiddleware, public_path=["/ping", "^/users"])
+app.add_middleware(AuthorizerMiddleware, public_paths=["/ping", "^/users"])
 ```
 
 As Dependency
 
 ```python
 from fastapi import FastAPI, Depends
 from fastapi_key_auth import AuthorizerDependency
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: fastapi-key-auth Version: 0.8.0 Summary: API key
+Metadata-Version: 2.1 Name: fastapi-key-auth Version: 0.9.0 Summary: API key
 validation Middleware Home-page: https://github.com/iwpnd/fastapi-key-auth
 License: MIT Keywords: tile38,async,client Author: Benjamin Ramser Author-
 email: legionaerr@googlemail.com Requires-Python: >=3.7,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-Dist:
-fastapi (>=0.70.0,<0.87.0) Requires-Dist: starlette (>=0.19.0,<0.20.0) Project-
-URL: Repository, https://github.com/iwpnd/fastapi-key-auth Description-Content-
-Type: text/markdown
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: fastapi
+(>=0.84.0,<=0.92.0) Requires-Dist: starlette (>=0.25.0,<0.26.0) Project-URL:
+Repository, https://github.com/iwpnd/fastapi-key-auth Description-Content-Type:
+text/markdown
                           **** FastAPI-key-auth ****
                 Secure your FastAPI endpoints using API keys.
                          Report_Bug Â· Request_Feature
 
 ***** Table of Contents *****
    1. About_The_Project
           o Built_With
@@ -29,16 +30,16 @@
 ### Built With - [starlette](https://github.com/encode/starlette) - [fastapi]
 (https://github.com/tiangolo/fastapi)  ## Getting Started ### Installation 1.
 Clone and install ```sh git clone https://github.com/iwpnd/fastapi-key-auth.git
 poetry install ``` 2. Install with pip ```sh pip install fastapi-key-auth ```
 3. Install with poetry ```sh poetry add fastapi-key-auth ``` ## Usage As
 Middleware: ```python from fastapi import FastAPI from fastapi_key_auth import
 AuthorizerMiddleware app = FastAPI() app.add_middleware(AuthorizerMiddleware,
-public_path=["/ping"], key_pattern="API_KEY_") # optional use regex startswith
-app.add_middleware(AuthorizerMiddleware, public_path=["/ping", "^/users"]) ```
+public_paths=["/ping"], key_pattern="API_KEY_") # optional use regex startswith
+app.add_middleware(AuthorizerMiddleware, public_paths=["/ping", "^/users"]) ```
 As Dependency ```python from fastapi import FastAPI, Depends from
 fastapi_key_auth import AuthorizerDependency authorizer = AuthorizerDependency
 (key_pattern="API_KEY_") # either globally or in a router app = FastAPI
 (dependencies=[Depends(authorizer)]) ``` ## License Distributed under the MIT
 License. See `LICENSE` for more information.  ## Contact Benjamin Ramser -
 [@imwithpanda](https://twitter.com/imwithpanda) - ahoi@iwpnd.pw Project Link:
 [https://github.com/iwpnd/fastapi-key-auth](https://github.com/iwpnd/fastapi-
```

