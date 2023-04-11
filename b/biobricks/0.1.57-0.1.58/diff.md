# Comparing `tmp/biobricks-0.1.57.tar.gz` & `tmp/biobricks-0.1.58.tar.gz`

## Comparing `biobricks-0.1.57.tar` & `biobricks-0.1.58.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks.svg
--rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 biobricks-0.1.57/coverage.xml
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 biobricks-0.1.57/requirements.txt
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 biobricks-0.1.57/.github/workflows/biobricks.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.57/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.57/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.57/.pytest_cache/README.md
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.57/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 biobricks-0.1.57/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.57/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 biobricks-0.1.57/.vscode/tasks.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/__init__.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/api.py
--rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/brick.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/checks.py
--rwxr-xr-x   0        0        0     4049 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/cli.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/config.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/local_bb.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/.pytest_cache/README.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/tests/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/tests/test_init.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.57/biobricks/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 biobricks-0.1.57/docker/Dockerfile
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.57/docker/test.sh
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 biobricks-0.1.57/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.1.57/LICENSE
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 biobricks-0.1.57/README.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 biobricks-0.1.57/pyproject.toml
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 biobricks-0.1.57/PKG-INFO
+-rw-r--r--   0        0        0    13118 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks.svg
+-rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 biobricks-0.1.58/coverage.xml
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 biobricks-0.1.58/requirements.txt
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 biobricks-0.1.58/.github/workflows/biobricks.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.58/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.58/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.58/.pytest_cache/README.md
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.58/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 biobricks-0.1.58/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.58/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 biobricks-0.1.58/.vscode/tasks.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/__init__.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/api.py
+-rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/brick.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/checks.py
+-rwxr-xr-x   0        0        0     4049 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/cli.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/config.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/local_bb.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/.pytest_cache/README.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/test_init.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 biobricks-0.1.58/biobricks/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 biobricks-0.1.58/docker/Dockerfile
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 biobricks-0.1.58/docker/test.sh
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 biobricks-0.1.58/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 biobricks-0.1.58/LICENSE
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 biobricks-0.1.58/README.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 biobricks-0.1.58/pyproject.toml
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 biobricks-0.1.58/PKG-INFO
```

### Comparing `biobricks-0.1.57/biobricks.svg` & `biobricks-0.1.58/biobricks.svg`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.57/coverage.xml` & `biobricks-0.1.58/coverage.xml`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.57/.github/workflows/biobricks.yml` & `biobricks-0.1.58/.github/workflows/biobricks.yml`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.57/biobricks/api.py` & `biobricks-0.1.58/biobricks/api.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.57/biobricks/brick.py` & `biobricks-0.1.58/biobricks/brick.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,14 +144,16 @@
 
         logger.info(f"discovering brick assets dvc.biobricks.ai")
         fs = dvc.api.DVCFileSystem(self.path())
         paths = fs.find("data",maxdepth=1) + fs.find("brick",maxdepth=1)
         parquet_paths = [x for x in paths if x.endswith('.parquet')]
 
         logger.info(f"pulling brick assets")
+        # TODO dvc currently queries the cache which involves big md5 calculations
+        # instead we should use the dvc api to pull the files directly
         run(f"dvc pull {' '.join(parquet_paths)}", cwd=self.path(), shell=True)
         
         logger.info(f"\033[94m{self.url()}\033[0m succesfully downloaded to BioBricks library.")
         return self
     
     def load(self):
         "load this brick"
```

### Comparing `biobricks-0.1.57/biobricks/checks.py` & `biobricks-0.1.58/biobricks/checks.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.57/biobricks/cli.py` & `biobricks-0.1.58/biobricks/cli.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.57/biobricks/config.py` & `biobricks-0.1.58/biobricks/config.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.57/biobricks/local_bb.py` & `biobricks-0.1.58/biobricks/local_bb.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,9 +30,9 @@
       print(f"'{brickref.name}' already exists, to update:")
       print(f"\trun `biobricks remove {brickref.name}`")
       print(f"\tand `biobricks add {brickref.name}`")
       return
     
     # add dependency to the dependencies file
     with open(self.dependencies_path, "a") as f:
-      f.write(f"{brickref.url}\n")
+      f.write(f"{brickref.url()}\n")
```

### Comparing `biobricks-0.1.57/biobricks/tests/test_init.py` & `biobricks-0.1.58/biobricks/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.57/docker/Dockerfile` & `biobricks-0.1.58/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.57/LICENSE` & `biobricks-0.1.58/LICENSE`

 * *Files identical despite different names*

### Comparing `biobricks-0.1.57/README.md` & `biobricks-0.1.58/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 > Input a token from biobrick.ai/token: <this is your access token>
 ```
 
 # Pull Bricks
 To download a brick and save it locally in your library use `bb.pull`. An example using the Tox21 dataset:  
 
 ```python
+import biobricks as bb
 bb.install('tox21') # save the brick to the brick library and download it's resources
 tox21 = bb.load('tox21') # load a SimpleNamespace with all the brick tables
 
 # List the resources in the brick
 for tablename in sorted(list(vars(tox21).keys())):
     print(tablename)
     
-tox21.tox21_ache_p4.to_pandas() # get a pyarrow Table and convert to pandas dataframe
+tox21.tox21_ache_p4.read().to_pandas() # get a pyarrow Table and convert to pandas dataframe
 ```
 
 To list the bricks currently available visit [github.com/biobricks-ai](https://github.com/biobricks-ai)
```

### Comparing `biobricks-0.1.57/pyproject.toml` & `biobricks-0.1.58/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "biobricks"
-version = "0.1.57"
+version = "0.1.58"
 authors = [
   { name="Jose A. Jaramillo", email="jjv@utp.edu.co" },
   { name="Thomas Luechtefeld", email="tom@insilica.co" }
 ]
 description = "Biobricks automates bioinformatics data."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `biobricks-0.1.57/PKG-INFO` & `biobricks-0.1.58/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobricks
-Version: 0.1.57
+Version: 0.1.58
 Summary: Biobricks automates bioinformatics data.
 Project-URL: Homepage, https://github.com/biobricks-ai/biobricks
 Project-URL: Bug Tracker, https://github.com/biobricks-ai/biobricks/issues
 Author-email: "Jose A. Jaramillo" <jjv@utp.edu.co>, Thomas Luechtefeld <tom@insilica.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,18 +38,19 @@
 > Input a token from biobrick.ai/token: <this is your access token>
 ```
 
 # Pull Bricks
 To download a brick and save it locally in your library use `bb.pull`. An example using the Tox21 dataset:  
 
 ```python
+import biobricks as bb
 bb.install('tox21') # save the brick to the brick library and download it's resources
 tox21 = bb.load('tox21') # load a SimpleNamespace with all the brick tables
 
 # List the resources in the brick
 for tablename in sorted(list(vars(tox21).keys())):
     print(tablename)
     
-tox21.tox21_ache_p4.to_pandas() # get a pyarrow Table and convert to pandas dataframe
+tox21.tox21_ache_p4.read().to_pandas() # get a pyarrow Table and convert to pandas dataframe
 ```
 
 To list the bricks currently available visit [github.com/biobricks-ai](https://github.com/biobricks-ai)
```

