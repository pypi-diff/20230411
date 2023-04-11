# Comparing `tmp/sra-pylib-1.3.1.tar.gz` & `tmp/sra-pylib-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sra-pylib-1.3.1.tar", last modified: Wed Mar  8 12:43:47 2023, max compression
+gzip compressed data, was "sra-pylib-1.4.0.tar", last modified: Tue Apr 11 11:38:58 2023, max compression
```

## Comparing `sra-pylib-1.3.1.tar` & `sra-pylib-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:43:47.403132 sra-pylib-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-08 12:43:37.000000 sra-pylib-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-03-08 12:43:47.403132 sra-pylib-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-08 12:43:37.000000 sra-pylib-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 12:43:47.403132 sra-pylib-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-08 12:43:37.000000 sra-pylib-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:43:47.403132 sra-pylib-1.3.1/sra/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-08 12:43:37.000000 sra-pylib-1.3.1/sra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18180 2023-03-08 12:43:37.000000 sra-pylib-1.3.1/sra/animal.py
--rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-03-08 12:43:37.000000 sra-pylib-1.3.1/sra/animu.py
--rw-r--r--   0 runner    (1001) docker     (123)    89817 2023-03-08 12:43:37.000000 sra-pylib-1.3.1/sra/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-08 12:43:37.000000 sra-pylib-1.3.1/sra/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-03-08 12:43:37.000000 sra-pylib-1.3.1/sra/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)    20647 2023-03-08 12:43:37.000000 sra-pylib-1.3.1/sra/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-03-08 12:43:37.000000 sra-pylib-1.3.1/sra/others.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-03-08 12:43:37.000000 sra-pylib-1.3.1/sra/pokemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:43:47.403132 sra-pylib-1.3.1/sra_pylib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-03-08 12:43:47.000000 sra-pylib-1.3.1/sra_pylib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-08 12:43:47.000000 sra-pylib-1.3.1/sra_pylib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 12:43:47.000000 sra-pylib-1.3.1/sra_pylib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-08 12:43:47.000000 sra-pylib-1.3.1/sra_pylib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-08 12:43:47.000000 sra-pylib-1.3.1/sra_pylib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:38:58.230808 sra-pylib-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-11 11:38:58.230808 sra-pylib-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 11:38:58.230808 sra-pylib-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:38:58.230808 sra-pylib-1.4.0/sra/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/sra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20783 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/sra/animal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/sra/animu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97290 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/sra/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/sra/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/sra/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/sra/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/sra/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/sra/others.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/sra/pokemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-11 11:38:46.000000 sra-pylib-1.4.0/sra/welcome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:38:58.230808 sra-pylib-1.4.0/sra_pylib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-11 11:38:58.000000 sra-pylib-1.4.0/sra_pylib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-11 11:38:58.000000 sra-pylib-1.4.0/sra_pylib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:38:58.000000 sra-pylib-1.4.0/sra_pylib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 11:38:58.000000 sra-pylib-1.4.0/sra_pylib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-11 11:38:58.000000 sra-pylib-1.4.0/sra_pylib.egg-info/top_level.txt
```

### Comparing `sra-pylib-1.3.1/LICENSE` & `sra-pylib-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sra-pylib-1.3.1/PKG-INFO` & `sra-pylib-1.4.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,43 @@
-Metadata-Version: 2.1
-Name: sra-pylib
-Version: 1.3.1
-Summary: A Wrapper of some-random-api for Python
-Home-page: https://github.com/Sayad-Uddin-Tahsin/sra-pylib
-Author: Sayad Uddin Tahsin
-Author-email: mr.pluto012@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/Sayad-Uddin-Tahsin/sra-pylib/issues
-Project-URL: PyPI, https://pypi.org/project/sra-pylib/
-Keywords: some-random-api,sra,api-wrapper,sra-pylib,sra-wrapper,tahsin-project
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# sra-pylib
-`sra-pylib` is a Python wrapper for [some-random-api](https://some-random-api.ml).
-
-```python
-import sra
-
->>> print(sra.animal.Panda.image_link)  # Prints a Panda Image link
-"https://i.imgur.com/YVLrUO9.jpg"
->>> print(sra.animal.Panda.fact)  # Prints a Panda Fact
-"Giant pandas have been driven out of the lowland areas where they used to live and now are found only in the Chinese provinces of Sichuan, Gansu, and Shaanxi. The forests in these provinces are very damp and rainy. In one year, a forest may receive up to 50 inches of rain and snow."
->>> sra.animal.Panda.save_image()  # Saves the Image
-```
-With `sra-pylib`, you can easily access the various endpoints of `some-random-api` in your Python projects, making it a powerful tool for working with image, fact, and other types of data.
-
-<a href="https://pypi.org/project/sra-pylib"><img src="https://img.shields.io/pypi/status/sra-pylib?label=Status&logo=pypi&logoColor=ffffff" height=22></a> <a href="https://pypi.org/project/sra-pylib"><img src="https://img.shields.io/pypi/v/sra-pylib?label=PyPI Version&logo=pypi&logoColor=ffffff" height=22></a> <a href="https://python.org"><img src="https://img.shields.io/pypi/pyversions/sra-pylib?label=Python&logo=python&logoColor=ffdd54" height=22></a>
-
-## Installation
-You can install `sra-pylib` using `pip`:
-```console
-python -m pip install sra-pylib
-```
-`sra-pylib` requires Python 3.7 or later.
-
-## Endpoints
-`sra-pylib` is currently under development. Currently, only the `animal`, `animu`, `canvas`, `fact`, `image`, `others` and `pokemon` categories of APIs are available in stable version, but we're working to add more.
-
-## Cloning the Repository
-If you want to work with the development version of sra-pylib, you can clone the repository and install it using pip:
-```console
-pip install git+https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git
-```
-This will install the package from the cloned repository.
+# sra-pylib
+`sra-pylib` is a Python wrapper for [some-random-api](https://some-random-api.ml).
+
+```python
+import sra
+
+>>> print(sra.animal.Panda.image_link)  # Prints a Panda Image link
+"https://i.imgur.com/YVLrUO9.jpg"
+>>> print(sra.animal.Panda.fact)  # Prints a Panda Fact
+"Giant pandas have been driven out of the lowland areas where they used to live and now are found only in the Chinese provinces of Sichuan, Gansu, and Shaanxi. The forests in these provinces are very damp and rainy. In one year, a forest may receive up to 50 inches of rain and snow."
+>>> sra.animal.Panda.save_image()  # Saves the Image
+```
+With `sra-pylib`, you can easily access the various endpoints of `some-random-api` in your Python projects, making it a powerful tool for working with image, fact, and other types of data.
+
+<a href="https://pypi.org/project/sra-pylib"><img src="https://img.shields.io/pypi/status/sra-pylib?label=Status&logo=pypi&logoColor=ffffff" height=22></a>
+<a href="https://pypi.org/project/sra-pylib"><img src="https://img.shields.io/pypi/v/sra-pylib?label=PyPI Version&logo=pypi&logoColor=ffffff" height=22></a>
+<a href="https://app.fossa.com/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_shield" alt="FOSSA Status"><img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib.svg?type=shield" height=22></a>
+<a href="https://python.org"><img src="https://img.shields.io/pypi/pyversions/sra-pylib?label=Python&logo=python&logoColor=ffdd54" height=22></a>
+
+## Installation
+You can install `sra-pylib` using `pip`:
+```console
+python -m pip install sra-pylib
+```
+`sra-pylib` requires Python 3.7 or later.
+
+## Endpoints
+`sra-pylib` is synced with some-random-api. It has all the Endpoints provided by some-random-api except the Premium ones.
+
+## Documentation
+Full documentation for the sra-pylib module can be found on [Wiki](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/wiki). The documentation includes detailed information on how to use the module, including examples and reference documentation for all classes and methods.
+
+If you have any questions or issues with the module, please refer to the documentation or submit a bug report on the [GitHub issues page](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/issues).
+
+## Cloning the Repository
+You also can install sra-pylib directly from Github, by using this pip command:
+```console
+pip install git+https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git
+```
+This will install the package directly from the repository.
+
+## License
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_large)
```

#### html2text {}

```diff
@@ -1,37 +1,32 @@
-Metadata-Version: 2.1 Name: sra-pylib Version: 1.3.1 Summary: A Wrapper of
-some-random-api for Python Home-page: https://github.com/Sayad-Uddin-Tahsin/
-sra-pylib Author: Sayad Uddin Tahsin Author-email: mr.pluto012@gmail.com
-License: MIT Project-URL: Bug Tracker, https://github.com/Sayad-Uddin-Tahsin/
-sra-pylib/issues Project-URL: PyPI, https://pypi.org/project/sra-pylib/
-Keywords: some-random-api,sra,api-wrapper,sra-pylib,sra-wrapper,tahsin-project
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE #
-sra-pylib `sra-pylib` is a Python wrapper for [some-random-api](https://some-
+# sra-pylib `sra-pylib` is a Python wrapper for [some-random-api](https://some-
 random-api.ml). ```python import sra >>> print(sra.animal.Panda.image_link) #
 Prints a Panda Image link "https://i.imgur.com/YVLrUO9.jpg" >>> print
 (sra.animal.Panda.fact) # Prints a Panda Fact "Giant pandas have been driven
 out of the lowland areas where they used to live and now are found only in the
 Chinese provinces of Sichuan, Gansu, and Shaanxi. The forests in these
 provinces are very damp and rainy. In one year, a forest may receive up to 50
 inches of rain and snow." >>> sra.animal.Panda.save_image() # Saves the Image
 ``` With `sra-pylib`, you can easily access the various endpoints of `some-
 random-api` in your Python projects, making it a powerful tool for working with
 image, fact, and other types of data. [https://img.shields.io/pypi/status/sra-
 pylib?label=Status&logo=pypi&logoColor=ffffff] [https://img.shields.io/pypi/v/
 sra-pylib?label=PyPI_Version&logo=pypi&logoColor=ffffff] [https://
-img.shields.io/pypi/pyversions/sra-
+app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-
+pylib.svg?type=shield] [https://img.shields.io/pypi/pyversions/sra-
 pylib?label=Python&logo=python&logoColor=ffdd54] ## Installation You can
 install `sra-pylib` using `pip`: ```console python -m pip install sra-pylib ```
-`sra-pylib` requires Python 3.7 or later. ## Endpoints `sra-pylib` is currently
-under development. Currently, only the `animal`, `animu`, `canvas`, `fact`,
-`image`, `others` and `pokemon` categories of APIs are available in stable
-version, but we're working to add more. ## Cloning the Repository If you want
-to work with the development version of sra-pylib, you can clone the repository
-and install it using pip: ```console pip install git+https://github.com/Sayad-
-Uddin-Tahsin/sra-pylib.git ``` This will install the package from the cloned
-repository.
+`sra-pylib` requires Python 3.7 or later. ## Endpoints `sra-pylib` is synced
+with some-random-api. It has all the Endpoints provided by some-random-api
+except the Premium ones. ## Documentation Full documentation for the sra-pylib
+module can be found on [Wiki](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/
+wiki). The documentation includes detailed information on how to use the
+module, including examples and reference documentation for all classes and
+methods. If you have any questions or issues with the module, please refer to
+the documentation or submit a bug report on the [GitHub issues page](https://
+github.com/Sayad-Uddin-Tahsin/sra-pylib/issues). ## Cloning the Repository You
+also can install sra-pylib directly from Github, by using this pip command:
+```console pip install git+https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git
+``` This will install the package directly from the repository. ## License [!
+[FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-
+Uddin-Tahsin%2Fsra-pylib.svg?type=large)](https://app.fossa.com/projects/
+git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_large)
```

### Comparing `sra-pylib-1.3.1/setup.py` & `sra-pylib-1.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='sra-pylib',
-    version='1.3.1',
+    version='1.4.0',
     author='Sayad Uddin Tahsin',
     author_email='mr.pluto012@gmail.com',
     description='A Wrapper of some-random-api for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Sayad-Uddin-Tahsin/sra-pylib',
     packages=find_packages(),
@@ -26,12 +26,13 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11'
     ],
     python_requires='>=3.7',
     project_urls={
+        'Documentation': 'https://github.com/Sayad-Uddin-Tahsin/sra-pylib/wiki',
         'Bug Tracker': 'https://github.com/Sayad-Uddin-Tahsin/sra-pylib/issues',
         'PyPI': 'https://pypi.org/project/sra-pylib/'
     },
     keywords=['some-random-api', 'sra', 'api-wrapper', 'sra-pylib', 'sra-wrapper', 'tahsin-project']
 )
```

### Comparing `sra-pylib-1.3.1/sra/animal.py` & `sra-pylib-1.4.0/sra/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,483 +1,625 @@
 import requests
 import sra
 
-class Bird():
+
+class Bird:
+    """
+    Returns a random Image Link of a Bird by attributes
+
+
+    :raise APITimeout: API taken too long to respond!
+    :raise APIError: Error Returned by API
+    """
+    try:
+        __resp = requests.get("https://some-random-api.ml/img/bird")
+    except requests.exceptions.ConnectionError:
+        raise sra.exceptions.APITimeout("API taken too long to respond!")
+    if __resp.status_code != 200:
+        if 'error' in __resp.json():
+            raise sra.exceptions.APIError(__resp.json()['error'])
+        else:
+            raise sra.exceptions.APIError(
+                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+
+    __resp = __resp.json()
+
+    image_link = __resp['link']
+    raw = __resp
+
+    @classmethod
+    def save_image(cls, name: str = "bird.png"):
+        """
+        Saves the Image
+
+        :param name: Image Name/PATH (Optional)
+        :return: Image, bool
+        :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise ImageNotFound: When failed to save Image
+        """
+        formats = ['.png', '.jpg', '.jpeg']
+        validFormat = False
+        for f in formats:
+            if str(name).endswith(f):
+                validFormat = True
+                break
+        if not validFormat:
+            raise sra.exceptions.InvalidFileFormat(
+                'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
+        path = name
+        try:
+            __r = requests.get(cls.image_link, stream=True)
+        except requests.exceptions.ConnectionError:
+            raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
+        if __r.status_code == 200:
+            with open(path, 'wb') as f:
+                f.write(__r.content)
+                return True
+        else:
+            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
+
+
+class Cat:
+    """
+    Returns a random Image Link of a Cat by attributes
+
+
+    :raise APITimeout: API taken too long to respond!
+    :raise APIError: Error Returned by API
+    """
+    try:
+        __resp = requests.get("https://some-random-api.ml/img/cat")
+    except requests.exceptions.ConnectionError:
+        raise sra.exceptions.APITimeout("API taken too long to respond!")
+    if __resp.status_code != 200:
+        if 'error' in __resp.json():
+            raise sra.exceptions.APIError(__resp.json()['error'])
+        else:
+            raise sra.exceptions.APIError(
+                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+
+    __resp = __resp.json()
+
+    image_link = __resp['link']
+    raw = __resp
+
+    @classmethod
+    def save_image(cls, name: str = "cat.png"):
+        """
+        Saves the Image
+
+        :param name: Image Name/PATH (Optional)
+        :return: Image, bool
+        :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise ImageNotFound: When failed to save Image
+        """
+        formats = ['.png', '.jpg', '.jpeg']
+        validFormat = False
+        for f in formats:
+            if str(name).endswith(f):
+                validFormat = True
+                break
+        if not validFormat:
+            raise sra.exceptions.InvalidFileFormat(
+                'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
+        path = name
+        try:
+            __r = requests.get(cls.image_link, stream=True)
+        except requests.exceptions.ConnectionError:
+            raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
+        if __r.status_code == 200:
+            with open(path, 'wb') as f:
+                f.write(__r.content)
+                return True
+        else:
+            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
+
+
+class Dog:
     """
-    Returns an Image Link and a Fact about Bird
+    Returns a random Image Link of a Dog by attributes
+
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/animal/bird")
+        __resp = requests.get("https://some-random-api.ml/img/dog")
     except requests.exceptions.ConnectionError:
-            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
                 f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
 
     __resp = __resp.json()
 
-    image_link = __resp['image']
-    fact = __resp['fact']
+    image_link = __resp['link']
+    raw = __resp
 
     @classmethod
-    def save_image(cls, name: str="bird.png"):
+    def save_image(cls, name: str = "dog.png"):
         """
-        Saves the Bird Image
+        Saves the Image
 
         :param name: Image Name/PATH (Optional)
-        :returns: Image, bool
+        :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
-            raise sra.exceptions.InvalidFileFormat('Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
+            raise sra.exceptions.InvalidFileFormat(
+                'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
         try:
             __r = requests.get(cls.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
-class Cat():
+class Fox:
     """
-    Returns an Image Link and a Fact about Cat
+    Returns a random Image Link of a Fox by attributes
+
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/animal/cat")
+        __resp = requests.get("https://some-random-api.ml/img/fox")
     except requests.exceptions.ConnectionError:
-            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
                 f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
 
     __resp = __resp.json()
 
-    image_link = __resp['image']
-    fact = __resp['fact']
+    image_link = __resp['link']
+    raw = __resp
 
     @classmethod
-    def save_image(cls, name: str="cat.png"):
+    def save_image(cls, name: str = "fox.png"):
         """
-        Saves the Cat Image
+        Saves the Image
 
         :param name: Image Name/PATH (Optional)
-        :returns: Image, bool
+        :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
-            raise sra.exceptions.InvalidFileFormat('Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
+            raise sra.exceptions.InvalidFileFormat(
+                'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
         try:
             __r = requests.get(cls.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
-class Dog():
+class Kangaroo:
     """
-    Returns an Image Link and a Fact about Dog
+    Returns a random Image Link of a Kangaroo by attributes
+
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/animal/dog")
+        __resp = requests.get("https://some-random-api.ml/img/kangaroo")
     except requests.exceptions.ConnectionError:
-            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
                 f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
 
     __resp = __resp.json()
 
-    image_link = __resp['image']
-    fact = __resp['fact']
+    image_link = __resp['link']
+    raw = __resp
 
     @classmethod
-    def save_image(cls, name: str="dog.png"):
+    def save_image(cls, name: str = "kangaroo.png"):
         """
-        Saves the Dog Image
+        Saves the Image
 
         :param name: Image Name/PATH (Optional)
-        :returns: Image, bool
+        :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
-            raise sra.exceptions.InvalidFileFormat('Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
+            raise sra.exceptions.InvalidFileFormat(
+                'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
         try:
             __r = requests.get(cls.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
-class Fox():
+class Koala:
     """
-    Returns an Image Link and a Fact about Fox
+    Returns a random Image Link of a Koala by attributes
+
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/animal/fox")
+        __resp = requests.get("https://some-random-api.ml/img/koala")
     except requests.exceptions.ConnectionError:
-            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
                 f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
 
     __resp = __resp.json()
 
-    image_link = __resp['image']
-    fact = __resp['fact']
+    image_link = __resp['link']
+    raw = __resp
 
     @classmethod
-    def save_image(cls, name: str="fox.png"):
+    def save_image(cls, name: str = "koala.png"):
         """
-        Saves the Fox Image
+        Saves the Image
 
         :param name: Image Name/PATH (Optional)
-        :returns: Image, bool
+        :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
-            raise sra.exceptions.InvalidFileFormat('Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
+            raise sra.exceptions.InvalidFileFormat(
+                'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
         try:
             __r = requests.get(cls.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
-class Kangaroo():
+class Panda:
     """
-    Returns an Image Link and a Fact about Kangaroo
+    Returns a random Image Link of a Panda by attributes
+
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/animal/kangaroo")
+        __resp = requests.get("https://some-random-api.ml/img/panda")
     except requests.exceptions.ConnectionError:
-            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
                 f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
 
     __resp = __resp.json()
 
-    image_link = __resp['image']
-    fact = __resp['fact']
+    image_link = __resp['link']
+    raw = __resp
 
     @classmethod
-    def save_image(cls, name: str="kangaroo.png"):
+    def save_image(cls, name: str = "panda.png"):
         """
-        Saves the Kangaroo Image
+        Saves the Image
 
         :param name: Image Name/PATH (Optional)
-        :returns: Image, bool
+        :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
-            raise sra.exceptions.InvalidFileFormat('Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
+            raise sra.exceptions.InvalidFileFormat(
+                'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
         try:
             __r = requests.get(cls.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
-class Koala():
+class Pikachu:
     """
-    Returns an Image Link and a Fact about Koala
+    Returns a random Image Link of a Pikachu by attributes
+
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/animal/koala")
+        __resp = requests.get("https://some-random-api.ml/img/pikachu")
     except requests.exceptions.ConnectionError:
-            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
                 f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
 
     __resp = __resp.json()
 
-    image_link = __resp['image']
-    fact = __resp['fact']
+    image_link = __resp['link']
+    raw = __resp
 
     @classmethod
-    def save_image(cls, name: str="koala.png"):
+    def save_image(cls, name: str = "pikachu.png"):
         """
-        Saves the Koala Image
+        Saves the Image
 
         :param name: Image Name/PATH (Optional)
-        :returns: Image, bool
+        :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
-            raise sra.exceptions.InvalidFileFormat('Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
+            raise sra.exceptions.InvalidFileFormat(
+                'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
         try:
             __r = requests.get(cls.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
-class Panda():
+class Raccoon:
     """
-    Returns an Image Link and a Fact about Panda
+    Returns a random Image Link of a Raccoon by attributes
+
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/animal/panda")
+        __resp = requests.get("https://some-random-api.ml/img/raccoon")
     except requests.exceptions.ConnectionError:
-            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
                 f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
 
     __resp = __resp.json()
 
-    image_link = __resp['image']
-    fact = __resp['fact']
+    image_link = __resp['link']
+    raw = __resp
 
     @classmethod
-    def save_image(cls, name: str="panda.png"):
+    def save_image(cls, name: str = "raccoon.png"):
         """
-        Saves the Panda Image
+        Saves the Image
 
         :param name: Image Name/PATH (Optional)
-        :returns: Image, bool
+        :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
-            raise sra.exceptions.InvalidFileFormat('Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
+            raise sra.exceptions.InvalidFileFormat(
+                'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
         try:
             __r = requests.get(cls.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
-class Raccoon():
+class RedPanda:
     """
-    Returns an Image Link and a Fact about Raccoon
+    Returns a random Image Link of a Red Panda by attributes
+
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/animal/raccoon")
+        __resp = requests.get("https://some-random-api.ml/img/red_panda")
     except requests.exceptions.ConnectionError:
-            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
                 f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
 
     __resp = __resp.json()
 
-    image_link = __resp['image']
-    fact = __resp['fact']
+    image_link = __resp['link']
+    raw = __resp
 
     @classmethod
-    def save_image(cls, name: str="raccoon.png"):
+    def save_image(cls, name: str = "red panda.png"):
         """
-        Saves the Raccoon Image
+        Saves the Image
 
         :param name: Image Name/PATH (Optional)
-        :returns: Image, bool
+        :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
-            raise sra.exceptions.InvalidFileFormat('Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
+            raise sra.exceptions.InvalidFileFormat(
+                'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
         try:
             __r = requests.get(cls.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
-class RedPanda():
+class Whale:
     """
-    Returns an Image Link and a Fact about Red Panda
+    Returns a random Image Link of a Whale by attributes
+
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/animal/red_panda")
+        __resp = requests.get("https://some-random-api.ml/img/whale")
     except requests.exceptions.ConnectionError:
-            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
                 f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
 
     __resp = __resp.json()
 
-    image_link = __resp['image']
-    fact = __resp['fact']
+    image_link = __resp['link']
+    raw = __resp
 
     @classmethod
-    def save_image(cls, name: str="red panda.png"):
+    def save_image(cls, name: str = "whale.png"):
         """
-        Saves the Red Panda Image
+        Saves the Image
 
         :param name: Image Name/PATH (Optional)
-        :returns: Image, bool
+        :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
-            raise sra.exceptions.InvalidFileFormat('Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
+            raise sra.exceptions.InvalidFileFormat(
+                'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
         try:
             __r = requests.get(cls.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
```

### Comparing `sra-pylib-1.3.1/sra/animu.py` & `sra-pylib-1.4.0/sra/animu.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,231 +1,247 @@
 import requests
 import sra
 
-class FacePalm():
+
+class FacePalm:
     """
-    Returns the GIF Link of a Face Palm by attribut
+    Returns the GIF Link of a Face Palm by attributes
+
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
-    es
+    """
+    def __init__(self):
+        self.__resp = None
 
-    Attributes:
-        gif_link (str):
-            The link to the Face Palm GIF.
-    """
-    try:
-        __resp = requests.get("https://some-random-api.ml/animu/face-palm")
-    except requests.exceptions.ConnectionError:
+        try:
+            self.__resp = requests.get("https://some-random-api.ml/animu/face-palm")
+        except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned,    200 expected!")
 
-    __resp = __resp.json()
+        self.__resp = self.__resp.json()
 
-    gif_link = __resp['link']
+        self.raw = self.__resp
+        self.gif_link = self.__resp['link']
 
-    @classmethod
-    def save_gif(cls, name: str='face palm.gif'):
+    def save_gif(self, name: str = 'face palm.gif'):
         """
         Saves the Face Palm GIF
 
         :param name: Image Name/PATH (Optional)
         :returns: GIF, bool
         :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise ImageNotFound: When failed to save Image
         """
         if not str(name).endswith(".gif"):
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".gif"!')
         path = name
         try:
-            r = requests.get(cls.gif_link, stream=True)
+            r = requests.get(self.gif_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the GIF. Status Code: {r.status_code} returned")
 
 
-class Hug():
+class Hug:
     """
     Returns the GIF Link of a Hug by attributes
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
-    try:
-        __resp = requests.get("https://some-random-api.ml/animu/hug")
-    except requests.exceptions.ConnectionError:
+    def __init__(self):
+        self.__resp = None
+
+        try:
+            self.__resp = requests.get("https://some-random-api.ml/animu/hug")
+        except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned,    200 expected!")
 
-    __resp = __resp.json()
+        self.__resp = self.__resp.json()
 
-    gif_link = __resp['link']
+        self.raw = self.__resp
+        self.gif_link = self.__resp['link']
 
-    @classmethod
-    def save_gif(cls, name: str='hug.gif'):
+    def save_gif(self, name: str = 'hug.gif'):
         """
         Saves the Hug GIF
 
         :param name: Image Name/PATH (Optional)
         :returns: GIF, bool
         :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise ImageNotFound: When failed to save Image
         """
         if not str(name).endswith(".gif"):
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".gif"!')
         path = name
         try:
-            r = requests.get(cls.gif_link, stream=True)
+            r = requests.get(self.gif_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the GIF. Status Code: {r.status_code} returned")
 
 
-class Pat():
+class Pat:
     """
     Returns the GIF Link of a Pat by attributes
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
-    try:
-        __resp = requests.get("https://some-random-api.ml/animu/pat")
-    except requests.exceptions.ConnectionError:
+    def __init__(self):
+        self.__resp = None
+
+        try:
+            self.__resp = requests.get("https://some-random-api.ml/animu/pat")
+        except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned,    200 expected!")
 
-    __resp = __resp.json()
+        self.__resp = self.__resp.json()
 
-    gif_link = __resp['link']
+        self.raw = self.__resp
+        self.gif_link = self.__resp['link']
 
-    @classmethod
-    def save_gif(cls, name: str='pat.gif'):
+    def save_gif(self, name: str = 'pat.gif'):
         """
         Saves the Pat GIF
 
         :param name: Image Name/PATH (Optional)
         :returns: GIF, bool
         :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise ImageNotFound: When failed to save Image
         """
         if not str(name).endswith(".gif"):
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".gif"!')
         path = name
         try:
-            r = requests.get(cls.gif_link, stream=True)
+            r = requests.get(self.gif_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the GIF. Status Code: {r.status_code} returned")
 
 
-class Wink():
+class Wink:
     """
     Returns the GIF Link of a Wink by attributes
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
-    try:
-        __resp = requests.get("https://some-random-api.ml/animu/wink")
-    except requests.exceptions.ConnectionError:
+    def __init__(self):
+        self.__resp = None
+
+        try:
+            self.__resp = requests.get("https://some-random-api.ml/animu/wink")
+        except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned,    200 expected!")
 
-    __resp = __resp.json()
+        self.__resp = self.__resp.json()
 
-    gif_link = __resp['link']
+        self.raw = self.__resp
+        self.gif_link = self.__resp['link']
 
-    @classmethod
-    def save_gif(cls, name: str='wink.gif'):
+    def save_gif(self, name: str = 'wink.gif'):
         """
         Saves the Wink GIF
 
         :param name: Image Name/PATH (Optional)
         :returns: GIF, bool
         :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise ImageNotFound: When failed to save Image
         """
         if not str(name).endswith(".gif"):
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".gif"!')
         path = name
         try:
-            r = requests.get(cls.gif_link, stream=True)
+            r = requests.get(self.gif_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the GIF. Status Code: {r.status_code} returned")
 
 
-class Quote():
+class Quote:
     """
     Returns a random Quote from Anime by attributes
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
-    try:
-        __resp = requests.get("https://some-random-api.ml/animu/quote")
-    except requests.exceptions.ConnectionError:
+    def __init__(self):
+        self.__resp = None
+
+        try:
+            self.__resp = requests.get("https://some-random-api.ml/animu/quote")
+        except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
-    __resp = __resp.json()
-
-    quote = __resp['sentence']
-    character = __resp['character']
-    anime_name = __resp['anime']
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned, 200 expected!")
+        self.__resp = self.__resp.json()
+
+        self.raw = self.__resp
+        self.quote = self.__resp['sentence']
+        self.character = self.__resp['character']
+        self.anime_name = self.__resp['anime']
 
-    @classmethod
-    def structured(cls):
+    def structured(self):
         """
         Returns a random Quote in a structured Way
 
         :returns: str
         """
 
-        return f"{cls.quote}\n-: {cls.character}/{cls.anime_name}"
+        return f"{self.quote}\n-: {self.character}/{self.anime_name}"
```

### Comparing `sra-pylib-1.3.1/sra/canvas.py` & `sra-pylib-1.4.0/sra/canvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,41 +4,53 @@
 import sra
 import re
 
 
 def is_valid_url(url):
     pattern = re.compile(
         r'^https?://'
-        r'([a-z0-9]+\.)*[a-z0-9]+\.[a-z]+/?'
-        r'([^\s/]+/?)+$'
+        r'(?:[a-z0-9]+(?:\.[a-z0-9]+)*/)*'
+        r'[a-z0-9]+\.[a-z]+/?$'
     )
     return bool(pattern.match(url))
 
 
-class Filter():
+def get_exact_avatar_url(url):
+    if "?" in str(url):
+        url = (str(url).split("?"))[0]
+    return url
+
+
+class Filter:
     """
     The Main Class of Canvas/Filter. Filter APIs are available as Sub-Class.
     """
 
-    @classmethod
-    def Blue(cls, avatar_url: str, name: str="image.png"):
+    def __init__(self):
+        self.__resp = None
+
+    def Blue(self, avatar_url: str, name: str = "image.png"):
         """
         Blueify your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -49,41 +61,44 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/filter/blue?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/blue?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def Blurple(cls, avatar_url: str, name: str="image.png"):
+    def Blurple(self, avatar_url: str, name: str = "image.png"):
         """
         Blurplify your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -94,41 +109,44 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/filter/blurple?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/blurple?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def Blurple2(cls, avatar_url: str, name: str="image.png"):
+    def Blurple2(self, avatar_url: str, name: str = "image.png"):
         """
         Blurplify your Avatar (New Discord blurple).
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -139,42 +157,46 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/filter/blurple2?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/blurple2?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def Brightness(cls, avatar_url: str, brightness: int=30, name: str="image.png"):
+    def Brightness(self, avatar_url: str, brightness: int = 30, name: str = "image.png"):
         """
         Brighten your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param brightness: The Brightness power (0 - 255)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
+        :raise InvalidBrightnessPower: When the Brightness Power is Invalid
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         if not 0 <= brightness <= 255:
             raise sra.exceptions.InvalidBrightnessPower("Brightness Power must be 0 - 255!")
         formats = ['.png', '.jpg', '.jpeg']
@@ -187,141 +209,155 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/filter/brightness?avatar={avatar_url}&brightness={brightness}", stream=True)
+            self.__resp = requests.get(
+                f"https://some-random-api.ml/canvas/filter/brightness?avatar={avatar_url}&brightness={brightness}",
+                stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def Color(cls, avatar_url: str, color: str, name: str="image.png"):
+    def Color(self, avatar_url: str, color: str, name: str = "image.png"):
         """
         Tint your Avatar a certain color. An alias of Tint
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param color: The Color Code in HEX without #
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise InvalidHEXColor: When HEX color code given, is invalid
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         if color.startswith("#"):
             color = color.replace("#", "", 1)
         if len(color) not in [6, 8]:
-            raise sra.exceptions.InvalidHEXColor(f"Given HEX Color Code must be 6 or 8 in length, but given code is {len(color)} in length")
+            raise sra.exceptions.InvalidHEXColor(
+                f"Given HEX Color Code must be 6 or 8 in length, but given code is {len(color)} in length")
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
 
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/color?color={color}&avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/color?color={color}&avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def Tint(cls, avatar_url: str, color: str, name: str="image.png"):
+    def Tint(self, avatar_url: str, color: str, name: str = "image.png"):
         """
         Tint your Avatar a certain color.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param color: The Color Code in HEX without #
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise InvalidHEXColor: When HEX color code given, is invalid
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         if color.startswith("#"):
             color = color.replace("#", "", 1)
         if len(color) not in [6, 8]:
-            raise sra.exceptions.InvalidHEXColor(f"Given HEX Color Code must be 6 or 8 in length, but given code is {len(color)} in length")
+            raise sra.exceptions.InvalidHEXColor(
+                f"Given HEX Color Code must be 6 or 8 in length, but given code is {len(color)} in length")
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
 
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/color?color={color}&avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/color?color={color}&avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def filter(cls, avatar_url: str, name: str="image.png"):
+    def Green(self, avatar_url: str, name: str = "image.png"):
         """
         Make your Avatar green like the Hulk.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -332,41 +368,44 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/filter/green?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/green?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def Greyscale(cls, avatar_url: str, name: str="image.png"):
+    def Greyscale(self, avatar_url: str, name: str = "image.png"):
         """
         Greyscale your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -377,41 +416,44 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/filter/greyscale?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/greyscale?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def InvertGrayscale(cls, avatar_url: str, name: str="image.png"):
+    def InvertGrayscale(self, avatar_url: str, name: str = "image.png"):
         """
         Invert and grayscale your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -422,41 +464,44 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/filter/invertgreyscale?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/invertgreyscale?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def Red(cls, avatar_url: str, name: str="image.png"):
+    def Red(self, avatar_url: str, name: str = "image.png"):
         """
         Redify your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -467,41 +512,43 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/filter/red?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/red?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def Sepia(cls, avatar_url: str, name: str="image.png"):
+    def Sepia(self, avatar_url: str, name: str = "image.png"):
         """
         Apply a sepia filter to your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -512,94 +559,105 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/filter/sepia?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/sepia?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def Threshold(cls, avatar_url: str, threshold: int=100, name: str="image.png"):
+    def Threshold(self, avatar_url: str, threshold: int = 100, name: str = "image.png"):
         """
         Threshold your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param threshold: Enter the Threshold integer
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
+        :raise ThresholdError: When the Threshold power is Invalid
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
 
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
+        if 0 > int(threshold) > 255:
+            raise sra.exceptions.ThresholdError("Threshold Power must be within 0 - 255!")
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/threshold?avatar={avatar_url}&threshold={threshold}", stream=True)
+            self.__resp = requests.get(
+                f"https://some-random-api.ml/canvas/threshold?avatar={avatar_url}&threshold={threshold}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
 
-class Misc():
+class Misc:
     """
-        The Main Class of Canvas/Misc. Misc APIs are available as Sub-Class.
+    The Main Class of Canvas/Misc. Misc APIs are available as Sub-Class.
     """
 
+    def __init__(self):
+        self.__resp = None
 
-    @classmethod
-    def BisexualBorder(cls, avatar_url: str, name: str="image.png"):
+    def BisexualBorder(self, avatar_url: str, name: str = "image.png"):
         """
         Add a bisex flag border to your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -610,41 +668,44 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/bisexual?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/bisexual?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def Blur(cls, avatar_url: str, name: str="image.png"):
+    def Blur(self, avatar_url: str, name: str = "image.png"):
         """
         Blur your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -655,88 +716,87 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/blur?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/blur?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def CircleCrop(cls, image_url: str, name: str="image.png"):
+    def CircleCrop(self, image_url: str, name: str = "image.png"):
         """
         Crop an image to a Circle.
 
         :param image_url: The URL of the Image
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
-        if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
-        if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
-            raise sra.exceptions.InvalidAvatarURL(
-                "Avatar Format must be '.jpg' or '.png'"
-            )
+        if not is_valid_url(image_url):
+            raise sra.exceptions.InvalidImageURL(
+                "Seems the Image URL is Invalid. Please recheck it and make sure it startswith http or https")
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
 
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/crop?avatar={image_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/crop?avatar={image_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def ColorViewer(cls, hex: str, name: str="image.png"):
+    def ColorViewer(self, hex: str, name: str = "image.png"):
         """
         View a color.
 
         :param hex: The Color Code in HEX without #
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise InvalidHEXColor: When HEX color code given, is invalid
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if hex.startswith("#"):
             hex = hex.replace("#", "", 1)
         if len(hex) not in [6, 8]:
-            raise sra.exceptions.InvalidHEXColor(f"Given HEX Color Code must be 6 or 8 in length, but given code is {len(hex)} in length")
+            raise sra.exceptions.InvalidHEXColor(
+                f"Given HEX Color Code must be 6 or 8 in length, but given code is {len(hex)} in length")
 
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
@@ -744,41 +804,43 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/colorviewer?hex={hex}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/colorviewer?hex={hex}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def HeartCrop(cls, image_url: str, name: str="image.png"):
+    def HeartCrop(self, avatar_url: str, name: str = "image.png"):
         """
         Crop an image to a heart shape
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -789,73 +851,73 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/heart?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/heart?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def RGBtoHEX(cls, rgb: str):
+    def RGBtoHEX(self, rgb: str):
         """
         Converts RGB code to HEX code
 
         :param rgb: Enter the RGB Code
         :return: HEX Code
+        :raise InvalidRGBCode: When the RGB Code given is invalid
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         codes = rgb.split(",")
         if len(codes) != 3:
             raise sra.exceptions.InvalidRGBCode(f"RGB Color Code must contains 3 blocks!")
 
-
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/hex?rgb={rgb}")
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/hex?rgb={rgb}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
 
-        if __resp.status_code == 200:
-            hex = __resp.json()['hex']
+        if self.__resp.status_code == 200:
+            hex = self.__resp.json()['hex']
             return hex
         else:
-            if __resp.status_code != 200:
-                if 'error' in __resp.json():
-                    raise sra.exceptions.APIError(__resp.json()['error'])
+            if self.__resp.status_code != 200:
+                if 'error' in self.__resp.json():
+                    raise sra.exceptions.APIError(self.__resp.json()['error'])
                 else:
                     raise sra.exceptions.APIError(
-                        f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
-
+                        f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned, 200 expected!")
 
-    @classmethod
-    def Horny(cls, avatar_url: str, name: str="image.png"):
+    def Horny(self, avatar_url: str, name: str = "image.png"):
         """
         Makes Horny card with the Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -866,41 +928,43 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/horny?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/horny?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def ItsSoStupid(cls, avatar_url: str, name: str="image.png"):
+    def ItsSoStupid(self, avatar_url: str, name: str = "image.png"):
         """
         Make an "Its so stupid" meme with your Avatar
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -911,41 +975,44 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/its-so-stupid?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/its-so-stupid?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def Jpg(cls, avatar_url: str, name: str="image.png"):
+    def Jpg(self, avatar_url: str, name: str = "image.png"):
         """
         Blur your Avatar. An alias of Blur
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -956,41 +1023,43 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/jpg?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/jpg?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def LesbianBorder(cls, avatar_url: str, name: str="image.png"):
+    def LesbianBorder(self, avatar_url: str, name: str = "image.png"):
         """
         Add a lesbian flag border to your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1001,41 +1070,44 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/lesbian?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/lesbian?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def LGBTBorder(cls, avatar_url: str, name: str="image.png"):
+    def LGBTBorder(self, avatar_url: str, name: str = "image.png"):
         """
         Add a lgbt flag border to your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1046,41 +1118,43 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/lgbt?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/lgbt?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def Lolice(cls, avatar_url: str, name: str="image.png"):
+    def Lolice(self, avatar_url: str, name: str = "image.png"):
         """
         Make Loli police to your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1091,44 +1165,48 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/lolice?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/lolice?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def GenshinNamecard(cls, avatar_url: str, username: str, birthday: str, description: typing.Optional[str]=None, name: str="image.png"):
+    def GenshinNamecard(self, avatar_url: str, username: str, birthday: str, description: typing.Optional[str] = None,
+                        name: str = "image.png"):
         """
         Make Genshin Namecard
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param username: A Username
         :param birthday: A Birthday
         :param description: A description (Optional)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1139,86 +1217,86 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/namecard?avatar={avatar_url}&birthday={birthday}&username={username}{'&description=' + description if description != None else ''}", stream=True)
+            self.__resp = requests.get(
+                f"https://some-random-api.ml/canvas/misc/namecard?avatar={avatar_url}&birthday={birthday}&username={username}{'&description=' + description if description is not None else ''}",
+                stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def NoBitches(cls, text, name: str="image.png"):
+    def NoBitches(self, text, name: str = "image.png"):
         """
         Make No Bitches Meme.
 
         :param text: The Text on the Meme
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
-        if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
-        if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
-            raise sra.exceptions.InvalidAvatarURL(
-                "Avatar Format must be '.jpg' or '.png'"
-            )
+
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
 
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/nobitches?no={urllib.parse.quote_plus(text)}", stream=True)
+            self.__resp = requests.get(
+                f"https://some-random-api.ml/canvas/nobitches?no={urllib.parse.quote_plus(text)}",
+                stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def NonbinaryBorder(cls, avatar_url: str, name: str="image.png"):
+    def NonbinaryBorder(self, avatar_url: str, name: str = "image.png"):
         """
         Make Nonbinary Bordered Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1229,131 +1307,123 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/nonbinary?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/nonbinary?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def Oogway(cls, quote: str, name: str="image.png"):
+    def Oogway(self, quote: str, name: str = "image.png"):
         """
         Make Oogway meme with custom quote.
 
         :param quote: The Custom Quote
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
-        if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
-        if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
-            raise sra.exceptions.InvalidAvatarURL(
-                "Avatar Format must be '.jpg' or '.png'"
-            )
+
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
 
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/oogway?quote={urllib.parse.quote_plus(quote)}", stream=True)
+            self.__resp = requests.get(
+                f"https://some-random-api.ml/canvas/misc/oogway?quote={urllib.parse.quote_plus(quote)}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def Oogway2(cls, quote: str, name: str="image.png"):
+    def Oogway2(self, quote: str, name: str = "image.png"):
         """
         Make Oogway meme with custom quote (Updated).
 
         :param quote: The Custom Quote
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
-        if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
-        if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
-            raise sra.exceptions.InvalidAvatarURL(
-                "Avatar Format must be '.jpg' or '.png'"
-            )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
 
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/oogway2?quote={urllib.parse.quote_plus(quote)}", stream=True)
+            self.__resp = requests.get(
+                f"https://some-random-api.ml/canvas/misc/oogway2?quote={urllib.parse.quote_plus(quote)}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def PansexualBorder(cls, avatar_url: str, name: str="image.png"):
+    def PansexualBorder(self, avatar_url: str, name: str = "image.png"):
         """
         Make Pansexual Bordered Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1364,41 +1434,44 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/pansexual?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/pansexual?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def Pixelate(cls, avatar_url: str, name: str="image.png"):
+    def Pixelate(self, avatar_url: str, name: str = "image.png"):
         """
         Make your Pixelated Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1409,75 +1482,78 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/pixelate?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/pixelate?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def HEXtoRGB(cls, hex: str):
+    def HEXtoRGB(self, hex: str):
         """
         Converts HEX code to RGB code.
 
-        :param hex: Enter the RGB Code
+        :param hex: Enter the HEX Code
         :return: RGB Code
+        :raise InvalidHEXColor: When HEX color code given, is invalid
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if hex.startswith("#"):
             hex = hex.replace("#", "", 1)
 
         if len(hex) not in [6, 8]:
-            raise sra.exceptions.InvalidHEXColor(f"Given HEX Color Code must be 6 or 8 in length, but given code is {len(hex)} in length")
+            raise sra.exceptions.InvalidHEXColor(
+                f"Given HEX Color Code must be 6 or 8 in length, but given code is {len(hex)} in length")
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/rgb?hex={hex}")
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/rgb?hex={hex}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
 
-        if __resp.status_code == 200:
-            __resp = __resp.json()
-            rgb = f"{__resp['r']}, {__resp['g']}, {__resp['b']}"
+        if self.__resp.status_code == 200:
+            self.__resp = self.__resp.json()
+            rgb = f"{self.__resp['r']}, {self.__resp['g']}, {self.__resp['b']}"
             return rgb
         else:
-            if __resp.status_code != 200:
-                if 'error' in __resp.json():
-                    raise sra.exceptions.APIError(__resp.json()['error'])
+            if self.__resp.status_code != 200:
+                if 'error' in self.__resp.json():
+                    raise sra.exceptions.APIError(self.__resp.json()['error'])
                 else:
                     raise sra.exceptions.APIError(
-                        f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+                        f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned, 200 expected!")
 
-
-    @classmethod
-    def SimpCard(cls, avatar_url: str, name: str="image.png"):
+    def SimpCard(self, avatar_url: str, name: str = "image.png"):
         """
         Make Simp Card with your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1488,41 +1564,44 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/simpcard?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/simpcard?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def Tonikawa(cls, avatar_url: str, name: str="image.png"):
+    def Tonikawa(self, avatar_url: str, name: str = "image.png"):
         """
         Make Tonikawa with your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1533,41 +1612,44 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/tonikawa?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/tonikawa?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def TransgenderBorder(cls, avatar_url: str, name: str="image.png"):
+    def TransgenderBorder(self, avatar_url: str, name: str = "image.png"):
         """
         Make Transgender Border with your Avatar
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1578,28 +1660,31 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/misc/transgender?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/transgender?avatar={avatar_url}",
+                                       stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
     themes = typing.Literal['light', 'dark', 'dim']
-    @classmethod
-    def Tweet(cls, display_name: str, username:str, avatar_url: str, comment: str, replyNumber: typing.Optional[int]=None, likeNumber: typing.Optional[int]=None, retweetNumber: typing.Optional[int]=None, theme: themes='light', name: str="image.png"):
+
+    def Tweet(self, display_name: str, username: str, avatar_url: str, comment: str,
+              replyNumber: typing.Optional[int] = None, likeNumber: typing.Optional[int] = None,
+              retweetNumber: typing.Optional[int] = None, theme: themes = 'light', name: str = "image.png"):
         """
         Make Fake Tweet
 
         :param display_name: The Display Name
         :param username: The Username
         :param avatar_url: URL of the Avatar
         :param comment: Comment for Fake Tweet
@@ -1607,28 +1692,35 @@
         :param likeNumber: Number of Likes will there be (Optional)
         :param retweetNumber: Number of retweets (Optional)
         :param theme: The Theme (Optional)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise DisplayNameError: When the Display Name doesn't meet the conditions
+        :raise UsernameError: When the Username doesn't meet the conditions
+        :raise CommentError: When the Comment doesn't meet the conditions
+        :raise ThemeError: When the Theme is Invalid
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if len(display_name) > 32:
             raise sra.exceptions.DisplayNameError("Display name length must be lesser than 32 characters!")
         if len(username) > 15:
             raise sra.exceptions.UsernameError("Username length must be lesser than 15 characters!")
         if len(comment) > 1000:
             raise sra.exceptions.CommentError("Comment length must be lesser than 1000 characters!")
         if theme.lower() not in ['light', 'dark', 'dim']:
             raise sra.exceptions.ThemeError("Invalid Theme! Theme must be light, dark or dim!")
         if not is_valid_url(avatar_url):
-            raise sra.exceptions.InvalidAvatarURL("Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+            raise sra.exceptions.InvalidAvatarURL(
+                "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
 
         formats = ['.png', '.jpg']
         validFormat = False
@@ -1640,49 +1732,52 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png" or ".jpg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/tweet?avatar={avatar_url}&displayname={urllib.parse.quote_plus(display_name)}&username={urllib.parse.quote_plus(username)}&comment={urllib.parse.quote_plus(comment)}{'&replies=' + str(replyNumber) if replyNumber != None else ''}{'&likes=' + str(likeNumber) if likeNumber != None else ''}{'&retweets=' + str(retweetNumber) if retweetNumber != None else ''}&theme={theme.lower()}", stream=True)
+            self.__resp = requests.get(
+                f"https://some-random-api.ml/canvas/tweet?avatar={avatar_url}&displayname={urllib.parse.quote_plus(display_name)}&username={urllib.parse.quote_plus(username)}&comment={urllib.parse.quote_plus(comment)}{'&replies=' + str(replyNumber) if replyNumber is not None else ''}{'&likes=' + str(likeNumber) if likeNumber is not None else ''}{'&retweets=' + str(retweetNumber) if retweetNumber is not None else ''}&theme={theme.lower()}",
+                stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def YoutubeComment(cls, username: str, avatar_url: str, comment: str, name: str="image.png"):
+    def YoutubeComment(self, username: str, avatar_url: str, comment: str, name: str = "image.png"):
         """
         Make Fake Youtube Comment.
 
         :param username: The Username
         :param avatar_url: URL of the Avatar
         :param comment: Comment for Fake Tweet
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if len(username) > 25:
             raise sra.exceptions.UsernameError("Username length must be lesser than 15 characters!")
         if len(comment) > 1000:
             raise sra.exceptions.CommentError("Comment length must be lesser than 1000 characters!")
 
         if not is_valid_url(avatar_url):
             raise sra.exceptions.InvalidAvatarURL(
                 "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg']
         validFormat = False
         for f in formats:
@@ -1693,48 +1788,55 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png" or ".jpg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/youtube-comment?avatar={avatar_url}&username={urllib.parse.quote_plus(username)}&comment={urllib.parse.quote_plus(comment)}",
-            stream=True)
+            self.__resp = requests.get(
+                f"https://some-random-api.ml/canvas/youtube-comment?avatar={avatar_url}&username={urllib.parse.quote_plus(username)}&comment={urllib.parse.quote_plus(comment)}",
+                stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
 
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
 
-class Overlay():
+class Overlay:
     """
     The Main Class of Canvas/Overlay. Overlay APIs are available as function.
     """
-    @classmethod
-    def Comrade(cls, avatar_url: str, name: str = "image.png"):
+
+    def __init__(self):
+        self.__resp = None
+
+    def Comrade(self, avatar_url: str, name: str = "image.png"):
         """
         Make Comraded Avatar
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
             raise sra.exceptions.InvalidAvatarURL(
                 "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1745,42 +1847,43 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/comrade?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/comrade?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def Gay(cls, avatar_url: str, name: str = "image.png"):
+    def Gay(self, avatar_url: str, name: str = "image.png"):
         """
         Give your Avatar a rainbow overlay.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
             raise sra.exceptions.InvalidAvatarURL(
                 "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1791,42 +1894,43 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/gay?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/gay?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def Glass(cls, avatar_url: str, name: str = "image.png"):
+    def Glass(self, avatar_url: str, name: str = "image.png"):
         """
         Give your Avatar a glass effect overlay
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
             raise sra.exceptions.InvalidAvatarURL(
                 "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1837,42 +1941,43 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/glass?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/glass?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def Jail(cls, avatar_url: str, name: str = "image.png"):
+    def Jail(self, avatar_url: str, name: str = "image.png"):
         """
         Make your Avatar Jailed
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
             raise sra.exceptions.InvalidAvatarURL(
                 "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1883,42 +1988,43 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/jail?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/jail?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def Passed(cls, avatar_url: str, name: str = "image.png"):
+    def Passed(self, avatar_url: str, name: str = "image.png"):
         """
         Mission passed overlay to your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
             raise sra.exceptions.InvalidAvatarURL(
                 "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -1929,42 +2035,43 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/passed?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/passed?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-
-    @classmethod
-    def Triggered(cls, avatar_url: str, name: str = "image.png"):
+    def Triggered(self, avatar_url: str, name: str = "image.gif"):
         """
         Get a Triggered GIF with your Avatar.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
             raise sra.exceptions.InvalidAvatarURL(
                 "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.gif']
         validFormat = False
         for f in formats:
@@ -1975,42 +2082,43 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".gif"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/triggered?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/triggered?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
-
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
 
-    @classmethod
-    def Wasted(cls, avatar_url: str, name: str = "image.png"):
+    def Wasted(self, avatar_url: str, name: str = "image.png"):
         """
         Give your Avatar a Wasted overlay.
 
         :param avatar_url: The URL of the Avatar (Format must be: .jpg or .png)
         :param name: Image Name/PATH (Optional)
         :return: Image, bool
         :raise InvalidFileFormat: When an unsupported file format is given
         :raise ImageNotFound: When failed to save Image
-        :raise InvalidAvatarURL: When Avatar URL doesn't meet the contidions
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise InvalidAvatarURL: When Avatar URL doesn't meet the conditions
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
         if not is_valid_url(avatar_url):
             raise sra.exceptions.InvalidAvatarURL(
                 "Seems the Avatar URL is Invalid. Please recheck it and make sure it startswith http or https")
+        avatar_url = get_exact_avatar_url(avatar_url)
         if not str(avatar_url).endswith(".jpg") and not str(avatar_url).endswith(".png"):
             raise sra.exceptions.InvalidAvatarURL(
                 "Avatar Format must be '.jpg' or '.png'"
             )
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
@@ -2021,16 +2129,17 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/canvas/wasted?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.ml/canvas/wasted?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __resp.status_code == 200:
+        if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
-                f.write(__resp.content)
+                f.write(self.__resp.content)
                 return True
         else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__resp.status_code} returned")
+            raise sra.exceptions.ImageNotFound(
+                f"Couldn't save the Image. Status Code: {self.__resp.status_code} returned")
```

### Comparing `sra-pylib-1.3.1/sra/exceptions.py` & `sra-pylib-1.4.0/sra/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,118 @@
 class ImageNotFound(Exception):
     """
     raises when it fails to save the Image from URL
     """
 
+
 class InvalidFileFormat(Exception):
     """
     raises when Invalid File Format is Given
     """
 
+
 class InvalidAvatarURL(Exception):
     """
     raises when the Avatar URL is Invalid
     """
 
+
+class InvalidImageURL(Exception):
+    """
+    raises when the Image URL is Invalid
+    """
+
+
 class InvalidHEXColor(Exception):
     """
     raises when given HEX Color Code in Invalid
     """
 
+
 class InvalidBrightnessPower(Exception):
     """
     raises when the Brightness Power is greater than 255 or lesser than 0
     """
 
-class InvalidResponse(Exception):
-    """
-    raises when API don't respond perfectly
-    """
 
 class InvalidRGBCode(Exception):
     """
     raises when RGB Code is Invalid
     """
 
+
 class DisplayNameError(Exception):
     """
     raises when Display name don't meet conditions
     """
 
+
 class UsernameError(Exception):
     """
     raises when Username don't meet conditions
     """
 
+
 class CommentError(Exception):
     """
     raises when Comment don't meet conditions
     """
 
+
 class ThemeError(Exception):
     """
     raises when Theme is Invalid
     """
 
-class InvalidAvatarFormat(Exception):
-    """
-    raises when Avatar URL is not .jpg or .png
-    """
 
 class APIError(Exception):
     """
     raises when API responses an error!
     """
 
+
 class APITimeout(Exception):
     """
     raises when API responses an error!
     """
 
+
 class ImageRetrieveError(Exception):
     """
     raises when API responses an error!
     """
 
+
+class InvalidTemplate(Exception):
+    """
+    raises when the Template is Invalid
+    """
+
+
+class InvalidBackground(Exception):
+    """
+    raises when the Background is Invalid
+    """
+
+
+class InvalidFont(Exception):
+    """
+    raises when the Font is Invalid
+    """
+
+
+class InvalidType(Exception):
+    """
+    raises when the Type is Invalid
+    """
+
+
+class InvalidTextColor(Exception):
+    """
+    raises when the Text Color is Invalid
+    """
+
+
+class ThresholdError(Exception):
+    """
+    raises when the Threshold Power is Invalid
+    """
```

### Comparing `sra-pylib-1.3.1/sra/image.py` & `sra-pylib-1.4.0/sra/animal.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,584 +1,541 @@
 import requests
 import sra
 
 
 class Bird:
     """
-    Returns a random Image Link about Bird by attributes
-
+    Returns an Image Link and a Fact about Bird
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
-    try:
-        __resp = requests.get("https://some-random-api.ml/img/bird")
-    except requests.exceptions.ConnectionError:
-        raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+    def __init__(self):
+        self.__resp = None
 
-    __resp = __resp.json()
+        try:
+            self.__resp = requests.get("https://some-random-api.ml/animal/bird")
+        except requests.exceptions.ConnectionError:
+            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned, 200 expected!")
 
-    image_link = __resp['link']
+        self.__resp = self.__resp.json()
 
-    @classmethod
-    def save_image(cls, name: str = "bird.png"):
+        self.image_link = self.__resp['image']
+        self.fact = self.__resp['fact']
+        self.raw = self.__resp
+
+    def save_image(self, name: str = "bird.png"):
         """
-        Saves the Image
+        Saves the Bird Image
 
         :param name: Image Name/PATH (Optional)
-        :return: Image, bool
+        :returns: Image, bool
+        :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
+        __r = None
         try:
-            __r = requests.get(cls.image_link, stream=True)
+            __r = requests.get(self.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
 class Cat:
     """
-    Returns a random Image Link about Cat by attributes
-
+    Returns an Image Link and a Fact about Cat
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
-    try:
-        __resp = requests.get("https://some-random-api.ml/img/cat")
-    except requests.exceptions.ConnectionError:
-        raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+    def __init__(self):
+        self.__resp = None
 
-    __resp = __resp.json()
+        try:
+            self.__resp = requests.get("https://some-random-api.ml/animal/cat")
+        except requests.exceptions.ConnectionError:
+            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned, 200 expected!")
+
+        self.__resp = self.__resp.json()
 
-    image_link = __resp['link']
+        self.image_link = self.__resp['image']
+        self.fact = self.__resp['fact']
+        self.raw = self.__resp
 
-    @classmethod
-    def save_image(cls, name: str = "cat.png"):
+    def save_image(self, name: str = "cat.png"):
         """
-        Saves the Image
+        Saves the Cat Image
 
         :param name: Image Name/PATH (Optional)
-        :return: Image, bool
+        :returns: Image, bool
+        :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
+        __r = None
         try:
-            __r = requests.get(cls.image_link, stream=True)
+            __r = requests.get(self.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
 class Dog:
     """
-    Returns a random Image Link about Dog by attributes
-
+    Returns an Image Link and a Fact about Dog
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
-    try:
-        __resp = requests.get("https://some-random-api.ml/img/dog")
-    except requests.exceptions.ConnectionError:
-        raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+    def __init__(self):
+        self.__resp = None
+
+        try:
+            self.__resp = requests.get("https://some-random-api.ml/animal/dog")
+        except requests.exceptions.ConnectionError:
+            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned, 200 expected!")
 
-    __resp = __resp.json()
+        self.__resp = self.__resp.json()
 
-    image_link = __resp['link']
+        self.image_link = self.__resp['image']
+        self.fact = self.__resp['fact']
+        self.raw = self.__resp
 
-    @classmethod
-    def save_image(cls, name: str = "dog.png"):
+    def save_image(self, name: str = "dog.png"):
         """
-        Saves the Image
+        Saves the Dog Image
 
         :param name: Image Name/PATH (Optional)
-        :return: Image, bool
+        :returns: Image, bool
+        :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
+        __r = None
         try:
-            __r = requests.get(cls.image_link, stream=True)
+            __r = requests.get(self.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
 class Fox:
     """
-    Returns a random Image Link about Fox by attributes
-
+    Returns an Image Link and a Fact about Fox
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
-    try:
-        __resp = requests.get("https://some-random-api.ml/img/fox")
-    except requests.exceptions.ConnectionError:
-        raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+    def __init__(self):
+        self.__resp = None
+
+        try:
+            self.__resp = requests.get("https://some-random-api.ml/animal/fox")
+        except requests.exceptions.ConnectionError:
+            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned, 200 expected!")
 
-    __resp = __resp.json()
+        self.__resp = self.__resp.json()
 
-    image_link = __resp['link']
+        self.image_link = self.__resp['image']
+        self.fact = self.__resp['fact']
+        self.raw = self.__resp
 
-    @classmethod
-    def save_image(cls, name: str = "fox.png"):
+    def save_image(self, name: str = "fox.png"):
         """
-        Saves the Image
+        Saves the Fox Image
 
         :param name: Image Name/PATH (Optional)
-        :return: Image, bool
+        :returns: Image, bool
+        :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
+        __r = None
         try:
-            __r = requests.get(cls.image_link, stream=True)
+            __r = requests.get(self.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
 class Kangaroo:
     """
-    Returns a random Image Link about Kangaroo by attributes
-
+    Returns an Image Link and a Fact about Kangaroo
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
-    try:
-        __resp = requests.get("https://some-random-api.ml/img/kangaroo")
-    except requests.exceptions.ConnectionError:
-        raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+    def __init__(self):
+        self.__resp = None
+
+        try:
+            self.__resp = requests.get("https://some-random-api.ml/animal/kangaroo")
+        except requests.exceptions.ConnectionError:
+            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned, 200 expected!")
 
-    __resp = __resp.json()
+        self.__resp = self.__resp.json()
 
-    image_link = __resp['link']
+        self.image_link = self.__resp['image']
+        self.fact = self.__resp['fact']
+        self.raw = self.__resp
 
-    @classmethod
-    def save_image(cls, name: str = "kangaroo.png"):
+    def save_image(self, name: str = "kangaroo.png"):
         """
-        Saves the Image
+        Saves the Kangaroo Image
 
         :param name: Image Name/PATH (Optional)
-        :return: Image, bool
+        :returns: Image, bool
+        :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
+        __r = None
         try:
-            __r = requests.get(cls.image_link, stream=True)
+            __r = requests.get(self.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
 class Koala:
     """
-    Returns a random Image Link about Koala by attributes
-
+    Returns an Image Link and a Fact about Koala
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
-    try:
-        __resp = requests.get("https://some-random-api.ml/img/koala")
-    except requests.exceptions.ConnectionError:
-        raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+    def __init__(self):
+        self.__resp = None
+
+        try:
+            self.__resp = requests.get("https://some-random-api.ml/animal/koala")
+        except requests.exceptions.ConnectionError:
+            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned, 200 expected!")
 
-    __resp = __resp.json()
+        self.__resp = self.__resp.json()
 
-    image_link = __resp['link']
+        self.image_link = self.__resp['image']
+        self.fact = self.__resp['fact']
+        self.raw = self.__resp
 
-    @classmethod
-    def save_image(cls, name: str = "koala.png"):
+    def save_image(self, name: str = "koala.png"):
         """
-        Saves the Image
+        Saves the Koala Image
 
         :param name: Image Name/PATH (Optional)
-        :return: Image, bool
+        :returns: Image, bool
+        :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
+        __r = None
         try:
-            __r = requests.get(cls.image_link, stream=True)
+            __r = requests.get(self.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
 class Panda:
     """
-    Returns a random Image Link about Panda by attributes
-
+    Returns an Image Link and a Fact about Panda
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
-    try:
-        __resp = requests.get("https://some-random-api.ml/img/panda")
-    except requests.exceptions.ConnectionError:
-        raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
-
-    __resp = __resp.json()
+    def __init__(self):
+        self.__resp = None
 
-    image_link = __resp['link']
-
-    @classmethod
-    def save_image(cls, name: str = "panda.png"):
-        """
-        Saves the Image
-
-        :param name: Image Name/PATH (Optional)
-        :return: Image, bool
-        """
-        formats = ['.png', '.jpg', '.jpeg']
-        validFormat = False
-        for f in formats:
-            if str(name).endswith(f):
-                validFormat = True
-                break
-        if not validFormat:
-            raise sra.exceptions.InvalidFileFormat(
-                'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
-        path = name
         try:
-            __r = requests.get(cls.image_link, stream=True)
+            self.__resp = requests.get("https://some-random-api.ml/animal/panda")
         except requests.exceptions.ConnectionError:
-            raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __r.status_code == 200:
-            with open(path, 'wb') as f:
-                f.write(__r.content)
-                return True
-        else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
+            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned, 200 expected!")
 
+        self.__resp = self.__resp.json()
 
-class Pikachu:
-    """
-    Returns a random Image Link about Pikachu by attributes
+        self.image_link = self.__resp['image']
+        self.fact = self.__resp['fact']
+        self.raw = self.__resp
 
-
-    :raise APITimeout: API taken too long to respond!
-    :raise APIError: Error Returned by API
-    """
-    try:
-        __resp = requests.get("https://some-random-api.ml/img/pikachu")
-    except requests.exceptions.ConnectionError:
-        raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
-
-    __resp = __resp.json()
-
-    image_link = __resp['link']
-
-    @classmethod
-    def save_image(cls, name: str = "pikachu.png"):
+    def save_image(self, name: str = "panda.png"):
         """
-        Saves the Image
+        Saves the Panda Image
 
         :param name: Image Name/PATH (Optional)
-        :return: Image, bool
+        :returns: Image, bool
+        :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
+        __r = None
         try:
-            __r = requests.get(cls.image_link, stream=True)
+            __r = requests.get(self.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
 class Raccoon:
     """
-    Returns a random Image Link about Raccoon by attributes
-
+    Returns an Image Link and a Fact about Raccoon
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
-    try:
-        __resp = requests.get("https://some-random-api.ml/img/raccoon")
-    except requests.exceptions.ConnectionError:
-        raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+    def __init__(self):
+        self.__resp = None
+
+        try:
+            self.__resp = requests.get("https://some-random-api.ml/animal/raccoon")
+        except requests.exceptions.ConnectionError:
+            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned, 200 expected!")
 
-    __resp = __resp.json()
+        self.__resp = self.__resp.json()
 
-    image_link = __resp['link']
+        self.image_link = self.__resp['image']
+        self.fact = self.__resp['fact']
+        self.raw = self.__resp
 
-    @classmethod
-    def save_image(cls, name: str = "raccoon.png"):
+    def save_image(self, name: str = "raccoon.png"):
         """
-        Saves the Image
+        Saves the Raccoon Image
 
         :param name: Image Name/PATH (Optional)
-        :return: Image, bool
+        :returns: Image, bool
+        :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
+        __r = None
         try:
-            __r = requests.get(cls.image_link, stream=True)
+            __r = requests.get(self.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
             raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
 
 
 class RedPanda:
     """
-    Returns a random Image Link about Red Panda by attributes
-
+    Returns an Image Link and a Fact about Red Panda
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
-    try:
-        __resp = requests.get("https://some-random-api.ml/img/red_panda")
-    except requests.exceptions.ConnectionError:
-        raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
-
-    __resp = __resp.json()
+    def __init__(self):
+        self.__resp = None
 
-    image_link = __resp['link']
-
-    @classmethod
-    def save_image(cls, name: str = "red panda.png"):
-        """
-        Saves the Image
-
-        :param name: Image Name/PATH (Optional)
-        :return: Image, bool
-        """
-        formats = ['.png', '.jpg', '.jpeg']
-        validFormat = False
-        for f in formats:
-            if str(name).endswith(f):
-                validFormat = True
-                break
-        if not validFormat:
-            raise sra.exceptions.InvalidFileFormat(
-                'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
-        path = name
         try:
-            __r = requests.get(cls.image_link, stream=True)
+            self.__resp = requests.get("https://some-random-api.ml/animal/red_panda")
         except requests.exceptions.ConnectionError:
-            raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
-        if __r.status_code == 200:
-            with open(path, 'wb') as f:
-                f.write(__r.content)
-                return True
-        else:
-            raise sra.exceptions.ImageNotFound(f"Couldn't save the Image. Status Code: {__r.status_code} returned")
-
-
-class Whale:
-    """
-    Returns a random Image Link about Whale by attributes
-
-
-    :raise APITimeout: API taken too long to respond!
-    :raise APIError: Error Returned by API
-    """
-    try:
-        __resp = requests.get("https://some-random-api.ml/img/whale")
-    except requests.exceptions.ConnectionError:
-        raise sra.exceptions.APITimeout("API taken too long to respond!")
-    if __resp.status_code != 200:
-        if 'error' in __resp.json():
-            raise sra.exceptions.APIError(__resp.json()['error'])
-        else:
-            raise sra.exceptions.APIError(
-                f"API is  Down now, Please try again later!\nStatus Code: {__resp.status_code} returned, 200 expected!")
+            raise sra.exceptions.APITimeout("API taken too long to respond!")
+        if self.__resp.status_code != 200:
+            if 'error' in self.__resp.json():
+                raise sra.exceptions.APIError(self.__resp.json()['error'])
+            else:
+                raise sra.exceptions.APIError(
+                    f"API is  Down now, Please try again later!\nStatus Code: {self.__resp.status_code} returned, 200 expected!")
 
-    __resp = __resp.json()
+        self.__resp = self.__resp.json()
 
-    image_link = __resp['link']
+        self.image_link = self.__resp['image']
+        self.fact = self.__resp['fact']
+        self.raw = self.__resp
 
-    @classmethod
-    def save_image(cls, name: str = "whale.png"):
+    def save_image(self, name: str = "red panda.png"):
         """
-        Saves the Image
+        Saves the Red Panda Image
 
         :param name: Image Name/PATH (Optional)
-        :return: Image, bool
+        :returns: Image, bool
+        :raise InvalidFileFormat: When an unsupported file format given
+        :raise ImageRetrieveError: Raises when failed to retrieve the Image
+        :raise ImageNotFound: When failed to save Image
         """
         formats = ['.png', '.jpg', '.jpeg']
         validFormat = False
         for f in formats:
             if str(name).endswith(f):
                 validFormat = True
                 break
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
+        __r = None
         try:
-            __r = requests.get(cls.image_link, stream=True)
+            __r = requests.get(self.image_link, stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __r.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(__r.content)
                 return True
         else:
```

### Comparing `sra-pylib-1.3.1/sra/pokemon.py` & `sra-pylib-1.4.0/sra/pokemon.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 class Ability:
     """
     Get Pokemon ability information
     """
 
     def __init__(self, ability: str):
         """
-        Returns the id, name, generation, effects, description, pokemons, descriptions and raw response by attributes
+        :returns: id, name, generation, effects, description, pokemons, descriptions and raw response by attributes
 
         :param ability: Ability Name/ID
+        :raise APITimeout: API taken too long to respond!
+        :raise APIError: Error Returned by API
         """
         self.id, self.name, self.generation, self.effects, self.description, self.pokemons, self.descriptions, self.raw = self.__getability(
             ability)
 
     @staticmethod
     def __getability(ability):
         try:
@@ -48,17 +50,19 @@
 class Item:
     """
     Get Pokemon item information
     """
 
     def __init__(self, item: str):
         """
-        Returns the id, name, effects, cost, attributes, category, sprite, descriptions and raw response by attributes
+        :returns: id, name, effects, cost, attributes, category, sprite, descriptions and raw response by attributes
 
         :param item: Item Name/ID
+        :raise APITimeout: API taken too long to respond!
+        :raise APIError: Error Returned by API
         """
         self.id, self.name, self.effects, self.cost, self.attributes, self.category, self.sprite, self.descriptions, self.raw = self.__getitem(
             item)
 
     @staticmethod
     def __getitem(item):
         try:
@@ -87,17 +91,19 @@
 class Move:
     """
     Get Pokemon move information
     """
 
     def __init__(self, move: str):
         """
-        Returns the id, name, generation, effects, type, category, contest, pp, power, accuracy, priority, pokemon, descriptions and raw response by attributes
+        :returns: the id, name, generation, effects, type, category, contest, pp, power, accuracy, priority, pokemon, descriptions and raw response by attributes
 
         :param move: Move Name/ID
+        :raise APITimeout: API taken too long to respond!
+        :raise APIError: Error Returned by API
         """
         self.id, self.name, self.generation, self.effects, self.type, self.category, self.contest, self.pp, self.power, self.accuracy, self.priority, self.pokemon, self.descriptions, self.raw = self.__getmove(
             move)
 
     @staticmethod
     def __getmove(move):
         try:
@@ -131,17 +137,19 @@
 class Pokedex:
     """
     Get Pokemon information
     """
 
     def __init__(self, pokemon: str):
         """
-        Returns the id, name, generation, effects, description, pokemons, descriptions and raw response by attributes
+        :returns: the id, name, generation, effects, description, pokemons, descriptions and raw response by attributes
 
         :param pokemon: Pokemon Name
+        :raise APITimeout: API taken too long to respond!
+        :raise APIError: Error Returned by API
         """
         self.name, self.id, self.type, self.species, self.abilities, self.height, self.weight, self.base_experience, self.gender, self.egg_groups, self.stats, self.family, self.sprites, self.description, self.generation, self.raw = self.__getpokemon(
             pokemon)
 
     def __getpokemon(self, pokemon):
         try:
             __resp = requests.get(f"https://some-random-api.ml/pokemon/pokedex?pokemon={urllib.parse.quote_plus(pokemon)}")
@@ -164,36 +172,36 @@
         weight = __resp['weight']
         base_experience = __resp['base_experience']
         gender = __resp['gender']
         egg_groups = __resp['egg_groups']
 
         class Stats:
             def __init__(self, stats_dict):
-                self.stats_dict = stats_dict
+                self.raw = stats_dict
                 self.hp = stats_dict['hp']
                 self.attack = stats_dict['attack']
                 self.defense = stats_dict['defense']
                 self.sp_atk = stats_dict['sp_atk']
                 self.sp_def = stats_dict['sp_def']
                 self.speed = stats_dict['speed']
                 self.total = stats_dict['total']
 
         stats = Stats(__resp['stats'])
 
         class Family:
             def __init__(self, family_dict):
-                self.family_dict = family_dict
+                self.raw = family_dict
                 self.evolutionStage = family_dict['evolutionStage']
                 self.evolutionLine = family_dict['evolutionLine']
 
         family = Family(__resp['family'])
 
         class Sprite:
             def __init__(self, sprites_dict):
-                self.sprites_dict = sprites_dict
+                self.raw = sprites_dict
                 self.normal = sprites_dict['normal']
                 self.animated = sprites_dict['animated']
 
         sprites = Sprite(__resp["sprites"])
 
         description = __resp['description']
         generation = __resp['generation']
```

