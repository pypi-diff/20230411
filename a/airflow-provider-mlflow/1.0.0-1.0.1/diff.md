# Comparing `tmp/airflow-provider-mlflow-1.0.0.tar.gz` & `tmp/airflow-provider-mlflow-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-mlflow-1.0.0.tar", last modified: Fri Apr  7 15:36:40 2023, max compression
+gzip compressed data, was "airflow-provider-mlflow-1.0.1.tar", last modified: Tue Apr 11 19:05:15 2023, max compression
```

## Comparing `airflow-provider-mlflow-1.0.0.tar` & `airflow-provider-mlflow-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:36:40.619386 airflow-provider-mlflow-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-07 15:36:40.619386 airflow-provider-mlflow-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:36:40.619386 airflow-provider-mlflow-1.0.0/airflow_provider_mlflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-07 15:36:40.000000 airflow-provider-mlflow-1.0.0/airflow_provider_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-07 15:36:40.000000 airflow-provider-mlflow-1.0.0/airflow_provider_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:36:40.000000 airflow-provider-mlflow-1.0.0/airflow_provider_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:36:40.000000 airflow-provider-mlflow-1.0.0/airflow_provider_mlflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-07 15:36:40.000000 airflow-provider-mlflow-1.0.0/airflow_provider_mlflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-07 15:36:40.000000 airflow-provider-mlflow-1.0.0/airflow_provider_mlflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:36:40.619386 airflow-provider-mlflow-1.0.0/mlflow_provider/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/mlflow_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/mlflow_provider/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:36:40.619386 airflow-provider-mlflow-1.0.0/mlflow_provider/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/mlflow_provider/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/mlflow_provider/hooks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/mlflow_provider/hooks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/mlflow_provider/hooks/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/mlflow_provider/hooks/pyfunc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:36:40.619386 airflow-provider-mlflow-1.0.0/mlflow_provider/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/mlflow_provider/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/mlflow_provider/operators/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/mlflow_provider/operators/pyfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/mlflow_provider/operators/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-07 15:36:40.619386 airflow-provider-mlflow-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 15:36:31.000000 airflow-provider-mlflow-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-11 19:05:15.000000 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-11 19:05:15.000000 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:05:15.000000 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:05:15.000000 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 19:05:15.000000 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 19:05:15.000000 airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/mlflow_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/pyfunc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/mlflow_provider/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/operators/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/operators/pyfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/mlflow_provider/operators/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-11 19:05:15.552349 airflow-provider-mlflow-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:05:06.000000 airflow-provider-mlflow-1.0.1/setup.py
```

### Comparing `airflow-provider-mlflow-1.0.0/LICENSE` & `airflow-provider-mlflow-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.0/PKG-INFO` & `airflow-provider-mlflow-1.0.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: airflow-provider-mlflow
-Version: 1.0.0
+Version: 1.0.1
 Summary: Apache Airflow provider for MLflow
 Home-page: https://github.com/astronomer/airflow-provider-mlflow
 Author: Faisal Hoda
 Author-email: faisal@astronomer.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/astronomer/airflow-provider-mlflow
 Project-URL: Homepage, https://github.com/astronomer/airflow-provider-mlflow
+Project-URL: Documentation, http://airflow-provider-mlflow.rtfd.io
+Project-URL: Changelog, https://github.com/astronomer/airflow-provider-mlflow/blob/main/CHANGELOG.rst
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -32,20 +34,47 @@
 - Deployments
 - Pyfunc
 
 https://mlflow.org/docs/latest/index.html
 
 Quick Start
 -----------
-Install and update using pip:
+**Install and update using pip:**
 
 .. code-block:: bash
 
     pip install airflow-provider-mlflow
 
+**Setting up Connections:**
+
+Connection Type: HTTP
+
+- Local MLflow
+    - Host: http://localhost (if running Airflwo in docker: http://host.docker.internal)
+    - Port: 5000
+
+- Hosted with Username/Password
+    - Connection Type: HTTP
+    - Host: Your MLflow host URL
+    - Login: Your MLflow username
+    - Password: Your MLflow password
+
+- Databricks
+    - Host: Your Databricks host URL (https://<instance-name>.cloud.databricks.com)
+    - Login: 'token'
+    - Password: Your Databricks token
+
+
 Examples can be found in the `example_dags <https://github.com/astronomer/airflow-provider-mlflow/tree/main/example_dags>`_ directory of the repo.
 
+Changelog
+---------
+
+We follow `Semantic Versioning <https://semver.org/>`_ for releases.
+Check `CHANGELOG.rst <https://github.com/astronomer/airflow-provider-mlflow/blob/main/CHANGELOG.rst>`_
+for the latest changes.
+
 
 License
 -------
 
 `Apache License 2.0 <https://github.com/astronomer/astronomer-providers/blob/main/LICENSE>`_
```

### Comparing `airflow-provider-mlflow-1.0.0/airflow_provider_mlflow.egg-info/PKG-INFO` & `airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: airflow-provider-mlflow
-Version: 1.0.0
+Version: 1.0.1
 Summary: Apache Airflow provider for MLflow
 Home-page: https://github.com/astronomer/airflow-provider-mlflow
 Author: Faisal Hoda
 Author-email: faisal@astronomer.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/astronomer/airflow-provider-mlflow
 Project-URL: Homepage, https://github.com/astronomer/airflow-provider-mlflow
+Project-URL: Documentation, http://airflow-provider-mlflow.rtfd.io
+Project-URL: Changelog, https://github.com/astronomer/airflow-provider-mlflow/blob/main/CHANGELOG.rst
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -32,20 +34,47 @@
 - Deployments
 - Pyfunc
 
 https://mlflow.org/docs/latest/index.html
 
 Quick Start
 -----------
-Install and update using pip:
+**Install and update using pip:**
 
 .. code-block:: bash
 
     pip install airflow-provider-mlflow
 
+**Setting up Connections:**
+
+Connection Type: HTTP
+
+- Local MLflow
+    - Host: http://localhost (if running Airflwo in docker: http://host.docker.internal)
+    - Port: 5000
+
+- Hosted with Username/Password
+    - Connection Type: HTTP
+    - Host: Your MLflow host URL
+    - Login: Your MLflow username
+    - Password: Your MLflow password
+
+- Databricks
+    - Host: Your Databricks host URL (https://<instance-name>.cloud.databricks.com)
+    - Login: 'token'
+    - Password: Your Databricks token
+
+
 Examples can be found in the `example_dags <https://github.com/astronomer/airflow-provider-mlflow/tree/main/example_dags>`_ directory of the repo.
 
+Changelog
+---------
+
+We follow `Semantic Versioning <https://semver.org/>`_ for releases.
+Check `CHANGELOG.rst <https://github.com/astronomer/airflow-provider-mlflow/blob/main/CHANGELOG.rst>`_
+for the latest changes.
+
 
 License
 -------
 
 `Apache License 2.0 <https://github.com/astronomer/astronomer-providers/blob/main/LICENSE>`_
```

### Comparing `airflow-provider-mlflow-1.0.0/airflow_provider_mlflow.egg-info/SOURCES.txt` & `airflow-provider-mlflow-1.0.1/airflow_provider_mlflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.0/mlflow_provider/__init__.py` & `airflow-provider-mlflow-1.0.1/mlflow_provider/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ## This is needed to allow Airflow to pick up specific metadata fields it needs for certain features. We recognize it's a bit unclean to define these in multiple places, but at this point it's the only workaround if you'd like your custom conn type to show up in the Airflow UI.
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 def get_provider_info():
     return {
         "package-name": "airflow-provider-sample", # Required
         "name": "Sample Airflow Provider", # Required
         "description": "A sample template for airflow providers.", # Required
         "hook-class-names": ["mlflow_provider.hooks.sample_hook.MLflowHook"],
```

### Comparing `airflow-provider-mlflow-1.0.0/mlflow_provider/hooks/base.py` & `airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/base.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.0/mlflow_provider/hooks/client.py` & `airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/client.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.0/mlflow_provider/hooks/deployment.py` & `airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/deployment.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.0/mlflow_provider/hooks/pyfunc.py` & `airflow-provider-mlflow-1.0.1/mlflow_provider/hooks/pyfunc.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.0/mlflow_provider/operators/deployment.py` & `airflow-provider-mlflow-1.0.1/mlflow_provider/operators/deployment.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.0/mlflow_provider/operators/pyfunc.py` & `airflow-provider-mlflow-1.0.1/mlflow_provider/operators/pyfunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
     # Load Model
     loaded_model = pyfunc.load_model(
         model_uri=model_uri,
         suppress_warnings=suppress_warnings,
         dst_path=dst_path
     )
 
+    loaded_model.metadata.signature = None
+
     # Run Inference and convert results to list of json depending on result type
     if isinstance(data, list):
         result = loaded_model.predict(data=nparray(data))
     else:
         result = loaded_model.predict(data=data)
 
     if type(result) is ndarray:
```

### Comparing `airflow-provider-mlflow-1.0.0/mlflow_provider/operators/registry.py` & `airflow-provider-mlflow-1.0.1/mlflow_provider/operators/registry.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-mlflow-1.0.0/setup.cfg` & `airflow-provider-mlflow-1.0.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 project_urls = 
 	Source Code=https://github.com/astronomer/airflow-provider-mlflow
 	Homepage=https://github.com/astronomer/airflow-provider-mlflow
+	Documentation=http://airflow-provider-mlflow.rtfd.io
+	Changelog=https://github.com/astronomer/airflow-provider-mlflow/blob/main/CHANGELOG.rst
 
 [options]
 python_requires = >=3.8
 packages = find:
 include_package_data = true
 install_requires = 
 	apache-airflow>=2.2.0
```

