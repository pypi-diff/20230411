# Comparing `tmp/sliceline-0.2.8.tar.gz` & `tmp/sliceline-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliceline-0.2.8.tar", max compression
+gzip compressed data, was "sliceline-0.2.9.tar", max compression
```

## Comparing `sliceline-0.2.8.tar` & `sliceline-0.2.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1531 2022-09-27 16:59:20.354475 sliceline-0.2.8/LICENSE
--rw-r--r--   0        0        0     2923 2022-09-27 16:59:20.354475 sliceline-0.2.8/README.rst
--rw-r--r--   0        0        0      840 2022-09-27 16:59:31.946495 sliceline-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       64 2022-09-27 16:59:20.358475 sliceline-0.2.8/sliceline/__init__.py
--rw-r--r--   0        0        0    23450 2022-09-27 16:59:20.358475 sliceline-0.2.8/sliceline/slicefinder.py
--rw-r--r--   0        0        0    30680 2022-09-27 16:59:20.358475 sliceline-0.2.8/sliceline/validation.py
--rw-r--r--   0        0        0     3728 1970-01-01 00:00:00.000000 sliceline-0.2.8/setup.py
--rw-r--r--   0        0        0     3631 1970-01-01 00:00:00.000000 sliceline-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1531 2022-11-22 15:10:23.706311 sliceline-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2923 2022-11-22 15:10:23.706311 sliceline-0.2.9/README.rst
+-rw-r--r--   0        0        0      839 2022-11-22 15:10:34.586606 sliceline-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0       64 2022-11-22 15:10:23.706311 sliceline-0.2.9/sliceline/__init__.py
+-rw-r--r--   0        0        0    23450 2022-11-22 15:10:23.706311 sliceline-0.2.9/sliceline/slicefinder.py
+-rw-r--r--   0        0        0    30680 2022-11-22 15:10:23.706311 sliceline-0.2.9/sliceline/validation.py
+-rw-r--r--   0        0        0     3727 1970-01-01 00:00:00.000000 sliceline-0.2.9/setup.py
+-rw-r--r--   0        0        0     3680 1970-01-01 00:00:00.000000 sliceline-0.2.9/PKG-INFO
```

### Comparing `sliceline-0.2.8/LICENSE` & `sliceline-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sliceline-0.2.8/README.rst` & `sliceline-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `sliceline-0.2.8/pyproject.toml` & `sliceline-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sliceline"
-version = "0.2.8" # This version is a generic placeholder. It should not be changed.
+version = "0.2.9" # This version is a generic placeholder. It should not be changed.
 description = "✂️ Fast slice finding for Machine Learning model debugging."
 authors = ["Antoine de Daran"]
 readme = "README.rst"
 license = "BSD-3-Clause"
 repository = "https://github.com/DataDome/sliceline"
 documentation = "https://sliceline.readthedocs.io/en/stable/"
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.10"
-numpy = "^1.22.0"
+python = ">=3.7, <3.10"
+numpy = "^1.0.0"
 scikit-learn = "^1.0.1"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 flake8 = "^3.0.0"
 jupyter = "^1.0.0"
 nbconvert = "^6.5.0"
```

### Comparing `sliceline-0.2.8/sliceline/slicefinder.py` & `sliceline-0.2.9/sliceline/slicefinder.py`

 * *Files identical despite different names*

### Comparing `sliceline-0.2.8/sliceline/validation.py` & `sliceline-0.2.9/sliceline/validation.py`

 * *Files identical despite different names*

### Comparing `sliceline-0.2.8/setup.py` & `sliceline-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['sliceline']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.22.0,<2.0.0', 'scikit-learn>=1.0.1,<2.0.0']
+['numpy>=1.0.0,<2.0.0', 'scikit-learn>=1.0.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'sliceline',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': '✂️ Fast slice finding for Machine Learning model debugging.',
     'long_description': 'Sliceline\n=========\n\nSliceline is a Python library for fast slice finding for Machine\nLearning model debugging.\n\nIt is an implementation of `SliceLine: Fast, Linear-Algebra-based Slice\nFinding for ML Model\nDebugging <https://mboehm7.github.io/resources/sigmod2021b_sliceline.pdf>`__,\nfrom Svetlana Sagadeeva and Matthias Boehm of Graz University of\nTechnology.\n\n👉 Getting started\n------------------\n\nGiven an input dataset ``X`` and a model error vector ``errors``,\nSliceLine finds the top slices in ``X`` that identify where a ML model\nperforms significantly worse.\n\nYou can use sliceline as follows:\n\n.. code:: python\n\n   from sliceline.slicefinder import Slicefinder\n\n   slice_finder = Slicefinder()\n\n   slice_finder.fit(X, errors)\n\n   print(slice_finder.top_slices_)\n\n   X_trans = slice_finder.transform(X)\n\nWe invite you to check the `demo\nnotebooks <https://github.com/DataDome/sliceline/blob/main/notebooks>`__\nfor a more thorough tutorial:\n\n1. Implementing Sliceline on Titanic dataset\n2. Implementing Sliceline on California housing dataset\n\n🛠 Installation\n---------------\n\nSliceline is intended to work with **Python 3.7 or above**. Installation\ncan be done with ``pip``:\n\n.. code:: sh\n\n   pip install sliceline\n\nThere are `wheels\navailable <https://pypi.org/project/sliceline/#files>`__ for Linux,\nMacOS, and Windows, which means that you most probably won’t have to\nbuild Sliceline from source.\n\nYou can install the latest development version from GitHub as so:\n\n.. code:: sh\n\n   pip install git+https://github.com/DataDome/sliceline --upgrade\n\nOr, through SSH:\n\n.. code:: sh\n\n   pip install git+ssh://git@github.com/datadome/sliceline.git --upgrade\n\n🔗 Useful links\n---------------\n\n-  `Documentation <https://sliceline.readthedocs.io/en/stable/>`__\n-  `Package releases <https://pypi.org/project/sliceline/#history>`__\n-  `SliceLine paper <https://mboehm7.github.io/resources/sigmod2021b_sliceline.pdf>`__\n\n👐 Contributing\n---------------\n\nFeel free to contribute in any way you like, we’re always open to new\nideas and approaches.\n\n-  `Open a\n   discussion <https://github.com/DataDome/sliceline/discussions/new>`__\n   if you have any question or enquiry whatsoever. It’s more useful to\n   ask your question in public rather than sending us a private email.\n   It’s also encouraged to open a discussion before contributing, so\n   that everyone is aligned and unnecessary work is avoided.\n-  Feel welcome to `open an\n   issue <https://github.com/DataDome/sliceline/issues/new/choose>`__ if\n   you think you’ve spotted a bug or a performance issue.\n\nPlease check out the `contribution\nguidelines <https://github.com/DataDome/sliceline/blob/main/CONTRIBUTING.md>`__\nif you want to bring modifications to the code base.\n\n📝 License\n----------\n\nSliceline is free and open-source software licensed under the `3-clause BSD license <https://github.com/DataDome/sliceline/blob/main/LICENSE>`__.\n',
     'author': 'Antoine de Daran',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DataDome/sliceline',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.10',
+    'python_requires': '>=3.7,<3.10',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `sliceline-0.2.8/PKG-INFO` & `sliceline-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sliceline
-Version: 0.2.8
+Version: 0.2.9
 Summary: ✂️ Fast slice finding for Machine Learning model debugging.
 Home-page: https://github.com/DataDome/sliceline
 License: BSD-3-Clause
 Author: Antoine de Daran
-Requires-Python: >=3.8,<3.10
+Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: numpy (>=1.22.0,<2.0.0)
+Requires-Dist: numpy (>=1.0.0,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0.1,<2.0.0)
 Project-URL: Documentation, https://sliceline.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/DataDome/sliceline
 Description-Content-Type: text/x-rst
 
 Sliceline
 =========
```

