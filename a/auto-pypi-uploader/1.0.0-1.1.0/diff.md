# Comparing `tmp/auto_pypi_uploader-1.0.0.tar.gz` & `tmp/auto_pypi_uploader-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_pypi_uploader-1.0.0.tar", last modified: Tue Apr 11 05:53:21 2023, max compression
+gzip compressed data, was "auto_pypi_uploader-1.1.0.tar", last modified: Tue Apr 11 11:50:24 2023, max compression
```

## Comparing `auto_pypi_uploader-1.0.0.tar` & `auto_pypi_uploader-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 05:53:21.736328 auto_pypi_uploader-1.0.0/
--rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 auto_pypi_uploader-1.0.0/LICENSE
--rw-r--r--   0 Huck       (503) staff       (20)    13237 2023-04-11 05:53:21.736105 auto_pypi_uploader-1.0.0/PKG-INFO
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 05:53:21.735127 auto_pypi_uploader-1.0.0/auto_pypi_uploader/
--rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 10:25:11.000000 auto_pypi_uploader-1.0.0/auto_pypi_uploader/__init__.py
--rw-r--r--   0 Huck       (503) staff       (20)     5956 2023-04-11 05:41:36.000000 auto_pypi_uploader-1.0.0/auto_pypi_uploader/pypi_uploader.py
--rw-r--r--   0 Huck       (503) staff       (20)    11437 2023-04-11 05:34:10.000000 auto_pypi_uploader-1.0.0/auto_pypi_uploader/setup_file_creator.py
-drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 05:53:21.735914 auto_pypi_uploader-1.0.0/auto_pypi_uploader.egg-info/
--rw-r--r--   0 Huck       (503) staff       (20)    13237 2023-04-11 05:53:21.000000 auto_pypi_uploader-1.0.0/auto_pypi_uploader.egg-info/PKG-INFO
--rw-r--r--   0 Huck       (503) staff       (20)      333 2023-04-11 05:53:21.000000 auto_pypi_uploader-1.0.0/auto_pypi_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-11 05:53:21.000000 auto_pypi_uploader-1.0.0/auto_pypi_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 Huck       (503) staff       (20)       20 2023-04-11 05:53:21.000000 auto_pypi_uploader-1.0.0/auto_pypi_uploader.egg-info/requires.txt
--rw-r--r--   0 Huck       (503) staff       (20)       19 2023-04-11 05:53:21.000000 auto_pypi_uploader-1.0.0/auto_pypi_uploader.egg-info/top_level.txt
--rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-11 05:53:21.736373 auto_pypi_uploader-1.0.0/setup.cfg
--rw-r--r--   0 Huck       (503) staff       (20)     1370 2023-04-11 05:53:21.000000 auto_pypi_uploader-1.0.0/setup.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 11:50:24.937166 auto_pypi_uploader-1.1.0/
+-rw-r--r--   0 Huck       (503) staff       (20)     1103 2023-04-09 20:11:22.000000 auto_pypi_uploader-1.1.0/LICENSE
+-rw-r--r--   0 Huck       (503) staff       (20)    13740 2023-04-11 11:50:24.937000 auto_pypi_uploader-1.1.0/PKG-INFO
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 11:50:24.936111 auto_pypi_uploader-1.1.0/auto_pypi_uploader/
+-rw-r--r--   0 Huck       (503) staff       (20)        0 2023-04-10 10:25:11.000000 auto_pypi_uploader-1.1.0/auto_pypi_uploader/__init__.py
+-rw-r--r--   0 Huck       (503) staff       (20)     6515 2023-04-11 11:49:27.000000 auto_pypi_uploader-1.1.0/auto_pypi_uploader/pypi_uploader.py
+-rw-r--r--   0 Huck       (503) staff       (20)    11928 2023-04-11 10:41:50.000000 auto_pypi_uploader-1.1.0/auto_pypi_uploader/setup_file_creator.py
+drwxr-xr-x   0 Huck       (503) staff       (20)        0 2023-04-11 11:50:24.936805 auto_pypi_uploader-1.1.0/auto_pypi_uploader.egg-info/
+-rw-r--r--   0 Huck       (503) staff       (20)    13740 2023-04-11 11:50:24.000000 auto_pypi_uploader-1.1.0/auto_pypi_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 Huck       (503) staff       (20)      333 2023-04-11 11:50:24.000000 auto_pypi_uploader-1.1.0/auto_pypi_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 Huck       (503) staff       (20)        1 2023-04-11 11:50:24.000000 auto_pypi_uploader-1.1.0/auto_pypi_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       37 2023-04-11 11:50:24.000000 auto_pypi_uploader-1.1.0/auto_pypi_uploader.egg-info/requires.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       19 2023-04-11 11:50:24.000000 auto_pypi_uploader-1.1.0/auto_pypi_uploader.egg-info/top_level.txt
+-rw-r--r--   0 Huck       (503) staff       (20)       38 2023-04-11 11:50:24.937211 auto_pypi_uploader-1.1.0/setup.cfg
+-rw-r--r--   0 Huck       (503) staff       (20)     1415 2023-04-11 11:50:24.000000 auto_pypi_uploader-1.1.0/setup.py
```

### Comparing `auto_pypi_uploader-1.0.0/LICENSE` & `auto_pypi_uploader-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_pypi_uploader-1.0.0/PKG-INFO` & `auto_pypi_uploader-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: auto_pypi_uploader
-Version: 1.0.0
-Summary: A program to automate the creation of the 'setup.py' file, changing a pip package's version & publishing it to PyPi.
+Version: 1.1.0
+Summary: A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi.
 Home-page: https://github.com/Huckdirks/auto-pypi-exporter
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
+License: MIT
 Keywords: PyPi,Pip,setup,setup.py,automation
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,153 +19,164 @@
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Uses](#uses)
     - [Running from Command Line](#running-from-command-line)
     - [Running with Command Line Arguments](#running-with-command-line-arguments)
     - [Importing as a Module](#importing-as-a-module)
+        - [Installing with pip](#installing-with-pip)
         - [`create_setup()`](#create_setup-takes-in)
         - [`set_login()`](#set_login-takes-in)
         - [`pypi_upload()`](#pypi_upload-takes-in)
 - [Running](#running)
     - [Dependencies](#dependencies)
     - [Setting Up .env File](#setting-up-env-file)
     - [Running](#running-1)
 - [Quality Assurance](#quality-assurance)
 - [Suggestions](#suggestions)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Introduction
 
-While working on my previous project: [text-excuse-generator](https://github.com/Huckdirks/text-excuse-generator), I just published my first package to [PyPi](https://pypi.org/project/text-excuse-generator/). I quickly realized that I wasn't going to be able to remember the command line arguments to pass into the required fields, and that I was bound to forget to change the version manually in the `setup.py` file every time I updated the package. So I decided to make a program that would automatically update the version number in the `setup.py` file and export my project to [PyPi](https://pypi.org/). I also added another script that would automatically create a `setup.py` file for me with the required fields.
+While working on my previous project: [text-excuse-generator](https://github.com/Huckdirks/text-excuse-generator), I just published my first package to [PyPi](https://pypi.org/project/text-excuse-generator/). I quickly realized that I wasn't going to be able to remember the command line arguments to pass into the required fields, and that I was bound to forget to change the version manually in the `setup.py` file every time I updated the package. So I decided to make a program that would automatically update the version number in the `setup.py` file and export a project to [PyPi](https://pypi.org/). I also added another script that would automatically create a `setup.py` file for me with the required fields.
 
 ## Uses
 
 There are three main ways to interact with the program: by [running it in the command line](#running-from-command-line), by [running it with command line arguments](#running-with-command-line-arguments), or by [importing it](#importing-as-a-module) into another python file.
 
 In order for this program to run, your project's directory must be set up as such:
 Any files and directories in **[ ]**'s are optional, **but highly recommended!!!**
-```bash
+```
 project_root_dir/
-    [LICENSE]
+    pypi_uploader.py (can be downloaded from auto_pypi_uploader/ or substituted with a program that imports the module)
+    setup.py (can be created with pypi_uploader.py or setup_file_creator.py)
     [README.md] (can also be in docs/)
+    [LICENSE]
+
     main_module_name/
             __init__.py
             (other python files...)
+
     [docs/]
-    setup.py (can be created with pypi_uploader.py or setup_file_creator.py)
-    pypi_uploader.py (can be downloaded from include/ or substituted with a program that imports the module)
+            [README.md]
 ```
 
 
 You can also have multiple modules in the same directory, or even multiple modules within a module, but you will need to add the `__init__.py` file to each directory that contains a module. e.g.
-```bash
+```
 project_root_dir/
-    [LICENSE]
+    pypi_uploader.py (can be downloaded from auto_pypi_uploader/ or substituted with a program that imports the module)
+    setup.py (can be created with pypi_uploader.py or setup_file_creator.py)
     [README.md] (can also be in docs/)
+    [LICENSE]
+
     main_module_name/
             __init__.py
             (other python files...)
             main_submodule_name/
                     __init__.py
                     (other python files...)
+
     secondary_module_name/
             __init__.py
             (other python files...)
+
     [docs/]
-    setup.py (can be created with pypi_uploader.py or setup_file_creator.py)
-    pypi_uploader.py (can be downloaded from include/ or substituted with a program that imports the module)
+            [README.md]
 ```
 
 ### Running from Command Line
 
-I'd recommend downloading [pypi_uploader.py](../include/pypi_uploader.py) from [include](../include/pypi_uploader.py) into a project's [root directory](../) if you want the functionality of the whole module. Or just [setup_file_creator](../include/setup_file_creator.py) if you only want to make a `setup.py` file. You can run the program by typing:
+I'd recommend downloading [pypi_uploader.py](../include/pypi_uploader.py) from [include](../include/pypi_uploader.py) into a project's [root directory](../) if you want the functionality of the whole module, or just [`setup_file_creator.py`](../auto_pypi_uploader/setup_file_creator.py) if you only want to make a `setup.py` file. You can run the program by typing:
 ```bash
 python3 pypi_uploader.py
 ```
 
-When you run the program normally, it will first check if a `setup.py` file exists in the current directory. If it doesn't, it will then run [`setup_file_creator`](../include/setup_file_creator.py)`.create_setup()`, which will ask you for:
+When you run the program normally, it will first check if a `setup.py` file exists in the current directory. If it doesn't, it will then run [`setup_file_creator`](../auto_pypi_uploader/setup_file_creator.py)`.create_setup()`, which will ask you for:
 - The Project's Name
 - The Project's Version
 - The Project's Author
 - The Project's Description
 
 And ask you if you want to add these optional fields:
+- The Project's License
 - The Project's Long Description Type (From [README.md](README.md))
 - The Project's URL
 - The Required Packages
 - Keywords
 - Classifiers
 - Minimum Python Version
 
 *If you just want to create a `setup.py` file, run:*
 ```bash
 python3 setup_file_creator.py
 ```
 
 
-If a `setup.py` file already exists, `pypi_uploader.py` will then ask you for a new version number, and update it in `setup.py`. It will then upload the package to [PyPi](https://pypi.org/). If you haven't already set up your login credentials, it will then ask you for your username and password & save it, and then proceed to upload the package.
+If a `setup.py` file already exists, [`pypi_uploader.py`](../auto_pypi_uploader/pypi_uploader.py) will then ask you for a new version number, and update it in `setup.py`. It will then upload the package to [PyPi](https://pypi.org/). If you haven't already set up your login credentials, it will then ask you for your username and password & save it, and then proceed to upload the package. It then automatically updates/ installs the package with `pip3 install --upgrade {project_name}`.
 
 The program runs: `python3 setup.py sdist bdist_wheel` and `python3 twine upload dist/* -u "{USERNAME}" -p "{PASSWORD}"` to upload the package to [PyPi](https://pypi.org/).
 
 ### Running with Command Line Arguments
 
-You can also run the program with command line arguments. If you want to send the text message, you can add `--send` or `-s` as the last argument. All command line arguments longer than a single word need to be in parentheses. I'd recommend downloading [pypi_uploader.py](../include/pypi_uploader.py) from [include](../include/pypi_uploader.py) into a project's [root directory](../) if you want all the functionality, or just [setup_file_creator](../include/setup_file_creator.py) if you only want to make a `setup.py` file, and running them from the command line. Please also include the [LICENSE](../LICENSE) file in the same directory as any files you add from [this project](https://github.com/Huckdirks/auto-pypi-uploader).
+You can also run the program with command line arguments. If you want to send the text message, you can add `--send` or `-s` as the last argument. All command line arguments longer than a single word need to be in parentheses. I'd recommend downloading [`pypi_uploader.py`](../auto_pypi_uploader/pypi_uploader.py) into a project's [root directory](../) if you want all the functionality, or just [`setup_file_creator.py`](../auto_pypi_uploader/setup_file_creator.py) if you only want to make a `setup.py` file, and running them from the command line. Please also include the [LICENSE](../LICENSE) file in the same directory as any files you add from [this project](https://github.com/Huckdirks/auto-pypi-uploader).
 
 #### **Creating a `setup.py` File**
 
 If you want to create a `setup.py` file, run:
 ```bash
-python3 setup_file_creator.py --name PROJECT_NAME --version VERSION --author AUTHOR --description DESCRIPTION [--long_description_content_type LONG_DESCRIPTION_TYPE] [--url URL] [--install_requires "INSTALL_REQUIRES"] [--keywords "KEYWORDS"] [--classifiers "CLASSIFIERS"] [--python_requires PYTHON_REQUIRES]
+python3 setup_file_creator.py --name PROJECT_NAME --version VERSION --author AUTHOR --description DESCRIPTION [--license LICENSE] [--long_description_content_type LONG_DESCRIPTION_TYPE] [--url URL] [--install_requires "INSTALL_REQUIRES"] [--keywords "KEYWORDS"] [--classifiers "CLASSIFIERS"] [--python_requires PYTHON_REQUIRES]
 ```
 Any parameters in [ ]'s are optional, and all parameters in " "'s can be a comma separated list: e.g.
 ```bash
-python3 setup_file_creator.py -n auto_pypi_uploader -v "1.0.0" -a "Huck Dirksmeier" -d "A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi." -l text/markdown -u https://github.com/Huckdirks/auto-pypi-uploader -i "twine, python-dotenv" -k "PyPi, Pip, setup, setup.py, automation" -c "Programming Language :: Python, License :: MIT License, Operating System :: OS Independent" -p ">=3.8"
+python3 setup_file_creator.py -n auto_pypi_uploader -v "1.0.0" -a "Huck Dirksmeier" -d "A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi." -l MIT -ld text/markdown -u https://github.com/Huckdirks/auto-pypi-uploader -i "twine, python-dotenv" -k "PyPi, Pip, setup, setup.py, automation" -c "Programming Language :: Python, License :: OSI Approved :: MIT License, Operating System :: OS Independent" -p ">=3.8"
 ```
 
 #### **Uploading [PyPi](https://pypi.org/) Package & Adding Login Information**
 If you want to upload a package to [PyPi](https://pypi.org/), run:
 ```bash
-python3 pypi_uploader.py [VERSION] [--user USERNAME PASSWORD]
+python3 pypi_uploader.py VERSION [--user USERNAME PASSWORD]
 ```
 e.g.
 ```bash
 python3 pypi_uploader.py "1.0.0" -u Huckdirks PASSWORD
 ```
-This assumes that you've already made a `setup.py` file. If you just want to update the version number, run `python3 pypi_uploader.py [VERSION]`. This assumes that you've already set up your login credentials. To just add login credentials, run `python3 pypi_uploader.py --user USERNAME PASSWORD`. This will add your username and password to a `.env` file in the current directory. If you decide to update the version & login information in a single call, **make sure the version is the first argument!** **YOU ONLY NEED TO ADD YOUR LOGIN INFORMATION ONCE, OTHERWISE IT WILL OVERRIDE THE PREVIOUS LOGIN INFORMATION!!!**
+This assumes that you've already made a `setup.py` file. If you just want to update the version number, run `python3 pypi_uploader.py VERSION`. This assumes that you've already set up your login credentials. To just add login credentials, run `python3 pypi_uploader.py --user USERNAME PASSWORD`. This will add your username and password to a `.env` file in the current directory. If you decide to update the version & login information in a single call, **make sure the version is the first argument!** **YOU ONLY NEED TO ADD YOUR LOGIN INFORMATION ONCE, OTHERWISE IT WILL OVERRIDE THE PREVIOUS LOGIN INFORMATION!!!**
 
 ### Importing as a Module
 
-You can also import the program as a module into another python file. The `auto_pypi_uploader` module has  two sub-modules:
-- `setup_file_creator` has one function: `create_setup()`
-- `pypi_uploader` has two functions: `pypi_upload()` and `set_login()`
+You can also import the program as a module into another python file.
 
 #### Installing with pip
 
 Simply run:
 ```bash
 pip install auto-pypi-uploader
 ```
+ The `auto_pypi_uploader` module has  two sub-modules:
+- `setup_file_creator` has one function: [`create_setup()`](#create_setup-takes-in)
+- `pypi_uploader` has two functions: [`pypi_upload()`](#pypi_upload-takes-in) and [`set_login()`](#set_login-takes-in)
+
 To import the modules into your python file, put this at the top of your file:
 ```python
 from auto_pypi_uploader.pypi_uploader import *
 from auto_pypi_uploader.setup_file_creator import *
 ```
 Or you can import the individual functions.
 
 #### `create_setup()` takes in:
 ```python
-create_setup(NAME: str, VERSION: str, AUTHOR: str, DESCRIPTION: str, help: bool, long_description_content_type: str, url: str, install_requires: list[str], keywords: list[str], classifiers: list[str], python_requires: str) -> bool
+create_setup(NAME: str, VERSION: str, AUTHOR: str, DESCRIPTION: str, help: bool, license: str, long_description_content_type: str, url: str, install_requires: list[str], keywords: list[str], classifiers: list[str], python_requires: str) -> bool
 ```
 `create_setup()` returns True if able to generate `setup.py` and False if not. **All uppercase parameters are required if parameters are passed in, and each parameter must be defined in the function call. You can also omit all parameters, and the function will prompt you for each one manually.**
 
 If you want to create a `setup.py` file, call the function like this:
 ```python
-create_setup(name = "auto_pypi_uploader", version = "1.0.0", author = "Huck Dirksmeier", description = "A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi.", long_description_content_type = "text/markdown", url = "https://github.com/Huckdirks/auto-pypi-uploader", install_requires = ["twine", "python-dotenv"], keywords = ["PyPi", "Pip", "setup", "setup.py", "automation"], classifiers = ["Programming Language :: Python", "License :: MIT License", "Operating System :: OS Independent"], python_requires = ">=3.8")
+create_setup(name = "auto_pypi_uploader", version = "1.0.0", author = "Huck Dirksmeier", description = "A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi.", license = "MIT", long_description_content_type = "text/markdown", url = "https://github.com/Huckdirks/auto-pypi-uploader", install_requires = ["twine", "python-dotenv"], keywords = ["PyPi", "Pip", "setup", "setup.py", "automation"], classifiers = ["Programming Language :: Python", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"], python_requires = ">=3.8")
 ```
 Make sure to put the fields before the variables when calling the function.
 
 #### `set_login()` takes in:
 ```python
 set_login(USERNAME: str, PASSWORD: str) -> None
 ```
@@ -172,15 +184,15 @@
 ```python
 set_login("USERNAME", "PASSWORD")
 ```
 If you want user input, just call [`pypi_upload()`](#pypi_upload-takes-in).
 
 #### `pypi_upload()` takes in:
 ```python
-pypi_upload(VERSION: str, USERNAME: str, PASSWORD: str) -> bool
+pypi_upload(VERSION: str, username: str, password: str) -> bool
 ```
 `pypi_upload()` returns True if the package was successfully uploaded, and False if it wasn't. **All uppercase parameters are required if parameters are passed in, and each parameter must be defined in the function call. You can also omit all parameters, and the function will prompt you for the version, and the login info if not previously saved.**
 If you want to upload a package & login to [PyPi](https://pypi.org/), call `pypi_upload()` like this:
 ```python
 pypi_upload(version = "0.0.0", username = "USERNAME", password = "PASSWORD")
 ```
 
@@ -205,15 +217,15 @@
 Either run the program without any arguments to manually input the information for the .env file, run with [command line arguments](#setting-up-env-file) to automatically input the information for the .env file, or pass in the correct parameters to the [`set_login()`](#set_login-takes-in) or [`pypi_upload()`](#pypi_upload-takes-in) function.
 
 ### Running
 
 **YOU HAVE TO INSTALL THE DEPENDENCIES & SETUP THE `.env` FILE BEFORE TRYING TO RUN THE PROGRAM!!!**
 If installed with pip, all dependencies should be installed automatically!
 
-Run `python3 text_excuse_generator.py` or `python3 text_excuse_generator.py [sender] [recipient] [problem] [excuse] [--send_text_flag]` in the command line in the source directory.
+Run [`python3 pypi_uploader.py`](#running-from-command-line) or [`python3 pypi_uploader.py VERSION [--user USERNAME PASSWORD]`](#running-with-command-line-arguments) in the command line in the source directory.
 
 More detailed instructions are in the [Uses](#uses) section.
 
 ## Quality Assurance
 All variable, function, class, module, & file names are written in [snake_case](https://en.wikipedia.org/wiki/Snake_case) to make sure everything is consistent, and all `const` variables are written in ALL-CAPS. The code is also quite commented and the variable names are quite verbose, so it should be easy enough to understand what's going on.
 
 If there are any other/better ways to check for quality assurance, please let me know in the [suggestions](https://github.com/Huckdirks/auto-pip-exporter/discussions/new?category=suggestions)!
```

### Comparing `auto_pypi_uploader-1.0.0/auto_pypi_uploader/pypi_uploader.py` & `auto_pypi_uploader-1.1.0/auto_pypi_uploader/pypi_uploader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Imported Libraries
 from dotenv import load_dotenv
-from setup_file_creator import create_setup
+# from setup_file_creator import create_setup
+from auto_pypi_uploader.setup_file_creator import create_setup
 
 # Python Libraries
 from os import getenv, system, getcwd
 from os.path import dirname, join, isfile
 from sys import argv
 from getpass import getpass
+from time import sleep
+import re
 
 # Constants
 ENV_NAME = "pypi_account_info.env"  # CHANGE THIS TO YOUR ENVIRONMENT NAME (.env file)
 ENV_PATH = join(dirname(__file__), ENV_NAME)
-SETUP_PATH = getcwd() + "/setup.py"
 
 
 # Set up the environment file
 def set_login(USERNAME: str, PASSWORD: str) -> None:
     with open(ENV_PATH, "w") as f:
         f.write(f"# PyPi Account Details\nUSERNAME = \"{USERNAME}\"\nPASSWORD = \"{PASSWORD}\"")
     return
@@ -35,16 +37,16 @@
         print("\tUsage to upload to PyPi: pypi_upload(version = \"[VERSION]\")\n\t\te.g. pypi_upload(version = \"1.0.0\")")
         print("\n\tUsage to create the environment file: set_login(username = \"[USERNAME]\", password = \"[PASSWORD]\")\n\t\te.g. set_login(username = \"username\", password = \"password\")")
         print("\nIf you run this program without any parameters, it will prompt the user for the current version (and the username & password if not already saved).")
         return False
     elif len(argv) == 4 and (argv[1].lower() == "-u" or argv[1].lower() == "--user"):  # If username & password are passed in, create the environment file
         print("Created environment file")
         return set_login(argv[2], argv[3])
-    elif not isfile(SETUP_PATH):  # If setup.py is not found, return False
-        print(f"Setup file not found: {SETUP_PATH}")
+    elif not isfile("setup.py"):  # If setup.py is not found, return False
+        print(f"Setup file not found: setup.py")
         if len(argv) <= 1 and not kwargs:  # If in user input mode, run create_setup()
             create_setup()
         else:   # If not in user input mode, return False
             print("Either run setup_file_creator.py or import create_setup from setup_file_creator and run create_setup() to create the 'setup.py' file\nRun with [-h/--help] or pass in [help=True] to see help")
             return False
     elif not isfile(ENV_PATH):    # If the environment file is not found, or username & password aren't passed in, create the .env & return False
         print(f"Environment file not found: {ENV_PATH}")
@@ -64,39 +66,48 @@
             return False
 
     if kwargs and "version" in kwargs:  # If a version is passed in as a parameter, use that version
         PACKAGE_VERSION = kwargs["version"]
     elif len(argv) == 2 and argv[1]:    # If a version is passed in via command line arguments, use that version
         PACKAGE_VERSION = argv[1]
     elif len(argv) <= 1 and not kwargs: # If no version is passed in & in user input mode, ask for a version
-        PACKAGE_VERSION = input("Please provide a package version")
+        PACKAGE_VERSION = input("Please provide a package version: ")
     else:                               # If no version is passed in (somehow), return False
         print("Please provide a package version")
         return False
     
     # Change version in setup.py
     lines = []
+    package_name = ""
     with open("setup.py", "r") as f:
         lines = f.readlines()
     
     # Find the line with "version = " and replace it with the new version
     for i, line in enumerate(lines):
-        if "version = " in line:
+        if "name" in line:
+            # Just get everything in between the ""'s
+            package_name = re.findall('"([^"]*)"', line)
+        elif "version = " in line:
+            # Replace the version with the new version
             lines[i] = f"\tversion = \"{PACKAGE_VERSION}\",\n"
             break
     
     # Write the new lines to setup.py
     with open("setup.py", "w") as f:
         f.writelines(lines)
 
     # Run setup.py then begin uploading to PyPi
     system("python3 setup.py sdist bdist_wheel")
 
     # Get PyPi Account Variables   
     load_dotenv(ENV_PATH)
     USERNAME = getenv("USERNAME")
     PASSWORD = getenv("PASSWORD")
-    system(f"twine upload dist/* -u \"{USERNAME}\" -p \"{PASSWORD}\"")
+    system(f"twine upload dist/* -u \"{USERNAME}\" -p \"{PASSWORD}\" --verbose")
+    print("\nWaiting a sec before downloading so PyPi can update the package\n")
+    sleep(15)
+    package_name = ''.join(package_name[0]) # Convert list to string (for some reason this wouldn't work where it's defined)
+    system(f"pip install --upgrade {package_name}")
     
 
 if __name__ == "__main__":
     pypi_upload()
```

### Comparing `auto_pypi_uploader-1.0.0/auto_pypi_uploader/setup_file_creator.py` & `auto_pypi_uploader-1.1.0/auto_pypi_uploader/setup_file_creator.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,26 +26,27 @@
             print("\nThis program has four required parameters:")
             print("\t1. [-n/--name] or name: The name of the package")
             print("\t2. [-v/--version] or version: The version of the package")
             print("\t3. [-a/--author] or author: The author of the package")
             print("\t4. [-d/--description] or description: The description of the package")
             print("\nIt can also take some optional parameters:")
             print("\t1. [-h/--help] or help: This help message")
-            print("\t2. [-l/--long_description_content_type] or long_description_content_type: The long description type of the package (default: \"text/markdown\")")
-            print("\t3. [-u/--url] or url: The URL to the website or GitHub repository for the project")
-            print("\t4. [-i/--install_requires] install_requires: The necessary packages to install for the package to work")
+            print("\t2. [-l/--license] or license: The license of the package")
+            print("\t3. [-ld/--long_description_content_type] or long_description_content_type: The long description type of the package (default: \"text/markdown\")")
+            print("\t4. [-u/--url] or url: The URL to the website or GitHub repository for the project")
+            print("\t5. [-i/--install_requires] install_requires: The necessary packages to install for the package to work")
             print("\t\t- Must be in a comma-separated list for Command Line Arguments, or a list for Function Call")
-            print("\t5. [-k/--keywords] or keywords: The keywords for the package")
+            print("\t6. [-k/--keywords] or keywords: The keywords for the package")
             print("\t\t- Must be in a comma-separated list for Command Line Arguments, or a list for Function Call")
-            print("\t6. [-c/--classifiers] or classifiers: The classifiers for the package")
+            print("\t7. [-c/--classifiers] or classifiers: The classifiers for the package")
             print("\t\t- Must be in a comma-separated list for Command Line Arguments, or a list for Function Call")
-            print("\t7. [-p/--python_requires] or python_requires: The minimum Python version required to run the package")
+            print("\t8. [-p/--python_requires] or python_requires: The minimum Python version required to run the package")
             print("\nHere's how to use all the parameters:")
-            print("\tCommand Line Arguments:\n\tpython3 setup_file_creator.py -n NAME -v \"0.0.0\" -a \"AUTHOR\" -d \"DESCRIPTION\" -l \"LONG DESCRIPTION CONTENT TYPE\" -u \"WEBSITE\" -i \"PUT, PACKAGES, HERE\" -k \"KEYWORDS, HERE\" -c \"PUT, CLASSIFIERS, HERE\" -p \"PYTHON VERSION\"")
-            print("\n\tPassing into Function:\n\tsetup_file_creator(name = \"NAME\", version = \"0.0.0\", author = \"AUTHOR\", description = \"DESCRIPTION\", long_description_content_type = \"LONG DESCRIPTION CONTENT TYPE\", url = \"WEBSITE\", install_requires = [\"PUT\", \"PACKAGES\", \"HERE\"], keywords = [\"KEYWORDS\", \"HERE\"], classifiers = [\"PUT\", \"CLASSIFIERS\", \"HERE\"], python_requires = \"PYTHON VERSION\")")
+            print("\tCommand Line Arguments:\n\tpython3 setup_file_creator.py -n NAME -v \"0.0.0\" -a \"AUTHOR\" -d \"DESCRIPTION\" -l \"LICENSE\" -ld \"LONG DESCRIPTION CONTENT TYPE\" -u \"WEBSITE\" -i \"PUT, PACKAGES, HERE\" -k \"KEYWORDS, HERE\" -c \"PUT, CLASSIFIERS, HERE\" -p \"PYTHON VERSION\"")
+            print("\n\tPassing into Function:\n\tsetup_file_creator(name = \"NAME\", version = \"0.0.0\", author = \"AUTHOR\", description = \"DESCRIPTION\", license = \"LICENSE\", long_description_content_type = \"LONG DESCRIPTION CONTENT TYPE\", url = \"WEBSITE\", install_requires = [\"PUT\", \"PACKAGES\", \"HERE\"], keywords = [\"KEYWORDS\", \"HERE\"], classifiers = [\"PUT\", \"CLASSIFIERS\", \"HERE\"], python_requires = \"PYTHON VERSION\")")
             print("\nIf you do not provide any parameters, the program will ask you for them")
             print("The program will automatically create a setup.py file in the current directory if one is not found")
             print("If a setup.py file is found, it will be overwritten")
             return False
         elif len(argv) > 1 or (kwargs and (not "name" in kwargs or not "version" in kwargs or not "author" in kwargs or not "description" in kwargs)):   # If parameters are provided, but not the minimum required parameters, return False
             print("\nPlease provide the minimum required parameters: name, version, author, & description")
             print("\te.g. setup_file_creator(name=\"auto-pypi-exporter\", version=\"1.0.0\", author=\"Huck Dirksmeier\", description=\"A program to automate changing a pip package's version & publishing it\")\n")
@@ -63,14 +64,16 @@
     python_requires = ""
 
     if kwargs:    # If parameters passed in from the function call
         NAME = kwargs["name"]
         VERSION = kwargs["version"]
         AUTHOR = kwargs["author"]
         DESCRIPTION = kwargs["description"]
+        if "license" in kwargs:
+            license = kwargs["license"]
         if "long_description_content_type" in kwargs:
             long_description_content_type = kwargs["long_description_content_type"]
         if "url" in kwargs:
             url = kwargs["url"]
         if "install_requires" in kwargs:
             install_requires = kwargs["install_requires"]
         if "keywords" in kwargs:
@@ -78,40 +81,46 @@
         if "classifiers" in kwargs:
             classifiers = kwargs["classifiers"]
         if "python_requires" in kwargs:
             python_requires = kwargs["python_requires"]
 
     elif len(argv) > 5: # If parameters passed in as command line arguments
         for i, arg in enumerate(argv):
-            if arg == "-n" or arg == "--name":
-                NAME = argv[i + 1]
-            elif arg == "-v" or arg == "--version":
-                VERSION = argv[i + 1]
-            elif arg == "-a" or arg == "--author":
-                AUTHOR = argv[i + 1]
-            elif arg == "-d" or arg == "--description":
-                DESCRIPTION = argv[i + 1]
-            elif arg == "-l" or arg == "--long_description_content_type":
-                long_description_content_type = argv[i + 1]
-            elif arg == "-u" or arg == "--url":
-                url = argv[i + 1]
-            elif arg == "-i" or arg == "--install_requires":
-                install_requires = argv[i + 1].split(",")
-            elif arg == "-k" or arg == "--keywords":
-                keywords = argv[i + 1].split(",")
-            elif arg == "-c" or arg == "--classifiers":
-                classifiers = argv[i + 1].split(",")
-            elif arg == "-p" or arg == "--python_requires":
-                python_requires = argv[i + 1]
+            match arg:
+                case ["-n", "--name"]:
+                    NAME = arg[i + 1]
+                case ["-v", "--version"]:
+                    VERSION = arg[i + 1]
+                case ["-a", "--author"]:
+                    AUTHOR = arg[i + 1]
+                case ["-d", "--description"]:
+                    DESCRIPTION = arg[i + 1]
+                case ["-l", "--license"]:
+                    license = arg[i + 1]
+                case ["-ld", "--long_description_content_type"]:
+                    long_description_content_type = arg[i + 1]
+                case ["-u", "--url"]:
+                    url = arg[i + 1]
+                case ["-i", "--install_requires"]:
+                    install_requires = arg[i + 1].split(",")
+                case ["-k", "--keywords"]:
+                    keywords = arg[i + 1].split(",")
+                case ["-c", "--classifiers"]:
+                    classifiers = arg[i + 1].split(",")
+                case ["-p", "--python_requires"]:
+                    python_requires = arg[i + 1]
 
     else:   # If no parameters passed in (in user input mode)
         NAME = input("Program Name: ")
         VERSION = input("Version: ")
         AUTHOR = input("Author: ")
         DESCRIPTION = input("Description: ")
+        LICENSE_QUESTION = input("\nWould you like to provide a license? (y/n): ")
+        if LICENSE_QUESTION.lower() == "y" or LICENSE_QUESTION.lower() == "yes":
+            license = input("License: ")
         LONG_DESCRIPTION_CONTENT_TYPE_QUESTION = input("\nWould you like to provide a long description content type (default: \"text/markdown\")? (y/n): ")
         if LONG_DESCRIPTION_CONTENT_TYPE_QUESTION.lower() == "y" or LONG_DESCRIPTION_CONTENT_TYPE_QUESTION.lower() == "yes":
             long_description_content_type = input("Long Description Content Type: ")
         URL_QUESTION = input("\nWould you like to provide a URL? (y/n): ")
         if URL_QUESTION.lower() == "y" or URL_QUESTION.lower() == "yes":
             url = input("URL: ")
         INSTALL_REQUIRES_QUESTION = input("\nWould you like to provide packages to install? (y/n): ")
@@ -141,24 +150,26 @@
         "else:\n",
         "\treadme_exists = False\n",
         "\n# Get the long description from the README file if it exists\n",
         "if readme_exists:\n",
         "\twith open(README_PATH) as file:\n",
         "\t\tlong_description = file.read()\n",
         "\nsetup(\n",
-        "\tname = \"" + NAME + "\",\n",
-        "\tversion = \"" + VERSION + "\",\n",
-        "\tauthor = \"" + AUTHOR + "\",\n",
-        "\tdescription = \"" + DESCRIPTION + "\",\n",
+        f"\tname = \"{NAME}\",\n",
+        f"\tversion = \"{VERSION}\",\n",
+        f"\tauthor = \"{AUTHOR}\",\n",
+        f"\tdescription = \"{DESCRIPTION}\",\n",
         "\tlong_description = long_description,\n",
         f"\tlong_description_content_type = \"{long_description_content_type}\",\n"
         "\tpackages = find_packages()",
     ]
+    if license:
+        setup_file.append(f",\n\tlicense = \"{license}\"")
     if url:
-        setup_file.append(",\n\turl = \"" + url + "\"")
+        setup_file.append(f",\n\turl = \"{url}\"")
     if install_requires:
         setup_file.append(",\n\tinstall_requires = " + str(install_requires).lower().replace(" ", ""))
     if keywords:
         # Remove the first character of each keyword if it is a space
         for i, KEYWORD in enumerate(keywords):
             if KEYWORD[0] == " ":
                 keywords[i] = KEYWORD[1:]
@@ -167,14 +178,15 @@
         # Remove the first character of each classifier if it is a space
         for i, CLASSIFIER in enumerate(classifiers):
             if CLASSIFIER[0] == " ":
                 classifiers[i] = CLASSIFIER[1:]
         setup_file.append(",\n\tclassifiers = " + str(classifiers))
     if python_requires:
         setup_file.append(",\n\tpython_requires = \"" + python_requires + "\"")
+    
     setup_file.append("\n)")
 
     # Writing setup.py file
     with open(FILE_PATH, "w") as file:
         for line in setup_file:
             file.write(line)
```

### Comparing `auto_pypi_uploader-1.0.0/auto_pypi_uploader.egg-info/PKG-INFO` & `auto_pypi_uploader-1.1.0/auto_pypi_uploader.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: auto-pypi-uploader
-Version: 1.0.0
-Summary: A program to automate the creation of the 'setup.py' file, changing a pip package's version & publishing it to PyPi.
+Version: 1.1.0
+Summary: A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi.
 Home-page: https://github.com/Huckdirks/auto-pypi-exporter
 Author: Huck Dirksmeier
 Author-email: Huckdirks@gmail.com
+License: MIT
 Keywords: PyPi,Pip,setup,setup.py,automation
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,153 +19,164 @@
 ## Table of Contents
 
 - [Introduction](#introduction)
 - [Uses](#uses)
     - [Running from Command Line](#running-from-command-line)
     - [Running with Command Line Arguments](#running-with-command-line-arguments)
     - [Importing as a Module](#importing-as-a-module)
+        - [Installing with pip](#installing-with-pip)
         - [`create_setup()`](#create_setup-takes-in)
         - [`set_login()`](#set_login-takes-in)
         - [`pypi_upload()`](#pypi_upload-takes-in)
 - [Running](#running)
     - [Dependencies](#dependencies)
     - [Setting Up .env File](#setting-up-env-file)
     - [Running](#running-1)
 - [Quality Assurance](#quality-assurance)
 - [Suggestions](#suggestions)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Introduction
 
-While working on my previous project: [text-excuse-generator](https://github.com/Huckdirks/text-excuse-generator), I just published my first package to [PyPi](https://pypi.org/project/text-excuse-generator/). I quickly realized that I wasn't going to be able to remember the command line arguments to pass into the required fields, and that I was bound to forget to change the version manually in the `setup.py` file every time I updated the package. So I decided to make a program that would automatically update the version number in the `setup.py` file and export my project to [PyPi](https://pypi.org/). I also added another script that would automatically create a `setup.py` file for me with the required fields.
+While working on my previous project: [text-excuse-generator](https://github.com/Huckdirks/text-excuse-generator), I just published my first package to [PyPi](https://pypi.org/project/text-excuse-generator/). I quickly realized that I wasn't going to be able to remember the command line arguments to pass into the required fields, and that I was bound to forget to change the version manually in the `setup.py` file every time I updated the package. So I decided to make a program that would automatically update the version number in the `setup.py` file and export a project to [PyPi](https://pypi.org/). I also added another script that would automatically create a `setup.py` file for me with the required fields.
 
 ## Uses
 
 There are three main ways to interact with the program: by [running it in the command line](#running-from-command-line), by [running it with command line arguments](#running-with-command-line-arguments), or by [importing it](#importing-as-a-module) into another python file.
 
 In order for this program to run, your project's directory must be set up as such:
 Any files and directories in **[ ]**'s are optional, **but highly recommended!!!**
-```bash
+```
 project_root_dir/
-    [LICENSE]
+    pypi_uploader.py (can be downloaded from auto_pypi_uploader/ or substituted with a program that imports the module)
+    setup.py (can be created with pypi_uploader.py or setup_file_creator.py)
     [README.md] (can also be in docs/)
+    [LICENSE]
+
     main_module_name/
             __init__.py
             (other python files...)
+
     [docs/]
-    setup.py (can be created with pypi_uploader.py or setup_file_creator.py)
-    pypi_uploader.py (can be downloaded from include/ or substituted with a program that imports the module)
+            [README.md]
 ```
 
 
 You can also have multiple modules in the same directory, or even multiple modules within a module, but you will need to add the `__init__.py` file to each directory that contains a module. e.g.
-```bash
+```
 project_root_dir/
-    [LICENSE]
+    pypi_uploader.py (can be downloaded from auto_pypi_uploader/ or substituted with a program that imports the module)
+    setup.py (can be created with pypi_uploader.py or setup_file_creator.py)
     [README.md] (can also be in docs/)
+    [LICENSE]
+
     main_module_name/
             __init__.py
             (other python files...)
             main_submodule_name/
                     __init__.py
                     (other python files...)
+
     secondary_module_name/
             __init__.py
             (other python files...)
+
     [docs/]
-    setup.py (can be created with pypi_uploader.py or setup_file_creator.py)
-    pypi_uploader.py (can be downloaded from include/ or substituted with a program that imports the module)
+            [README.md]
 ```
 
 ### Running from Command Line
 
-I'd recommend downloading [pypi_uploader.py](../include/pypi_uploader.py) from [include](../include/pypi_uploader.py) into a project's [root directory](../) if you want the functionality of the whole module. Or just [setup_file_creator](../include/setup_file_creator.py) if you only want to make a `setup.py` file. You can run the program by typing:
+I'd recommend downloading [pypi_uploader.py](../include/pypi_uploader.py) from [include](../include/pypi_uploader.py) into a project's [root directory](../) if you want the functionality of the whole module, or just [`setup_file_creator.py`](../auto_pypi_uploader/setup_file_creator.py) if you only want to make a `setup.py` file. You can run the program by typing:
 ```bash
 python3 pypi_uploader.py
 ```
 
-When you run the program normally, it will first check if a `setup.py` file exists in the current directory. If it doesn't, it will then run [`setup_file_creator`](../include/setup_file_creator.py)`.create_setup()`, which will ask you for:
+When you run the program normally, it will first check if a `setup.py` file exists in the current directory. If it doesn't, it will then run [`setup_file_creator`](../auto_pypi_uploader/setup_file_creator.py)`.create_setup()`, which will ask you for:
 - The Project's Name
 - The Project's Version
 - The Project's Author
 - The Project's Description
 
 And ask you if you want to add these optional fields:
+- The Project's License
 - The Project's Long Description Type (From [README.md](README.md))
 - The Project's URL
 - The Required Packages
 - Keywords
 - Classifiers
 - Minimum Python Version
 
 *If you just want to create a `setup.py` file, run:*
 ```bash
 python3 setup_file_creator.py
 ```
 
 
-If a `setup.py` file already exists, `pypi_uploader.py` will then ask you for a new version number, and update it in `setup.py`. It will then upload the package to [PyPi](https://pypi.org/). If you haven't already set up your login credentials, it will then ask you for your username and password & save it, and then proceed to upload the package.
+If a `setup.py` file already exists, [`pypi_uploader.py`](../auto_pypi_uploader/pypi_uploader.py) will then ask you for a new version number, and update it in `setup.py`. It will then upload the package to [PyPi](https://pypi.org/). If you haven't already set up your login credentials, it will then ask you for your username and password & save it, and then proceed to upload the package. It then automatically updates/ installs the package with `pip3 install --upgrade {project_name}`.
 
 The program runs: `python3 setup.py sdist bdist_wheel` and `python3 twine upload dist/* -u "{USERNAME}" -p "{PASSWORD}"` to upload the package to [PyPi](https://pypi.org/).
 
 ### Running with Command Line Arguments
 
-You can also run the program with command line arguments. If you want to send the text message, you can add `--send` or `-s` as the last argument. All command line arguments longer than a single word need to be in parentheses. I'd recommend downloading [pypi_uploader.py](../include/pypi_uploader.py) from [include](../include/pypi_uploader.py) into a project's [root directory](../) if you want all the functionality, or just [setup_file_creator](../include/setup_file_creator.py) if you only want to make a `setup.py` file, and running them from the command line. Please also include the [LICENSE](../LICENSE) file in the same directory as any files you add from [this project](https://github.com/Huckdirks/auto-pypi-uploader).
+You can also run the program with command line arguments. If you want to send the text message, you can add `--send` or `-s` as the last argument. All command line arguments longer than a single word need to be in parentheses. I'd recommend downloading [`pypi_uploader.py`](../auto_pypi_uploader/pypi_uploader.py) into a project's [root directory](../) if you want all the functionality, or just [`setup_file_creator.py`](../auto_pypi_uploader/setup_file_creator.py) if you only want to make a `setup.py` file, and running them from the command line. Please also include the [LICENSE](../LICENSE) file in the same directory as any files you add from [this project](https://github.com/Huckdirks/auto-pypi-uploader).
 
 #### **Creating a `setup.py` File**
 
 If you want to create a `setup.py` file, run:
 ```bash
-python3 setup_file_creator.py --name PROJECT_NAME --version VERSION --author AUTHOR --description DESCRIPTION [--long_description_content_type LONG_DESCRIPTION_TYPE] [--url URL] [--install_requires "INSTALL_REQUIRES"] [--keywords "KEYWORDS"] [--classifiers "CLASSIFIERS"] [--python_requires PYTHON_REQUIRES]
+python3 setup_file_creator.py --name PROJECT_NAME --version VERSION --author AUTHOR --description DESCRIPTION [--license LICENSE] [--long_description_content_type LONG_DESCRIPTION_TYPE] [--url URL] [--install_requires "INSTALL_REQUIRES"] [--keywords "KEYWORDS"] [--classifiers "CLASSIFIERS"] [--python_requires PYTHON_REQUIRES]
 ```
 Any parameters in [ ]'s are optional, and all parameters in " "'s can be a comma separated list: e.g.
 ```bash
-python3 setup_file_creator.py -n auto_pypi_uploader -v "1.0.0" -a "Huck Dirksmeier" -d "A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi." -l text/markdown -u https://github.com/Huckdirks/auto-pypi-uploader -i "twine, python-dotenv" -k "PyPi, Pip, setup, setup.py, automation" -c "Programming Language :: Python, License :: MIT License, Operating System :: OS Independent" -p ">=3.8"
+python3 setup_file_creator.py -n auto_pypi_uploader -v "1.0.0" -a "Huck Dirksmeier" -d "A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi." -l MIT -ld text/markdown -u https://github.com/Huckdirks/auto-pypi-uploader -i "twine, python-dotenv" -k "PyPi, Pip, setup, setup.py, automation" -c "Programming Language :: Python, License :: OSI Approved :: MIT License, Operating System :: OS Independent" -p ">=3.8"
 ```
 
 #### **Uploading [PyPi](https://pypi.org/) Package & Adding Login Information**
 If you want to upload a package to [PyPi](https://pypi.org/), run:
 ```bash
-python3 pypi_uploader.py [VERSION] [--user USERNAME PASSWORD]
+python3 pypi_uploader.py VERSION [--user USERNAME PASSWORD]
 ```
 e.g.
 ```bash
 python3 pypi_uploader.py "1.0.0" -u Huckdirks PASSWORD
 ```
-This assumes that you've already made a `setup.py` file. If you just want to update the version number, run `python3 pypi_uploader.py [VERSION]`. This assumes that you've already set up your login credentials. To just add login credentials, run `python3 pypi_uploader.py --user USERNAME PASSWORD`. This will add your username and password to a `.env` file in the current directory. If you decide to update the version & login information in a single call, **make sure the version is the first argument!** **YOU ONLY NEED TO ADD YOUR LOGIN INFORMATION ONCE, OTHERWISE IT WILL OVERRIDE THE PREVIOUS LOGIN INFORMATION!!!**
+This assumes that you've already made a `setup.py` file. If you just want to update the version number, run `python3 pypi_uploader.py VERSION`. This assumes that you've already set up your login credentials. To just add login credentials, run `python3 pypi_uploader.py --user USERNAME PASSWORD`. This will add your username and password to a `.env` file in the current directory. If you decide to update the version & login information in a single call, **make sure the version is the first argument!** **YOU ONLY NEED TO ADD YOUR LOGIN INFORMATION ONCE, OTHERWISE IT WILL OVERRIDE THE PREVIOUS LOGIN INFORMATION!!!**
 
 ### Importing as a Module
 
-You can also import the program as a module into another python file. The `auto_pypi_uploader` module has  two sub-modules:
-- `setup_file_creator` has one function: `create_setup()`
-- `pypi_uploader` has two functions: `pypi_upload()` and `set_login()`
+You can also import the program as a module into another python file.
 
 #### Installing with pip
 
 Simply run:
 ```bash
 pip install auto-pypi-uploader
 ```
+ The `auto_pypi_uploader` module has  two sub-modules:
+- `setup_file_creator` has one function: [`create_setup()`](#create_setup-takes-in)
+- `pypi_uploader` has two functions: [`pypi_upload()`](#pypi_upload-takes-in) and [`set_login()`](#set_login-takes-in)
+
 To import the modules into your python file, put this at the top of your file:
 ```python
 from auto_pypi_uploader.pypi_uploader import *
 from auto_pypi_uploader.setup_file_creator import *
 ```
 Or you can import the individual functions.
 
 #### `create_setup()` takes in:
 ```python
-create_setup(NAME: str, VERSION: str, AUTHOR: str, DESCRIPTION: str, help: bool, long_description_content_type: str, url: str, install_requires: list[str], keywords: list[str], classifiers: list[str], python_requires: str) -> bool
+create_setup(NAME: str, VERSION: str, AUTHOR: str, DESCRIPTION: str, help: bool, license: str, long_description_content_type: str, url: str, install_requires: list[str], keywords: list[str], classifiers: list[str], python_requires: str) -> bool
 ```
 `create_setup()` returns True if able to generate `setup.py` and False if not. **All uppercase parameters are required if parameters are passed in, and each parameter must be defined in the function call. You can also omit all parameters, and the function will prompt you for each one manually.**
 
 If you want to create a `setup.py` file, call the function like this:
 ```python
-create_setup(name = "auto_pypi_uploader", version = "1.0.0", author = "Huck Dirksmeier", description = "A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi.", long_description_content_type = "text/markdown", url = "https://github.com/Huckdirks/auto-pypi-uploader", install_requires = ["twine", "python-dotenv"], keywords = ["PyPi", "Pip", "setup", "setup.py", "automation"], classifiers = ["Programming Language :: Python", "License :: MIT License", "Operating System :: OS Independent"], python_requires = ">=3.8")
+create_setup(name = "auto_pypi_uploader", version = "1.0.0", author = "Huck Dirksmeier", description = "A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi.", license = "MIT", long_description_content_type = "text/markdown", url = "https://github.com/Huckdirks/auto-pypi-uploader", install_requires = ["twine", "python-dotenv"], keywords = ["PyPi", "Pip", "setup", "setup.py", "automation"], classifiers = ["Programming Language :: Python", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"], python_requires = ">=3.8")
 ```
 Make sure to put the fields before the variables when calling the function.
 
 #### `set_login()` takes in:
 ```python
 set_login(USERNAME: str, PASSWORD: str) -> None
 ```
@@ -172,15 +184,15 @@
 ```python
 set_login("USERNAME", "PASSWORD")
 ```
 If you want user input, just call [`pypi_upload()`](#pypi_upload-takes-in).
 
 #### `pypi_upload()` takes in:
 ```python
-pypi_upload(VERSION: str, USERNAME: str, PASSWORD: str) -> bool
+pypi_upload(VERSION: str, username: str, password: str) -> bool
 ```
 `pypi_upload()` returns True if the package was successfully uploaded, and False if it wasn't. **All uppercase parameters are required if parameters are passed in, and each parameter must be defined in the function call. You can also omit all parameters, and the function will prompt you for the version, and the login info if not previously saved.**
 If you want to upload a package & login to [PyPi](https://pypi.org/), call `pypi_upload()` like this:
 ```python
 pypi_upload(version = "0.0.0", username = "USERNAME", password = "PASSWORD")
 ```
 
@@ -205,15 +217,15 @@
 Either run the program without any arguments to manually input the information for the .env file, run with [command line arguments](#setting-up-env-file) to automatically input the information for the .env file, or pass in the correct parameters to the [`set_login()`](#set_login-takes-in) or [`pypi_upload()`](#pypi_upload-takes-in) function.
 
 ### Running
 
 **YOU HAVE TO INSTALL THE DEPENDENCIES & SETUP THE `.env` FILE BEFORE TRYING TO RUN THE PROGRAM!!!**
 If installed with pip, all dependencies should be installed automatically!
 
-Run `python3 text_excuse_generator.py` or `python3 text_excuse_generator.py [sender] [recipient] [problem] [excuse] [--send_text_flag]` in the command line in the source directory.
+Run [`python3 pypi_uploader.py`](#running-from-command-line) or [`python3 pypi_uploader.py VERSION [--user USERNAME PASSWORD]`](#running-with-command-line-arguments) in the command line in the source directory.
 
 More detailed instructions are in the [Uses](#uses) section.
 
 ## Quality Assurance
 All variable, function, class, module, & file names are written in [snake_case](https://en.wikipedia.org/wiki/Snake_case) to make sure everything is consistent, and all `const` variables are written in ALL-CAPS. The code is also quite commented and the variable names are quite verbose, so it should be easy enough to understand what's going on.
 
 If there are any other/better ways to check for quality assurance, please let me know in the [suggestions](https://github.com/Huckdirks/auto-pip-exporter/discussions/new?category=suggestions)!
```

### Comparing `auto_pypi_uploader-1.0.0/setup.py` & `auto_pypi_uploader-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 # Set the long description if the README file exists
 if readme_exists:
     with open(README_PATH, "r") as file:
         long_description = file.read()
 
 setup(
     name = "auto_pypi_uploader",
-	version = "1.0.0",
+	version = "1.1.0",
     author = "Huck Dirksmeier",
     author_email = "Huckdirks@gmail.com",
-    description = "A program to automate the creation of the 'setup.py' file, changing a pip package's version & publishing it to PyPi.",
+    description = "A program to automate the creation of the 'setup.py' file, changing a pip package's version, & publishing it to PyPi.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
+    license = "MIT",
     url = "https://github.com/Huckdirks/auto-pypi-exporter",
     packages = find_packages(),
-    install_requires = ["python-dotenv", "twine"],
+    install_requires = ["python-dotenv", "twine", "wheel", "setuptools"],
     keywords = ["PyPi", "Pip", "setup", "setup.py", "automation"],
     classifiers = [
         "Programming Language :: Python",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires = ">=3.0"
```

