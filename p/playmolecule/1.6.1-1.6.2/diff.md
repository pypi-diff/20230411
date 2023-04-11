# Comparing `tmp/playmolecule-1.6.1.tar.gz` & `tmp/playmolecule-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.6.1.tar", last modified: Wed Apr  5 13:31:53 2023, max compression
+gzip compressed data, was "playmolecule-1.6.2.tar", last modified: Tue Apr 11 13:35:44 2023, max compression
```

## Comparing `playmolecule-1.6.1.tar` & `playmolecule-1.6.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:31:53.825024 playmolecule-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-05 13:31:41.000000 playmolecule-1.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-05 13:31:41.000000 playmolecule-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-05 13:31:53.825024 playmolecule-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-05 13:31:41.000000 playmolecule-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:31:53.821024 playmolecule-1.6.1/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-05 13:31:41.000000 playmolecule-1.6.1/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-05 13:31:41.000000 playmolecule-1.6.1/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-05 13:31:41.000000 playmolecule-1.6.1/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-05 13:31:41.000000 playmolecule-1.6.1/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    38068 2023-04-05 13:31:41.000000 playmolecule-1.6.1/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-04-05 13:31:41.000000 playmolecule-1.6.1/playmolecule/func2argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    32135 2023-04-05 13:31:41.000000 playmolecule-1.6.1/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-05 13:31:41.000000 playmolecule-1.6.1/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-05 13:31:41.000000 playmolecule-1.6.1/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-05 13:31:41.000000 playmolecule-1.6.1/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-05 13:31:41.000000 playmolecule-1.6.1/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33199 2023-04-05 13:31:41.000000 playmolecule-1.6.1/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-05 13:31:41.000000 playmolecule-1.6.1/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:31:53.821024 playmolecule-1.6.1/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-05 13:31:53.000000 playmolecule-1.6.1/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-05 13:31:53.000000 playmolecule-1.6.1/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 13:31:53.000000 playmolecule-1.6.1/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-05 13:31:53.000000 playmolecule-1.6.1/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-05 13:31:53.000000 playmolecule-1.6.1/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-05 13:31:41.000000 playmolecule-1.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 13:31:53.825024 playmolecule-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-05 13:31:41.000000 playmolecule-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:35:44.855669 playmolecule-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-11 13:35:22.000000 playmolecule-1.6.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 13:35:22.000000 playmolecule-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-11 13:35:44.855669 playmolecule-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-11 13:35:22.000000 playmolecule-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:35:44.851669 playmolecule-1.6.2/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32923 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/func2argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33199 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-11 13:35:22.000000 playmolecule-1.6.2/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:35:44.855669 playmolecule-1.6.2/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-11 13:35:44.000000 playmolecule-1.6.2/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-11 13:35:44.000000 playmolecule-1.6.2/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:35:44.000000 playmolecule-1.6.2/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-11 13:35:44.000000 playmolecule-1.6.2/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-11 13:35:44.000000 playmolecule-1.6.2/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 13:35:22.000000 playmolecule-1.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:35:44.855669 playmolecule-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-11 13:35:22.000000 playmolecule-1.6.2/setup.py
```

### Comparing `playmolecule-1.6.1/LICENSE.md` & `playmolecule-1.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.1/PKG-INFO` & `playmolecule-1.6.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.6.1
+Version: 1.6.2
 Summary: The playmolecule python code.
 Home-page: https://github.com/acellera/playmolecule-python-api/
 Author: Acellera
 Author-email: info@acellera.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
```

### Comparing `playmolecule-1.6.1/playmolecule/__init__.py` & `playmolecule-1.6.2/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.1/playmolecule/config.py` & `playmolecule-1.6.2/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.1/playmolecule/datacenter.py` & `playmolecule-1.6.2/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.1/playmolecule/devutils.py` & `playmolecule-1.6.2/playmolecule/devutils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1043,182 +1043,7 @@
             traceback.print_exc(file=f)
 
         try:
             job._set_error()
         except Exception:
             pass
 
-
-def _test_func(
-    outdir: Path,
-    pdb: Path,
-    simtime: float = 0.5,
-    equiltimes: list[float] = None,
-    randomize: list[bool] = [True],
-    no_prep: bool = False,
-    forcefield: str = "CHARMM",
-    **kwargs,
-):
-    """TestFunc
-
-    Test function
-
-    Parameters
-    ----------
-    outdir : Path
-        Output directory
-    pdb : Path
-        Input file
-    simtime : float
-        Simulation time
-    equiltimes : list[float]
-        List of equilibration times
-    randomize : list[bool]
-        List of booleans
-    no_prep : bool
-        No preparation
-    forcefield : str, choices=("CHARMM", "AMBER")
-        The simulation forcefield
-    """
-    print("Running test function with args:", locals())
-
-
-class _TestWrapper(unittest.TestCase):
-    def test_app_wrapper(self):
-        args = [
-            "--outdir",
-            "/tmp/",
-            "--pdb",
-            "/tmp/test.pdb",
-            "--simtime",
-            "0.3",
-            "--equiltimes",
-            "0.1 0.2",
-            "--randomize",
-            "false True",
-            "--no-prep",
-            "--forcefield",
-            "AMBER",
-        ]
-        app_wrapper2("playmolecule.devutils._test_func", " ".join(args))
-
-    # def test_app_wrapper_pmws(self):
-    #     import os
-
-    #     args = [
-    #         "--outdir",
-    #         "/tmp/",
-    #         "--pdb",
-    #         "/tmp/test.pdb",
-    #         "--simtime",
-    #         "0.3",
-    #         "--equiltimes",
-    #         "0.1 0.2",
-    #         "--randomize",
-    #         "false True",
-    #         "--no-prep",
-    #         "--forcefield",
-    #         "AMBER",
-    #     ]
-    #     app_wrapper2(
-    #         "playmolecule.devutils._test_func",
-    #         token=os.environ["PM_TOKEN"],
-    #         execid="xx",
-    #     )
-
-    def test_app_argparse_dump(self):
-        import tempfile
-        import json
-
-        dump_ref = {
-            "description": "Test function",
-            "params": [
-                {
-                    "mandatory": True,
-                    "type": "Path",
-                    "name": "outdir",
-                    "value": None,
-                    "tag": "--outdir",
-                    "description": "Output directory",
-                    "nargs": None,
-                    "choices": None,
-                    "metavar": None,
-                },
-                {
-                    "mandatory": True,
-                    "type": "Path",
-                    "name": "pdb",
-                    "value": None,
-                    "tag": "--pdb",
-                    "description": "Input file",
-                    "nargs": None,
-                    "choices": None,
-                    "metavar": None,
-                },
-                {
-                    "mandatory": False,
-                    "type": "float",
-                    "name": "simtime",
-                    "value": 0.5,
-                    "tag": "--simtime",
-                    "description": "Simulation time",
-                    "nargs": None,
-                    "choices": None,
-                    "metavar": None,
-                },
-                {
-                    "mandatory": False,
-                    "type": "float",
-                    "name": "equiltimes",
-                    "value": None,
-                    "tag": "--equiltimes",
-                    "description": "List of equilibration times",
-                    "nargs": "+",
-                    "choices": None,
-                    "metavar": None,
-                },
-                {
-                    "mandatory": False,
-                    "type": "str_to_bool",
-                    "name": "randomize",
-                    "value": [True],
-                    "tag": "--randomize",
-                    "description": "List of booleans",
-                    "nargs": "+",
-                    "choices": None,
-                    "metavar": None,
-                },
-                {
-                    "mandatory": False,
-                    "type": "bool",
-                    "name": "no_prep",
-                    "value": False,
-                    "tag": "--no-prep",
-                    "description": "No preparation",
-                    "nargs": None,
-                    "choices": None,
-                    "metavar": None,
-                },
-                {
-                    "mandatory": False,
-                    "type": "str",
-                    "name": "forcefield",
-                    "value": "CHARMM",
-                    "tag": "--forcefield",
-                    "description": "The simulation forcefield",
-                    "nargs": None,
-                    "choices": ["CHARMM", "AMBER"],
-                    "metavar": None,
-                },
-            ],
-        }
-        with tempfile.TemporaryDirectory() as tmpdir:
-            argpf = os.path.join(tmpdir, "argp.json")
-            app_wrapper2("playmolecule.devutils._test_func", dump_argparser=argpf)
-
-            with open(argpf, "r") as f:
-                argp = json.load(f)
-                assert argp == dump_ref
-
-
-if __name__ == "__main__":
-    unittest.main(verbosity=2)
```

### Comparing `playmolecule-1.6.1/playmolecule/func2argparse.py` & `playmolecule-1.6.2/playmolecule/func2argparse.py`

 * *Files 26% similar despite different names*

```diff
@@ -215,111 +215,7 @@
     if isinstance(value, bool):
         return value
     if value.lower() == "false":
         return False
     if value.lower() == "true":
         return True
     raise RuntimeError(f"Invalid boolean value {value}")
-
-
-def _test_func(
-    x: int,
-    y: Path,
-    z: int = 54,
-    w: list[str] = ("hey", "ho"),
-    k: str = "choice1",
-    ll: list[int] = None,
-    flg: bool = False,
-    lb: list[bool] = True,
-):
-    """This is a test function
-
-    Parameters
-    ----------
-    x : int
-        First arg
-    y : Path
-        Second arg
-    z : int
-        Third arg
-    w : list[str]
-        Fourth arg.
-        Multiline documentation
-    k : str, choices=("choice1", "choice2")
-        Fifth arg
-    ll : list[int]
-        This is an empty list
-    flg : bool
-        Set to True to do something
-    lb : list[bool]
-        A list of boolean values
-    Examples
-    --------
-    >>> test_func()
-    """
-    print(x, y, z, w, k, ll, flg, lb)
-
-
-class _TestFunc2Argparse(unittest.TestCase):
-    def _dict2list(self, dd):
-        ll = []
-        for key, val in dd.items():
-            ll.append(f"--{key}")
-            if type(val) not in (list, tuple):
-                if isinstance(val, bool) and val:
-                    continue
-                ll.append(str(val))
-            else:
-                for vv in val:
-                    ll.append(str(vv))
-        return ll
-
-    def _compare_results(self, test_args, args):
-        args = vars(args)
-        for key in test_args:
-            if key == "y":
-                assert args[key] == Path(test_args[key])
-            else:
-                assert args[key] == test_args[key], f"{args[key]}, {test_args[key]}"
-
-    def test_func2argparse(self):
-        parser = func_to_argparser(_test_func, exit_on_error=False)
-
-        test_args = {
-            "x": 5,
-            "y": "./func2argparse.py",
-            "z": 42,
-            "w": ["stefan", "doerr"],
-            "k": "choice2",
-            "ll": [84, 32],
-            "flg": True,
-            "lb": [False, True],
-        }
-
-        args = parser.parse_args(self._dict2list(test_args))
-        self._compare_results(test_args, args)
-
-        test_args = {
-            "x": 5,
-            "y": "./func2argparse.py",
-        }
-        args = parser.parse_args(self._dict2list(test_args))
-        self._compare_results(test_args, args)
-
-        test_args = {
-            "x": "ho",  # Wrong, should be integer
-            "y": "./func2argparse.py",
-        }
-        self.assertRaises(
-            argparse.ArgumentError, parser.parse_args, self._dict2list(test_args)
-        )
-        test_args = {
-            "x": "7.5",  # Wrong, should be integer
-            "y": "./func2argparse.py",
-        }
-        self.assertRaises(
-            argparse.ArgumentError, parser.parse_args, self._dict2list(test_args)
-        )
-
-
-if __name__ == "__main__":
-    unittest.main(verbosity=2)
```

### Comparing `playmolecule-1.6.1/playmolecule/job.py` & `playmolecule-1.6.2/playmolecule/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,28 +209,29 @@
             except Exception as e:
                 msg = f"Could not set Job attribute {key} with error {e}. The Job was possibly spawned with an older app version."
                 if strict:
                     raise JobConfigNotLoadedError(msg)
                 else:
                     logger.warning(msg)
 
-    # TODO: accept more synonyms
     def _get_validator(self, type):
         if type == "bool":
             return val.Boolean()
         elif type == "int":
             return val.Number(int, "ANY")
         elif type == "string" or type == "str":
             return val.String()
         elif type == "file" or type == "Path":
             return StringOrDataset()
         elif type == "float":
             return val.Number(float, "ANY")
         elif type == "fileORstring":
             return val.String()
+        elif type == "str_to_bool":
+            return val.Boolean()
 
     @property
     def _token(self):
         return self._session._token
 
     @property
     def _server_endpoint(self):
```

### Comparing `playmolecule-1.6.1/playmolecule/jsonlogger.py` & `playmolecule-1.6.2/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.1/playmolecule/local.py` & `playmolecule-1.6.2/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.1/playmolecule/playqueue.py` & `playmolecule-1.6.2/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.1/playmolecule/session.py` & `playmolecule-1.6.2/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.1/playmolecule/utils.py` & `playmolecule-1.6.2/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.6.1/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.6.2/playmolecule.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.6.1
+Version: 1.6.2
 Summary: The playmolecule python code.
 Home-page: https://github.com/acellera/playmolecule-python-api/
 Author: Acellera
 Author-email: info@acellera.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
```

### Comparing `playmolecule-1.6.1/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.6.2/playmolecule.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.md
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 playmolecule/__init__.py
+playmolecule/_test_funcs.py
 playmolecule/config.ini
 playmolecule/config.py
 playmolecule/datacenter.py
 playmolecule/devutils.py
 playmolecule/func2argparse.py
 playmolecule/job.py
 playmolecule/jsonlogger.py
```

### Comparing `playmolecule-1.6.1/setup.py` & `playmolecule-1.6.2/setup.py`

 * *Files identical despite different names*

