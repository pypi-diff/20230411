# Comparing `tmp/idun_guardian_client-1.1b4.tar.gz` & `tmp/idun_guardian_client-1.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idun_guardian_client-1.1b4.tar", last modified: Tue Apr 11 07:28:50 2023, max compression
+gzip compressed data, was "idun_guardian_client-1.1b9.tar", last modified: Tue Apr 11 19:28:24 2023, max compression
```

## Comparing `idun_guardian_client-1.1b4.tar` & `idun_guardian_client-1.1b9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 07:28:50.205638 idun_guardian_client-1.1b4/
--rw-r--r--   0 waddaben   (501) staff       (20)     8991 2023-04-11 07:28:50.205391 idun_guardian_client-1.1b4/PKG-INFO
--rw-r--r--   0 waddaben   (501) staff       (20)     8426 2023-04-11 07:25:03.000000 idun_guardian_client-1.1b4/README.md
--rw-r--r--   0 waddaben   (501) staff       (20)      869 2023-04-11 07:25:34.000000 idun_guardian_client-1.1b4/pyproject.toml
--rw-r--r--   0 waddaben   (501) staff       (20)       38 2023-04-11 07:28:50.205692 idun_guardian_client-1.1b4/setup.cfg
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 07:28:50.199288 idun_guardian_client-1.1b4/src/
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 07:28:50.203341 idun_guardian_client-1.1b4/src/idun_guardian_client/
--rw-r--r--   0 waddaben   (501) staff       (20)      339 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/__init__.py
--rw-r--r--   0 waddaben   (501) staff       (20)        0 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/__main__.py
--rw-r--r--   0 waddaben   (501) staff       (20)     8661 2023-04-11 07:10:00.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/client.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1797 2023-04-07 12:29:46.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/config.py
--rw-r--r--   0 waddaben   (501) staff       (20)    11623 2023-04-07 15:53:12.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/debug_logs.py
--rw-r--r--   0 waddaben   (501) staff       (20)    20783 2023-04-07 21:23:44.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/igeb_api.py
--rw-r--r--   0 waddaben   (501) staff       (20)    30620 2023-04-07 21:24:40.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/igeb_bluetooth.py
--rw-r--r--   0 waddaben   (501) staff       (20)     2846 2023-04-07 11:46:38.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/igeb_utils.py
--rw-r--r--   0 waddaben   (501) staff       (20)      191 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/mock_utils.py
--rw-r--r--   0 waddaben   (501) staff       (20)      164 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/setup.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1214 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/src/idun_guardian_client/test_producer_consumer.py
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 07:28:50.204411 idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/
--rw-r--r--   0 waddaben   (501) staff       (20)     8991 2023-04-11 07:28:50.000000 idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/PKG-INFO
--rw-r--r--   0 waddaben   (501) staff       (20)      752 2023-04-11 07:28:50.000000 idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/SOURCES.txt
--rw-r--r--   0 waddaben   (501) staff       (20)        1 2023-04-11 07:28:50.000000 idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/dependency_links.txt
--rw-r--r--   0 waddaben   (501) staff       (20)      137 2023-04-11 07:28:50.000000 idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/requires.txt
--rw-r--r--   0 waddaben   (501) staff       (20)       21 2023-04-11 07:28:50.000000 idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/top_level.txt
-drwxr-xr-x   0 waddaben   (501) staff       (20)        0 2023-04-11 07:28:50.205055 idun_guardian_client-1.1b4/tests/
--rw-r--r--   0 waddaben   (501) staff       (20)     1940 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/tests/test_ble.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1672 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/tests/test_ble_record.py
--rw-r--r--   0 waddaben   (501) staff       (20)     1106 2023-04-06 15:19:16.000000 idun_guardian_client-1.1b4/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:28:24.435719 idun_guardian_client-1.1b9/
+-rw-rw-rw-   0        0        0     9259 2023-04-11 19:28:24.434721 idun_guardian_client-1.1b9/PKG-INFO
+-rw-rw-rw-   0        0        0     8680 2023-04-11 19:14:50.000000 idun_guardian_client-1.1b9/README.md
+-rw-rw-rw-   0        0        0      906 2023-04-11 19:27:44.000000 idun_guardian_client-1.1b9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 19:28:24.436716 idun_guardian_client-1.1b9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 19:28:24.332890 idun_guardian_client-1.1b9/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 19:28:24.381682 idun_guardian_client-1.1b9/src/idun_guardian_client/
+-rw-rw-rw-   0        0        0      351 2023-04-11 19:14:51.000000 idun_guardian_client-1.1b9/src/idun_guardian_client/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 19:14:51.000000 idun_guardian_client-1.1b9/src/idun_guardian_client/__main__.py
+-rw-rw-rw-   0        0        0     8881 2023-04-11 19:14:51.000000 idun_guardian_client-1.1b9/src/idun_guardian_client/client.py
+-rw-rw-rw-   0        0        0     1841 2023-04-11 19:14:51.000000 idun_guardian_client-1.1b9/src/idun_guardian_client/config.py
+-rw-rw-rw-   0        0        0    12059 2023-04-11 19:15:28.000000 idun_guardian_client-1.1b9/src/idun_guardian_client/debug_logs.py
+-rw-rw-rw-   0        0        0    21239 2023-04-11 19:15:28.000000 idun_guardian_client-1.1b9/src/idun_guardian_client/igeb_api.py
+-rw-rw-rw-   0        0        0    31451 2023-04-11 19:15:28.000000 idun_guardian_client-1.1b9/src/idun_guardian_client/igeb_bluetooth.py
+-rw-rw-rw-   0        0        0     2968 2023-04-11 19:14:51.000000 idun_guardian_client-1.1b9/src/idun_guardian_client/igeb_utils.py
+-rw-rw-rw-   0        0        0      200 2023-04-11 19:14:51.000000 idun_guardian_client-1.1b9/src/idun_guardian_client/mock_utils.py
+-rw-rw-rw-   0        0        0      174 2023-04-11 19:14:51.000000 idun_guardian_client-1.1b9/src/idun_guardian_client/setup.py
+-rw-rw-rw-   0        0        0     1263 2023-04-11 19:14:51.000000 idun_guardian_client-1.1b9/src/idun_guardian_client/test_producer_consumer.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:28:24.423595 idun_guardian_client-1.1b9/src/idun_guardian_client.egg-info/
+-rw-rw-rw-   0        0        0     9259 2023-04-11 19:28:24.000000 idun_guardian_client-1.1b9/src/idun_guardian_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      752 2023-04-11 19:28:24.000000 idun_guardian_client-1.1b9/src/idun_guardian_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 19:28:24.000000 idun_guardian_client-1.1b9/src/idun_guardian_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-04-11 19:28:24.000000 idun_guardian_client-1.1b9/src/idun_guardian_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-11 19:28:24.000000 idun_guardian_client-1.1b9/src/idun_guardian_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 19:28:24.431729 idun_guardian_client-1.1b9/tests/
+-rw-rw-rw-   0        0        0     2017 2023-04-11 19:14:51.000000 idun_guardian_client-1.1b9/tests/test_ble.py
+-rw-rw-rw-   0        0        0     1738 2023-04-11 19:14:51.000000 idun_guardian_client-1.1b9/tests/test_ble_record.py
+-rw-rw-rw-   0        0        0     1151 2023-04-11 19:14:51.000000 idun_guardian_client-1.1b9/tests/test_utils.py
```

### Comparing `idun_guardian_client-1.1b4/PKG-INFO` & `idun_guardian_client-1.1b9/src/idun_guardian_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,268 +1,268 @@
-Metadata-Version: 2.1
-Name: idun_guardian_client
-Version: 1.1b4
-Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
-Author-email: IDUN Technologies <contact@iduntechnologies.com>
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: Other/Proprietary License
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Natural Language :: English
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
-# User guide and documentation
-
-## What can you do with the Python SDK?
-
-1. You can use the Python SDK to search for the device.
-2. You can use the Python SDK to connect and record data from the earbud.
-3. You can download the data to your local machine.
-
----
-
-## Prerequisites
-
-- [Python 3.10](https://www.python.org/downloads/release/python-3100), if you already have another python version installed and you do not want to create a virtual environment to run the SDK, then you have to install Python 3.10 and [set it as your default Python](https://www.youtube.com/watch?v=zriWqGNJg4k).
-    - If you have conflicts with other packages when installing the Python SDK:
-        -  Use [Conda](https://www.anaconda.com/products/distribution) which will create an environment and configure your python version to the correct one with the following command: 
-        
-        ```bash
-        conda create -n idun_env python=3.10
-        ```
-        or
-        - Use [Pipenv](https://pypi.org/project/pipenv/) which will create your virtual environment manually using the following command.
-        ```bash
-        pipenv install --python 3.10
-        ```
----
-
-## Quick installation guide
-
-1. Create a new repository or folder
-2. Open the terminal in the same folder location or direct to that location within an already open terminal. For Windows you can use command prompt or Anaconda prompt, and Mac OS you can use the terminal or Anaconda prompt.
-
-3. First activate the virtual environment if you have created one by using the following command, this command must always be run before using the python SDK:
-    ```bash
-    conda activate idun_env
-    ```
-    or
-    ```bash
-    pipenv shell
-    ```
-
-4. After the environment is activated, install the Python SDK using the following command:
-    - With a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) use the following command:
-    ```bash
-    pip install idun-guardian-client
-    ```
-    or
-    - With a [pipenv environment](https://pypi.org/project/pipenv/) use the following command:
-    ```bash
-    pipenv install idun-guardian-client
-    ```
-
-5. After installing the package, make sure that the dependencies are correctly installed by running the following command and inspecting the packages installed in the terminal output:
-
-    ```bash
-    pip list
-    ```
-
----
-
-## How to use the Python SDK
-
-You can also download all the SDK example files from our [GitHub repository](https://github.com/iduntech/idun-guardian-client-examples.git), or copy and paste it from the examples below.
-
-### Example 1: Search for the device
-
-1. Create a new file inside the folder where you created your environment and name it `search.py`
-2. Open the terminal in the folder and activate your virtual environment using the steps from the [Quick installation guide](#quick-installation-guide).
-3. Open the `search.py` file and copy the code from step 1 below.
-4. Activate the virtual environment **only** if you have not already done so by using:
-
-    ```bash
-    conda activate idun_env
-    ```
-    or
-    ```bash
-    pipenv shell
-    ```
-4. Run the following command in the terminal to run the code after you have activate the enviroment:
-    ```bash
-    python search.py
-    ```
-
-#### Recommendation of steps to follow which is elaborated further below
-
-1. Search for the device
-2. Check the battery level
-3. Check the impedance
-4. Record data from the earbud
-5. Download the data from the cloud using the recording ID
-
-### **1. Search the earbud manually**
-
-- To search for the earbud, you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-bci = GuardianClient()
-
-device_address = asyncio.run(bci.search_device())
-```
-
-- Follow the steps in the terminal to search for the earbud with the name `IGEB`
-- If there are more than one IGEB device in the area, you will be asked to select the device you want to connect to connect to, a list such as below will pop up in the terminal:
-
-    - For Windows:
-    ```bash
-    ----- Available devices -----
-
-    Index | Name | Address
-    ----------------------------
-    0     | IGEB | XX:XX:XX:XX:XX:XX
-    1     | IGEB | XX:XX:XX:XX:XX:XX
-    2     | IGEB | XX:XX:XX:XX:XX:XX
-    ----------------------------
-    ```
-    - For Mac OS:
-    ```bash
-    ----- Available devices -----
-    Index | Name | UUID
-    ----------------------------
-    0    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
-    1    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
-    2    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
-    ----------------------------
-    ```
-
-- Enter the index number of the device you want to connect to.
-
-
-### **2. Check battery level**
-
-- To read out the battery level, you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-bci = GuardianClient()
-bci.address = asyncio.run(bci.search_device())
-
-asyncio.run(bci.start_battery())
-```
-
-### **3. Check impedance values**
-
-- To read out the impedance values, you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-IMPEDANCE_DURATION = 5  # duration of impedance measurement in seconds
-MAINS_FREQUENCY_60Hz = False
-# mains frequency in Hz (50 or 60), for Europe 50Hz, for US 60Hz
-
-
-# Get device address
-bci = GuardianClient()
-bci.address = asyncio.run(bci.search_device())
-
-# start a recording session
-asyncio.run(
-    bci.start_recording(
-        recording_timer=IMPEDANCE_DURATION,
-        mains_freq_60hz=MAINS_FREQUENCY_60Hz,
-        impedance_measurement=True)
-)
-```
-
-### **4. Start a recording**
-
-- To start a recording with a pre-defined timer (e.g. `100` in seconds), you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-EXPERIMENT: str = "Sleeping"
-RECORDING_TIMER: int = 36000 # 10 hours in seconds
-LED_SLEEP: bool = False
-SENDING_TIMEOUT: float = 2 # No sending receipt time before interrupt
-BI_DIRECTIONAL_TIMEOUT: float = 20 # No bi-directional data receiving before interrupt
-
-# start a recording session
-bci = GuardianClient()
-bci.address = asyncio.run(bci.search_device())
-
-# start a recording session
-asyncio.run(
-    bci.start_recording(
-        recording_timer=RECORDING_TIMER,
-        led_sleep=LED_SLEEP,
-        experiment=EXPERIMENT,
-        sending_timout=SENDING_TIMEOUT,
-        bi_directional_receiving_timeout=BI_DIRECTIONAL_TIMEOUT,
-    )
-)
-
-```
-
-- To stop the recording, either wait for the timer to run out or interrupt the recording
-    - with Mac OS enter the cancellation command in the terminal running the script, this would be `Ctrl+.` or `Ctrl+C`
-    - with Windows enter the cancellation command in the terminal running the script, this would be `Ctrl+C` or `Ctrl+Shift+C`
-
-### **4. Get all recorded info**
-
-- To download the data, you need to first get the list of all your recordings and choose the one you would like to download
-- Run the following command in your python shell or in your python script:
-
-```python
-from idun_guardian_client.igeb_api import GuardianAPI
-
-api = GuardianAPI()
-
-# get a list of all recordings
-recording_list = api.get_recordings_info_all(device_id = "XX-XX-XX-XX-XX-XX") # Device ID is derived from the MAC address of the earbud and in the log file
-
-```
-
-### **5. Get recording info**
-
-- To list the information on a specific recording, you need to run the following command in your python shell or in your python script:
-
-```python
-from idun_guardian_client.igeb_api import GuardianAPI
-
-api = GuardianAPI()
-
-# get single recording
-api.get_recording_info_by_id(
-    device_id = "XX-XX-XX-XX-XX-XX",
-    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
-)
-
-```
-
-### **5. Download recording**
-
-- To download the data insert the `device_id` along with the `recording_id` and run the following command in your python shell or in your python script
-
-```python
-from idun_guardian_client.igeb_api import GuardianAPI
-
-api = GuardianAPI()
-
-# download recording
-api.download_recording_by_id(
-    device_id = "XX-XX-XX-XX-XX-XX",
-    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxx"
-)
-# The info about th recording can be found in the log file
-```
+Metadata-Version: 2.1
+Name: idun-guardian-client
+Version: 1.1b9
+Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
+Author-email: IDUN Technologies <contact@iduntechnologies.com>
+Classifier: Development Status :: 1 - Planning
+Classifier: License :: Other/Proprietary License
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Natural Language :: English
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
+# User guide and documentation
+
+## What can you do with the Python SDK?
+
+1. You can use the Python SDK to search for the device.
+2. You can use the Python SDK to connect and record data from the earbud.
+3. You can download the data to your local machine.
+
+---
+
+## Prerequisites
+
+- [Python 3.10](https://www.python.org/downloads/release/python-3100), if you already have another python version installed and you do not want to create a virtual environment to run the SDK, then you have to install Python 3.10 and [set it as your default Python](https://www.youtube.com/watch?v=zriWqGNJg4k).
+    - If you have conflicts with other packages when installing the Python SDK:
+        -  Use [Conda](https://www.anaconda.com/products/distribution) which will create an environment and configure your python version to the correct one with the following command: 
+        
+        ```bash
+        conda create -n idun_env python=3.10
+        ```
+        or
+        - Use [Pipenv](https://pypi.org/project/pipenv/) which will create your virtual environment manually using the following command.
+        ```bash
+        pipenv install --python 3.10
+        ```
+---
+
+## Quick installation guide
+
+1. Create a new repository or folder
+2. Open the terminal in the same folder location or direct to that location within an already open terminal. For Windows you can use command prompt or Anaconda prompt, and Mac OS you can use the terminal or Anaconda prompt.
+
+3. First activate the virtual environment if you have created one by using the following command, this command must always be run before using the python SDK:
+    ```bash
+    conda activate idun_env
+    ```
+    or
+    ```bash
+    pipenv shell
+    ```
+
+4. After the environment is activated, install the Python SDK using the following command:
+    - With a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) use the following command:
+    ```bash
+    pip install idun-guardian-client
+    ```
+    or
+    - With a [pipenv environment](https://pypi.org/project/pipenv/) use the following command:
+    ```bash
+    pipenv install idun-guardian-client
+    ```
+
+5. After installing the package, make sure that the dependencies are correctly installed by running the following command and inspecting the packages installed in the terminal output:
+
+    ```bash
+    pip list
+    ```
+
+---
+
+## How to use the Python SDK
+
+You can also download all the SDK example files from our [GitHub repository](https://github.com/iduntech/idun-guardian-client-examples.git), or copy and paste it from the examples below.
+
+### Example 1: Search for the device
+
+1. Create a new file inside the folder where you created your environment and name it `search.py`
+2. Open the terminal in the folder and activate your virtual environment using the steps from the [Quick installation guide](#quick-installation-guide).
+3. Open the `search.py` file and copy the code from step 1 below.
+4. Activate the virtual environment **only** if you have not already done so by using:
+
+    ```bash
+    conda activate idun_env
+    ```
+    or
+    ```bash
+    pipenv shell
+    ```
+4. Run the following command in the terminal to run the code after you have activate the enviroment:
+    ```bash
+    python search.py
+    ```
+
+#### Recommendation of steps to follow which is elaborated further below
+
+1. Search for the device
+2. Check the battery level
+3. Check the impedance
+4. Record data from the earbud
+5. Download the data from the cloud using the recording ID
+
+### **1. Search the earbud manually**
+
+- To search for the earbud, you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+bci = GuardianClient()
+
+device_address = asyncio.run(bci.search_device())
+```
+
+- Follow the steps in the terminal to search for the earbud with the name `IGEB`
+- If there are more than one IGEB device in the area, you will be asked to select the device you want to connect to connect to, a list such as below will pop up in the terminal:
+
+    - For Windows:
+    ```bash
+    ----- Available devices -----
+
+    Index | Name | Address
+    ----------------------------
+    0     | IGEB | XX:XX:XX:XX:XX:XX
+    1     | IGEB | XX:XX:XX:XX:XX:XX
+    2     | IGEB | XX:XX:XX:XX:XX:XX
+    ----------------------------
+    ```
+    - For Mac OS:
+    ```bash
+    ----- Available devices -----
+    Index | Name | UUID
+    ----------------------------
+    0    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
+    1    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
+    2    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
+    ----------------------------
+    ```
+
+- Enter the index number of the device you want to connect to.
+
+
+### **2. Check battery level**
+
+- To read out the battery level, you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+bci = GuardianClient()
+bci.address = asyncio.run(bci.search_device())
+
+asyncio.run(bci.start_battery())
+```
+
+### **3. Check impedance values**
+
+- To read out the impedance values, you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+IMPEDANCE_DURATION = 5  # duration of impedance measurement in seconds
+MAINS_FREQUENCY_60Hz = False
+# mains frequency in Hz (50 or 60), for Europe 50Hz, for US 60Hz
+
+
+# Get device address
+bci = GuardianClient()
+bci.address = asyncio.run(bci.search_device())
+
+# start a recording session
+asyncio.run(
+    bci.start_recording(
+        recording_timer=IMPEDANCE_DURATION,
+        mains_freq_60hz=MAINS_FREQUENCY_60Hz,
+        impedance_measurement=True)
+)
+```
+
+### **4. Start a recording**
+
+- To start a recording with a pre-defined timer (e.g. `100` in seconds), you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+EXPERIMENT: str = "Sleeping"
+RECORDING_TIMER: int = 36000 # 10 hours in seconds
+LED_SLEEP: bool = False
+SENDING_TIMEOUT: float = 2 # No sending receipt time before interrupt
+BI_DIRECTIONAL_TIMEOUT: float = 20 # No bi-directional data receiving before interrupt
+
+# start a recording session
+bci = GuardianClient()
+bci.address = asyncio.run(bci.search_device())
+
+# start a recording session
+asyncio.run(
+    bci.start_recording(
+        recording_timer=RECORDING_TIMER,
+        led_sleep=LED_SLEEP,
+        experiment=EXPERIMENT,
+        sending_timout=SENDING_TIMEOUT,
+        bi_directional_receiving_timeout=BI_DIRECTIONAL_TIMEOUT,
+    )
+)
+
+```
+
+- To stop the recording, either wait for the timer to run out or interrupt the recording
+    - with Mac OS enter the cancellation command in the terminal running the script, this would be `Ctrl+.` or `Ctrl+C`
+    - with Windows enter the cancellation command in the terminal running the script, this would be `Ctrl+C` or `Ctrl+Shift+C`
+
+### **4. Get all recorded info**
+
+- To download the data, you need to first get the list of all your recordings and choose the one you would like to download
+- Run the following command in your python shell or in your python script:
+
+```python
+from idun_guardian_client.igeb_api import GuardianAPI
+
+api = GuardianAPI()
+
+# get a list of all recordings
+recording_list = api.get_recordings_info_all(device_id = "XX-XX-XX-XX-XX-XX") # Device ID is derived from the MAC address of the earbud and in the log file
+
+```
+
+### **5. Get recording info**
+
+- To list the information on a specific recording, you need to run the following command in your python shell or in your python script:
+
+```python
+from idun_guardian_client.igeb_api import GuardianAPI
+
+api = GuardianAPI()
+
+# get single recording
+api.get_recording_info_by_id(
+    device_id = "XX-XX-XX-XX-XX-XX",
+    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
+)
+
+```
+
+### **5. Download recording**
+
+- To download the data insert the `device_id` along with the `recording_id` and run the following command in your python shell or in your python script
+
+```python
+from idun_guardian_client.igeb_api import GuardianAPI
+
+api = GuardianAPI()
+
+# download recording
+api.download_recording_by_id(
+    device_id = "XX-XX-XX-XX-XX-XX",
+    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxx"
+)
+# The info about th recording can be found in the log file
+```
```

### Comparing `idun_guardian_client-1.1b4/README.md` & `idun_guardian_client-1.1b9/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,254 +1,254 @@
-# User guide and documentation
-
-## What can you do with the Python SDK?
-
-1. You can use the Python SDK to search for the device.
-2. You can use the Python SDK to connect and record data from the earbud.
-3. You can download the data to your local machine.
-
----
-
-## Prerequisites
-
-- [Python 3.10](https://www.python.org/downloads/release/python-3100), if you already have another python version installed and you do not want to create a virtual environment to run the SDK, then you have to install Python 3.10 and [set it as your default Python](https://www.youtube.com/watch?v=zriWqGNJg4k).
-    - If you have conflicts with other packages when installing the Python SDK:
-        -  Use [Conda](https://www.anaconda.com/products/distribution) which will create an environment and configure your python version to the correct one with the following command: 
-        
-        ```bash
-        conda create -n idun_env python=3.10
-        ```
-        or
-        - Use [Pipenv](https://pypi.org/project/pipenv/) which will create your virtual environment manually using the following command.
-        ```bash
-        pipenv install --python 3.10
-        ```
----
-
-## Quick installation guide
-
-1. Create a new repository or folder
-2. Open the terminal in the same folder location or direct to that location within an already open terminal. For Windows you can use command prompt or Anaconda prompt, and Mac OS you can use the terminal or Anaconda prompt.
-
-3. First activate the virtual environment if you have created one by using the following command, this command must always be run before using the python SDK:
-    ```bash
-    conda activate idun_env
-    ```
-    or
-    ```bash
-    pipenv shell
-    ```
-
-4. After the environment is activated, install the Python SDK using the following command:
-    - With a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) use the following command:
-    ```bash
-    pip install idun-guardian-client
-    ```
-    or
-    - With a [pipenv environment](https://pypi.org/project/pipenv/) use the following command:
-    ```bash
-    pipenv install idun-guardian-client
-    ```
-
-5. After installing the package, make sure that the dependencies are correctly installed by running the following command and inspecting the packages installed in the terminal output:
-
-    ```bash
-    pip list
-    ```
-
----
-
-## How to use the Python SDK
-
-You can also download all the SDK example files from our [GitHub repository](https://github.com/iduntech/idun-guardian-client-examples.git), or copy and paste it from the examples below.
-
-### Example 1: Search for the device
-
-1. Create a new file inside the folder where you created your environment and name it `search.py`
-2. Open the terminal in the folder and activate your virtual environment using the steps from the [Quick installation guide](#quick-installation-guide).
-3. Open the `search.py` file and copy the code from step 1 below.
-4. Activate the virtual environment **only** if you have not already done so by using:
-
-    ```bash
-    conda activate idun_env
-    ```
-    or
-    ```bash
-    pipenv shell
-    ```
-4. Run the following command in the terminal to run the code after you have activate the enviroment:
-    ```bash
-    python search.py
-    ```
-
-#### Recommendation of steps to follow which is elaborated further below
-
-1. Search for the device
-2. Check the battery level
-3. Check the impedance
-4. Record data from the earbud
-5. Download the data from the cloud using the recording ID
-
-### **1. Search the earbud manually**
-
-- To search for the earbud, you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-bci = GuardianClient()
-
-device_address = asyncio.run(bci.search_device())
-```
-
-- Follow the steps in the terminal to search for the earbud with the name `IGEB`
-- If there are more than one IGEB device in the area, you will be asked to select the device you want to connect to connect to, a list such as below will pop up in the terminal:
-
-    - For Windows:
-    ```bash
-    ----- Available devices -----
-
-    Index | Name | Address
-    ----------------------------
-    0     | IGEB | XX:XX:XX:XX:XX:XX
-    1     | IGEB | XX:XX:XX:XX:XX:XX
-    2     | IGEB | XX:XX:XX:XX:XX:XX
-    ----------------------------
-    ```
-    - For Mac OS:
-    ```bash
-    ----- Available devices -----
-    Index | Name | UUID
-    ----------------------------
-    0    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
-    1    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
-    2    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
-    ----------------------------
-    ```
-
-- Enter the index number of the device you want to connect to.
-
-
-### **2. Check battery level**
-
-- To read out the battery level, you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-bci = GuardianClient()
-bci.address = asyncio.run(bci.search_device())
-
-asyncio.run(bci.start_battery())
-```
-
-### **3. Check impedance values**
-
-- To read out the impedance values, you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-IMPEDANCE_DURATION = 5  # duration of impedance measurement in seconds
-MAINS_FREQUENCY_60Hz = False
-# mains frequency in Hz (50 or 60), for Europe 50Hz, for US 60Hz
-
-
-# Get device address
-bci = GuardianClient()
-bci.address = asyncio.run(bci.search_device())
-
-# start a recording session
-asyncio.run(
-    bci.start_recording(
-        recording_timer=IMPEDANCE_DURATION,
-        mains_freq_60hz=MAINS_FREQUENCY_60Hz,
-        impedance_measurement=True)
-)
-```
-
-### **4. Start a recording**
-
-- To start a recording with a pre-defined timer (e.g. `100` in seconds), you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-EXPERIMENT: str = "Sleeping"
-RECORDING_TIMER: int = 36000 # 10 hours in seconds
-LED_SLEEP: bool = False
-SENDING_TIMEOUT: float = 2 # No sending receipt time before interrupt
-BI_DIRECTIONAL_TIMEOUT: float = 20 # No bi-directional data receiving before interrupt
-
-# start a recording session
-bci = GuardianClient()
-bci.address = asyncio.run(bci.search_device())
-
-# start a recording session
-asyncio.run(
-    bci.start_recording(
-        recording_timer=RECORDING_TIMER,
-        led_sleep=LED_SLEEP,
-        experiment=EXPERIMENT,
-        sending_timout=SENDING_TIMEOUT,
-        bi_directional_receiving_timeout=BI_DIRECTIONAL_TIMEOUT,
-    )
-)
-
-```
-
-- To stop the recording, either wait for the timer to run out or interrupt the recording
-    - with Mac OS enter the cancellation command in the terminal running the script, this would be `Ctrl+.` or `Ctrl+C`
-    - with Windows enter the cancellation command in the terminal running the script, this would be `Ctrl+C` or `Ctrl+Shift+C`
-
-### **4. Get all recorded info**
-
-- To download the data, you need to first get the list of all your recordings and choose the one you would like to download
-- Run the following command in your python shell or in your python script:
-
-```python
-from idun_guardian_client.igeb_api import GuardianAPI
-
-api = GuardianAPI()
-
-# get a list of all recordings
-recording_list = api.get_recordings_info_all(device_id = "XX-XX-XX-XX-XX-XX") # Device ID is derived from the MAC address of the earbud and in the log file
-
-```
-
-### **5. Get recording info**
-
-- To list the information on a specific recording, you need to run the following command in your python shell or in your python script:
-
-```python
-from idun_guardian_client.igeb_api import GuardianAPI
-
-api = GuardianAPI()
-
-# get single recording
-api.get_recording_info_by_id(
-    device_id = "XX-XX-XX-XX-XX-XX",
-    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
-)
-
-```
-
-### **5. Download recording**
-
-- To download the data insert the `device_id` along with the `recording_id` and run the following command in your python shell or in your python script
-
-```python
-from idun_guardian_client.igeb_api import GuardianAPI
-
-api = GuardianAPI()
-
-# download recording
-api.download_recording_by_id(
-    device_id = "XX-XX-XX-XX-XX-XX",
-    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxx"
-)
-# The info about th recording can be found in the log file
-```
+# User guide and documentation
+
+## What can you do with the Python SDK?
+
+1. You can use the Python SDK to search for the device.
+2. You can use the Python SDK to connect and record data from the earbud.
+3. You can download the data to your local machine.
+
+---
+
+## Prerequisites
+
+- [Python 3.10](https://www.python.org/downloads/release/python-3100), if you already have another python version installed and you do not want to create a virtual environment to run the SDK, then you have to install Python 3.10 and [set it as your default Python](https://www.youtube.com/watch?v=zriWqGNJg4k).
+    - If you have conflicts with other packages when installing the Python SDK:
+        -  Use [Conda](https://www.anaconda.com/products/distribution) which will create an environment and configure your python version to the correct one with the following command: 
+        
+        ```bash
+        conda create -n idun_env python=3.10
+        ```
+        or
+        - Use [Pipenv](https://pypi.org/project/pipenv/) which will create your virtual environment manually using the following command.
+        ```bash
+        pipenv install --python 3.10
+        ```
+---
+
+## Quick installation guide
+
+1. Create a new repository or folder
+2. Open the terminal in the same folder location or direct to that location within an already open terminal. For Windows you can use command prompt or Anaconda prompt, and Mac OS you can use the terminal or Anaconda prompt.
+
+3. First activate the virtual environment if you have created one by using the following command, this command must always be run before using the python SDK:
+    ```bash
+    conda activate idun_env
+    ```
+    or
+    ```bash
+    pipenv shell
+    ```
+
+4. After the environment is activated, install the Python SDK using the following command:
+    - With a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) use the following command:
+    ```bash
+    pip install idun-guardian-client
+    ```
+    or
+    - With a [pipenv environment](https://pypi.org/project/pipenv/) use the following command:
+    ```bash
+    pipenv install idun-guardian-client
+    ```
+
+5. After installing the package, make sure that the dependencies are correctly installed by running the following command and inspecting the packages installed in the terminal output:
+
+    ```bash
+    pip list
+    ```
+
+---
+
+## How to use the Python SDK
+
+You can also download all the SDK example files from our [GitHub repository](https://github.com/iduntech/idun-guardian-client-examples.git), or copy and paste it from the examples below.
+
+### Example 1: Search for the device
+
+1. Create a new file inside the folder where you created your environment and name it `search.py`
+2. Open the terminal in the folder and activate your virtual environment using the steps from the [Quick installation guide](#quick-installation-guide).
+3. Open the `search.py` file and copy the code from step 1 below.
+4. Activate the virtual environment **only** if you have not already done so by using:
+
+    ```bash
+    conda activate idun_env
+    ```
+    or
+    ```bash
+    pipenv shell
+    ```
+4. Run the following command in the terminal to run the code after you have activate the enviroment:
+    ```bash
+    python search.py
+    ```
+
+#### Recommendation of steps to follow which is elaborated further below
+
+1. Search for the device
+2. Check the battery level
+3. Check the impedance
+4. Record data from the earbud
+5. Download the data from the cloud using the recording ID
+
+### **1. Search the earbud manually**
+
+- To search for the earbud, you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+bci = GuardianClient()
+
+device_address = asyncio.run(bci.search_device())
+```
+
+- Follow the steps in the terminal to search for the earbud with the name `IGEB`
+- If there are more than one IGEB device in the area, you will be asked to select the device you want to connect to connect to, a list such as below will pop up in the terminal:
+
+    - For Windows:
+    ```bash
+    ----- Available devices -----
+
+    Index | Name | Address
+    ----------------------------
+    0     | IGEB | XX:XX:XX:XX:XX:XX
+    1     | IGEB | XX:XX:XX:XX:XX:XX
+    2     | IGEB | XX:XX:XX:XX:XX:XX
+    ----------------------------
+    ```
+    - For Mac OS:
+    ```bash
+    ----- Available devices -----
+    Index | Name | UUID
+    ----------------------------
+    0    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
+    1    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
+    2    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
+    ----------------------------
+    ```
+
+- Enter the index number of the device you want to connect to.
+
+
+### **2. Check battery level**
+
+- To read out the battery level, you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+bci = GuardianClient()
+bci.address = asyncio.run(bci.search_device())
+
+asyncio.run(bci.start_battery())
+```
+
+### **3. Check impedance values**
+
+- To read out the impedance values, you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+IMPEDANCE_DURATION = 5  # duration of impedance measurement in seconds
+MAINS_FREQUENCY_60Hz = False
+# mains frequency in Hz (50 or 60), for Europe 50Hz, for US 60Hz
+
+
+# Get device address
+bci = GuardianClient()
+bci.address = asyncio.run(bci.search_device())
+
+# start a recording session
+asyncio.run(
+    bci.start_recording(
+        recording_timer=IMPEDANCE_DURATION,
+        mains_freq_60hz=MAINS_FREQUENCY_60Hz,
+        impedance_measurement=True)
+)
+```
+
+### **4. Start a recording**
+
+- To start a recording with a pre-defined timer (e.g. `100` in seconds), you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+EXPERIMENT: str = "Sleeping"
+RECORDING_TIMER: int = 36000 # 10 hours in seconds
+LED_SLEEP: bool = False
+SENDING_TIMEOUT: float = 2 # No sending receipt time before interrupt
+BI_DIRECTIONAL_TIMEOUT: float = 20 # No bi-directional data receiving before interrupt
+
+# start a recording session
+bci = GuardianClient()
+bci.address = asyncio.run(bci.search_device())
+
+# start a recording session
+asyncio.run(
+    bci.start_recording(
+        recording_timer=RECORDING_TIMER,
+        led_sleep=LED_SLEEP,
+        experiment=EXPERIMENT,
+        sending_timout=SENDING_TIMEOUT,
+        bi_directional_receiving_timeout=BI_DIRECTIONAL_TIMEOUT,
+    )
+)
+
+```
+
+- To stop the recording, either wait for the timer to run out or interrupt the recording
+    - with Mac OS enter the cancellation command in the terminal running the script, this would be `Ctrl+.` or `Ctrl+C`
+    - with Windows enter the cancellation command in the terminal running the script, this would be `Ctrl+C` or `Ctrl+Shift+C`
+
+### **4. Get all recorded info**
+
+- To download the data, you need to first get the list of all your recordings and choose the one you would like to download
+- Run the following command in your python shell or in your python script:
+
+```python
+from idun_guardian_client.igeb_api import GuardianAPI
+
+api = GuardianAPI()
+
+# get a list of all recordings
+recording_list = api.get_recordings_info_all(device_id = "XX-XX-XX-XX-XX-XX") # Device ID is derived from the MAC address of the earbud and in the log file
+
+```
+
+### **5. Get recording info**
+
+- To list the information on a specific recording, you need to run the following command in your python shell or in your python script:
+
+```python
+from idun_guardian_client.igeb_api import GuardianAPI
+
+api = GuardianAPI()
+
+# get single recording
+api.get_recording_info_by_id(
+    device_id = "XX-XX-XX-XX-XX-XX",
+    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
+)
+
+```
+
+### **5. Download recording**
+
+- To download the data insert the `device_id` along with the `recording_id` and run the following command in your python shell or in your python script
+
+```python
+from idun_guardian_client.igeb_api import GuardianAPI
+
+api = GuardianAPI()
+
+# download recording
+api.download_recording_by_id(
+    device_id = "XX-XX-XX-XX-XX-XX",
+    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxx"
+)
+# The info about th recording can be found in the log file
+```
```

### Comparing `idun_guardian_client-1.1b4/src/idun_guardian_client/client.py` & `idun_guardian_client-1.1b9/src/idun_guardian_client/client.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,220 +1,220 @@
-"""
-Initialization of the IDUN Guardian Client
-"""
-import os
-import asyncio
-from typing import Union
-import logging
-from datetime import datetime
-from .igeb_bluetooth import GuardianBLE
-from .igeb_api import GuardianAPI
-from .igeb_utils import check_platform, check_valid_mac, check_valid_uuid
-import uuid
-from typing import Union
-
-
-class GuardianClient:
-    """
-    Class object for the communication between Guardian Earbuds and Cloud API
-    """
-
-    def __init__(
-        self,
-        address: Union[str, None] = None,
-        debug=True,
-        debug_console=True,
-    ) -> None:
-        """Initialize the Guardian Client
-
-        Args:
-            address (str, optional): The MAC address of the Guardian Earbuds. Defaults to "00000000-0000-0000-0000-000000000000".
-            debug (bool, optional): Enable debug logging. Defaults to True.
-            debug_console (bool, optional): Enable debug logging to console. Defaults to True.
-
-        Raises:
-            ValueError: If the MAC address is not valid
-        """
-        self.is_connected = False
-        self.debug = debug
-        self.debug_to_console = debug_console
-        if self.debug:
-            self.configure_logger()
-
-        if address is not None:
-            if self.check_ble_address(address):
-                self.guardian_ble = GuardianBLE(address, debug=self.debug)
-                self.address = address
-        else:
-            logging.info("No BLE address provided, will search for device...")
-            print("No BLE address provided, will search for device..")
-            self.guardian_ble = GuardianBLE(debug=self.debug)
-
-        self.guardian_api = GuardianAPI(debug=self.debug)
-
-    def configure_logger(self):
-        """Configure the logger for the Guardian Client"""
-        if not os.path.exists("./logs"):
-            os.makedirs("logs")
-
-        datestr = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
-        log_filename = f"./logs/ble_info-{datestr}.log"
-
-        if not os.path.exists(os.path.dirname(log_filename)):
-            os.makedirs(os.path.dirname(log_filename))
-        log_handlers = [logging.FileHandler(log_filename)]
-
-        if self.debug_to_console:
-            log_handlers.append(logging.StreamHandler())
-
-        logging.basicConfig(
-            level=logging.INFO,
-            datefmt="%d-%b-%y %H:%M:%S",
-            format="%(asctime)s: %(name)s - %(levelname)s - %(message)s",
-            handlers=log_handlers,
-        )
-
-    def check_ble_address(self, address: str) -> bool:
-        """Check if the BLE address is valid
-
-        Args:
-            address (str): The MAC address of the Guardian Earbuds
-
-        Returns:
-            bool: True if the address is valid, False otherwise
-        """
-        if (
-            check_platform() == "Windows"
-            or check_platform() == "Linux"
-            and check_valid_mac(address)
-        ):
-            return True
-        elif check_platform() == "Darwin" and check_valid_uuid(address):
-            logging.info("Platform detected: Darwin")
-            # print(f"UUID is valid for system Darwin: {address}")
-            return True
-        else:
-            logging.error("Invalid BLE address")
-            raise ValueError("Invalid BLE address")
-
-    async def search_device(self):
-        """Connect to the Guardian Earbuds
-
-        Returns:
-            is_connected: bool
-        """
-
-        self.address = await self.guardian_ble.search_device()
-
-        return self.address
-
-    async def get_device_address(self) -> str:
-        """Get the MAC address of the Guardian Earbuds.
-        It searches the MAC address of the device automatically. This
-        address is used as the deviceID for cloud communication
-        """
-        device_address = await self.guardian_ble.get_device_mac()
-        return device_address
-
-    async def start_recording(
-        self,
-        recording_timer: int = 36000,
-        led_sleep: bool = False,
-        experiment: str = "None provided",
-        impedance_measurement: bool = False,
-        mains_freq_60hz: bool = False,
-        sending_timout: float = 2,
-        bi_directional_receiving_timeout: float = 5,
-    ):
-        """
-        Start recording data from the Guardian Earbuds.
-        Unidirectional websocket connection to the Guardian Cloud API.
-
-        Args:
-            recording_timer (int, optional): The duration of the recording in seconds. Defaults to 36000.
-            led_sleep (bool, optional): Enable LED sleep mode. Defaults to False.
-            experiment (str, optional): The name of the experiment. Defaults to "None provided". This will
-                                        go to the log file.
-            impedance_measurement (bool, optional): Enable impedance measurement. Defaults to False.
-            mains_freq_60hz (bool, optional): Set to True if the mains frequency is 60Hz. Defaults to False.
-            sending_timout (float): The timeout in seconds for sending data to the cloud. Defaults to 1.
-                                    If no data is sent for a second the sending is interupted and the data
-                                    is buffered. If you have a fast internet and you do not want to lose any data,
-                                    then make 0.5 seconds. If you have slow internet and are fine with losing some data,
-                                    then make 5 seconds. The seconds will be the amount lost before noticing internet loss.
-            bi_directional_receiving_timeout (float): The timeout in seconds for receiving data from the cloud. Defaults to 4.
-                                                      If no data is received for 5 seconds the receiving is interupted and the data
-                                                      the connection will be re-established. If you have a fast internet and you do not want to lose
-                                                      bi-directional data, then make 5 seconds. If you have slow internet and are fine with losing some data,
-                                                      then make 10 seconds. The seconds will be the amount lost before noticing internet loss.
-
-
-        Raises:
-            ValueError: If the recording timer is not valid
-        """
-        # set the timers
-        self.guardian_api.runtime_receipt_timeout = sending_timout
-        self.guardian_api.runtime_bi_directional_timeout = (
-            bi_directional_receiving_timeout
-        )
-
-        if self.debug:
-            logging.info(
-                "[CLIENT]: Recording timer set to: %s seconds", recording_timer
-            )
-            logging.info("[CLIENT]: Start recording")
-
-        print(f"[CLIENT]: Recording timer set to: {recording_timer} seconds")
-        print("-----Recording starting------")
-
-        data_queue: asyncio.Queue = asyncio.Queue(maxsize=86400)
-
-        recording_id = "py-" + str(
-            uuid.uuid4()
-        )  # the recordingID is a unique ID for each recording
-        logging.info("[CLIENT] Recording ID: %s", recording_id)
-        # log the experiment name in bold using the logging module
-        logging.info("[CLIENT] Experiment description: %s", experiment)
-        mac_id = await self.guardian_ble.get_device_mac()
-
-        tasks = []
-        tasks.append(
-            self.guardian_ble.run_ble_record(
-                data_queue,
-                recording_timer,
-                mac_id,
-                led_sleep,
-                impedance_measurement,
-                mains_freq_60hz,
-            )
-        )
-        tasks.append(
-            self.guardian_api.connect_ws_api(
-                data_queue, mac_id, recording_id, impedance_measurement
-            )
-        )
-
-        await asyncio.wait(tasks)
-        if self.debug:
-            logging.info("[CLIENT]: -----------  All tasks are COMPLETED -----------")
-        print(f"-----Recording ID {recording_id}------")
-        print(f"-----Device ID {mac_id}------")
-        print("-----Recording stopped------")
-
-    def stop_recording(self):
-        """Stop recording data from the Guardian Earbuds"""
-
-    async def start_battery(self):
-        """
-        Start recording data from the Guardian Earbuds.
-        Unidirectional websocket connection to the Guardian Cloud API.
-        """
-        print("-----Battery readout started------")
-        if self.debug:
-            logging.info("[CLIENT]: Start recording")
-
-        ble_client_task = self.guardian_ble.read_battery_level()
-        await asyncio.wait([ble_client_task])
-
-        if self.debug:
-            logging.info("[CLIENT]: Disconnect BLE and close websocket connection")
-        print("-----Battery check stopped------")
+"""
+Initialization of the IDUN Guardian Client
+"""
+import os
+import asyncio
+from typing import Union
+import logging
+from datetime import datetime
+from .igeb_bluetooth import GuardianBLE
+from .igeb_api import GuardianAPI
+from .igeb_utils import check_platform, check_valid_mac, check_valid_uuid
+import uuid
+from typing import Union
+
+
+class GuardianClient:
+    """
+    Class object for the communication between Guardian Earbuds and Cloud API
+    """
+
+    def __init__(
+        self,
+        address: Union[str, None] = None,
+        debug=True,
+        debug_console=True,
+    ) -> None:
+        """Initialize the Guardian Client
+
+        Args:
+            address (str, optional): The MAC address of the Guardian Earbuds. Defaults to "00000000-0000-0000-0000-000000000000".
+            debug (bool, optional): Enable debug logging. Defaults to True.
+            debug_console (bool, optional): Enable debug logging to console. Defaults to True.
+
+        Raises:
+            ValueError: If the MAC address is not valid
+        """
+        self.is_connected = False
+        self.debug = debug
+        self.debug_to_console = debug_console
+        if self.debug:
+            self.configure_logger()
+
+        if address is not None:
+            if self.check_ble_address(address):
+                self.guardian_ble = GuardianBLE(address, debug=self.debug)
+                self.address = address
+        else:
+            logging.info("No BLE address provided, will search for device...")
+            print("No BLE address provided, will search for device..")
+            self.guardian_ble = GuardianBLE(debug=self.debug)
+
+        self.guardian_api = GuardianAPI(debug=self.debug)
+
+    def configure_logger(self):
+        """Configure the logger for the Guardian Client"""
+        if not os.path.exists("./logs"):
+            os.makedirs("logs")
+
+        datestr = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
+        log_filename = f"./logs/ble_info-{datestr}.log"
+
+        if not os.path.exists(os.path.dirname(log_filename)):
+            os.makedirs(os.path.dirname(log_filename))
+        log_handlers = [logging.FileHandler(log_filename)]
+
+        if self.debug_to_console:
+            log_handlers.append(logging.StreamHandler())
+
+        logging.basicConfig(
+            level=logging.INFO,
+            datefmt="%d-%b-%y %H:%M:%S",
+            format="%(asctime)s: %(name)s - %(levelname)s - %(message)s",
+            handlers=log_handlers,
+        )
+
+    def check_ble_address(self, address: str) -> bool:
+        """Check if the BLE address is valid
+
+        Args:
+            address (str): The MAC address of the Guardian Earbuds
+
+        Returns:
+            bool: True if the address is valid, False otherwise
+        """
+        if (
+            check_platform() == "Windows"
+            or check_platform() == "Linux"
+            and check_valid_mac(address)
+        ):
+            return True
+        elif check_platform() == "Darwin" and check_valid_uuid(address):
+            logging.info("Platform detected: Darwin")
+            # print(f"UUID is valid for system Darwin: {address}")
+            return True
+        else:
+            logging.error("Invalid BLE address")
+            raise ValueError("Invalid BLE address")
+
+    async def search_device(self):
+        """Connect to the Guardian Earbuds
+
+        Returns:
+            is_connected: bool
+        """
+
+        self.address = await self.guardian_ble.search_device()
+
+        return self.address
+
+    async def get_device_address(self) -> str:
+        """Get the MAC address of the Guardian Earbuds.
+        It searches the MAC address of the device automatically. This
+        address is used as the deviceID for cloud communication
+        """
+        device_address = await self.guardian_ble.get_device_mac()
+        return device_address
+
+    async def start_recording(
+        self,
+        recording_timer: int = 36000,
+        led_sleep: bool = False,
+        experiment: str = "None provided",
+        impedance_measurement: bool = False,
+        mains_freq_60hz: bool = False,
+        sending_timout: float = 2,
+        bi_directional_receiving_timeout: float = 5,
+    ):
+        """
+        Start recording data from the Guardian Earbuds.
+        Unidirectional websocket connection to the Guardian Cloud API.
+
+        Args:
+            recording_timer (int, optional): The duration of the recording in seconds. Defaults to 36000.
+            led_sleep (bool, optional): Enable LED sleep mode. Defaults to False.
+            experiment (str, optional): The name of the experiment. Defaults to "None provided". This will
+                                        go to the log file.
+            impedance_measurement (bool, optional): Enable impedance measurement. Defaults to False.
+            mains_freq_60hz (bool, optional): Set to True if the mains frequency is 60Hz. Defaults to False.
+            sending_timout (float): The timeout in seconds for sending data to the cloud. Defaults to 1.
+                                    If no data is sent for a second the sending is interupted and the data
+                                    is buffered. If you have a fast internet and you do not want to lose any data,
+                                    then make 0.5 seconds. If you have slow internet and are fine with losing some data,
+                                    then make 5 seconds. The seconds will be the amount lost before noticing internet loss.
+            bi_directional_receiving_timeout (float): The timeout in seconds for receiving data from the cloud. Defaults to 4.
+                                                      If no data is received for 5 seconds the receiving is interupted and the data
+                                                      the connection will be re-established. If you have a fast internet and you do not want to lose
+                                                      bi-directional data, then make 5 seconds. If you have slow internet and are fine with losing some data,
+                                                      then make 10 seconds. The seconds will be the amount lost before noticing internet loss.
+
+
+        Raises:
+            ValueError: If the recording timer is not valid
+        """
+        # set the timers
+        self.guardian_api.runtime_receipt_timeout = sending_timout
+        self.guardian_api.runtime_bi_directional_timeout = (
+            bi_directional_receiving_timeout
+        )
+
+        if self.debug:
+            logging.info(
+                "[CLIENT]: Recording timer set to: %s seconds", recording_timer
+            )
+            logging.info("[CLIENT]: Start recording")
+
+        print(f"[CLIENT]: Recording timer set to: {recording_timer} seconds")
+        print("-----Recording starting------")
+
+        data_queue: asyncio.Queue = asyncio.Queue(maxsize=86400)
+
+        recording_id = "py-" + str(
+            uuid.uuid4()
+        )  # the recordingID is a unique ID for each recording
+        logging.info("[CLIENT] Recording ID: %s", recording_id)
+        # log the experiment name in bold using the logging module
+        logging.info("[CLIENT] Experiment description: %s", experiment)
+        mac_id = await self.guardian_ble.get_device_mac()
+
+        tasks = []
+        tasks.append(
+            self.guardian_ble.run_ble_record(
+                data_queue,
+                recording_timer,
+                mac_id,
+                led_sleep,
+                impedance_measurement,
+                mains_freq_60hz,
+            )
+        )
+        tasks.append(
+            self.guardian_api.connect_ws_api(
+                data_queue, mac_id, recording_id, impedance_measurement
+            )
+        )
+
+        await asyncio.wait(tasks)
+        if self.debug:
+            logging.info("[CLIENT]: -----------  All tasks are COMPLETED -----------")
+        print(f"-----Recording ID {recording_id}------")
+        print(f"-----Device ID {mac_id}------")
+        print("-----Recording stopped------")
+
+    def stop_recording(self):
+        """Stop recording data from the Guardian Earbuds"""
+
+    async def start_battery(self):
+        """
+        Start recording data from the Guardian Earbuds.
+        Unidirectional websocket connection to the Guardian Cloud API.
+        """
+        print("-----Battery readout started------")
+        if self.debug:
+            logging.info("[CLIENT]: Start recording")
+
+        ble_client_task = self.guardian_ble.read_battery_level()
+        await asyncio.wait([ble_client_task])
+
+        if self.debug:
+            logging.info("[CLIENT]: Disconnect BLE and close websocket connection")
+        print("-----Battery check stopped------")
```

### Comparing `idun_guardian_client-1.1b4/src/idun_guardian_client/config.py` & `idun_guardian_client-1.1b9/src/idun_guardian_client/config.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from pydantic import BaseSettings
-
-
-class Settings(BaseSettings):
-    """
-    Microservice settings. They can be set as environment variables.
-    """
-
-    # GDK 2.0 BLE characteristic
-    STARTBYTE: str = "0xF0"
-    ENDBYTE: str = "0x0F"
-    DEVICE_ID: str = "703DF80E-F543-1947-C0AD-2178ACACAFC7"
-    UUID_MEAS_EEGIMU: str = "beffd56c-c915-48f5-930d-4c1feee0fcc4"
-    UUID_MEAS_EEG: str = "beffd56c-c915-48f5-930d-4c1feee0fcc5"
-    UUID_MEAS_IMP: str = "beffd56c-c915-48f5-930d-4c1feee0fcc8"
-    UUID_DEVICE_SERVICE: str = "0000180a-0000-1000-8000-00805f9b34fb"
-    UUID_MAC_ID: str = "00002a25-0000-1000-8000-00805f9b34fb"
-    UUID_FIRMWARE_VERSION: str = "00002a26-0000-1000-8000-00805f9b34fb"
-    UUID_BATTERY_ID: str = "00002a19-0000-1000-8000-00805f9b34fb"
-    UUID_CFG: str = "beffd56c-c915-48f5-930d-4c1feee0fcc9"
-    UUID_CMD: str = "beffd56c-c915-48f5-930d-4c1feee0fcca"
-    LED_ON_CFG: str = "d1"
-    LED_OFF_CFG: str = "d0"
-    NOTCH_FREQ_50_CFG: str = "n0"
-    NOTCH_FREQ_60_CFG: str = "n1"
-    START_CMD: str = "M"  #'\x62' #b -> start measurement
-    STOP_CMD: str = "S"  # '\x73' #s -> stop measurement
-    START_IMP_CMD: str = "Z"  # '\x7a' #z -> start impedance
-    STOP_IMP_CMD: str = "X"  # '\x78' #x -> stop impedance
-
-    CONNECTION_TIME = 60
-    # GDK 1.0 BLE characteristic
-    # DEVICE_ID=9649E20B-C6BF-DC4B-5D79-FB7BF216F2EC
-    UUID_MEAS_GDK: str = "1becaf24-9719-47c3-8fdc-d1d2beadd4cb"
-    # UUID_CMD_GDK=1becaf24-9719-47c3-8fdc-d1d2beadd4cc
-    UUID_BATT_GDK: str = "00002a19-0000-1000-8000-00805f9b34fb"
-
-    # Websocket Connection API Gateway
-    WS_IDENTIFIER: str = "wss://wpcg36nil5.execute-api.eu-central-1.amazonaws.com/v1/"
-    # REST API Gateway
-    REST_API_LOGIN: str = "https://d3pq71txhb.execute-api.eu-central-1.amazonaws.com/"
-
-
-settings = Settings()
+from pydantic import BaseSettings
+
+
+class Settings(BaseSettings):
+    """
+    Microservice settings. They can be set as environment variables.
+    """
+
+    # GDK 2.0 BLE characteristic
+    STARTBYTE: str = "0xF0"
+    ENDBYTE: str = "0x0F"
+    DEVICE_ID: str = "703DF80E-F543-1947-C0AD-2178ACACAFC7"
+    UUID_MEAS_EEGIMU: str = "beffd56c-c915-48f5-930d-4c1feee0fcc4"
+    UUID_MEAS_EEG: str = "beffd56c-c915-48f5-930d-4c1feee0fcc5"
+    UUID_MEAS_IMP: str = "beffd56c-c915-48f5-930d-4c1feee0fcc8"
+    UUID_DEVICE_SERVICE: str = "0000180a-0000-1000-8000-00805f9b34fb"
+    UUID_MAC_ID: str = "00002a25-0000-1000-8000-00805f9b34fb"
+    UUID_FIRMWARE_VERSION: str = "00002a26-0000-1000-8000-00805f9b34fb"
+    UUID_BATTERY_ID: str = "00002a19-0000-1000-8000-00805f9b34fb"
+    UUID_CFG: str = "beffd56c-c915-48f5-930d-4c1feee0fcc9"
+    UUID_CMD: str = "beffd56c-c915-48f5-930d-4c1feee0fcca"
+    LED_ON_CFG: str = "d1"
+    LED_OFF_CFG: str = "d0"
+    NOTCH_FREQ_50_CFG: str = "n0"
+    NOTCH_FREQ_60_CFG: str = "n1"
+    START_CMD: str = "M"  #'\x62' #b -> start measurement
+    STOP_CMD: str = "S"  # '\x73' #s -> stop measurement
+    START_IMP_CMD: str = "Z"  # '\x7a' #z -> start impedance
+    STOP_IMP_CMD: str = "X"  # '\x78' #x -> stop impedance
+
+    CONNECTION_TIME = 60
+    # GDK 1.0 BLE characteristic
+    # DEVICE_ID=9649E20B-C6BF-DC4B-5D79-FB7BF216F2EC
+    UUID_MEAS_GDK: str = "1becaf24-9719-47c3-8fdc-d1d2beadd4cb"
+    # UUID_CMD_GDK=1becaf24-9719-47c3-8fdc-d1d2beadd4cc
+    UUID_BATT_GDK: str = "00002a19-0000-1000-8000-00805f9b34fb"
+
+    # Websocket Connection API Gateway
+    WS_IDENTIFIER: str = "wss://wpcg36nil5.execute-api.eu-central-1.amazonaws.com/v1/"
+    # REST API Gateway
+    REST_API_LOGIN: str = "https://d3pq71txhb.execute-api.eu-central-1.amazonaws.com/"
+
+
+settings = Settings()
```

### Comparing `idun_guardian_client-1.1b4/src/idun_guardian_client/debug_logs.py` & `idun_guardian_client-1.1b9/src/idun_guardian_client/debug_logs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,425 +1,424 @@
-"""
-This module contains the functions that are used to log the debug messages.
-"""
-import logging
-import time
-
-
-def log_first_message(data_model, package_receipt, debug):
-    if debug:
-        logging.info("[API]: First package sent")
-        logging.info(
-            "[API]: data_model.stop = %s",
-            data_model.stop,
-        )
-        logging.info(
-            "[API]: data_model.deviceID = %s",
-            data_model.deviceID,
-        )
-        logging.info(
-            "[API]: data_model.recordingID = %s",
-            data_model.recordingID,
-        )
-        logging.info(
-            "[API]: First package receipt: %s",
-            package_receipt,
-        )
-
-
-def log_final_message(data_model, package_receipt, debug):
-    if debug:
-        logging.info("[API]: Last package sent")
-        logging.info(
-            "[API]: data_model.stop = %s",
-            data_model.stop,
-        )
-        logging.info(
-            "[API]: data_model.deviceID = %s",
-            data_model.deviceID,
-        )
-        logging.info(
-            "[API]: data_model.recordingID = %s",
-            data_model.recordingID,
-        )
-        logging.info(
-            "[API]: Last package receipt: %s",
-            package_receipt,
-        )
-        logging.info("[API]: Cloud connection sucesfully terminated")
-        logging.info("[API]: Breaking inner loop of API client")
-
-
-def logging_connection(websocket_resource_url, debug):
-    if debug:
-        logging.info(
-            "[API]: Connected to websocket resource url: %s",
-            websocket_resource_url,
-        )
-        logging.info("[API]: Sending data to the cloud")
-
-
-def logging_break(debug):
-    if debug:
-        logging.info("[API]: Breaking API client while loop")
-
-
-def logging_ping_error(error, retry_time, debug):
-    if debug:
-        logging.info("[API]: Ping interuption: %s", error)
-        logging.info("[API]: Ping failed, connection closed")
-        logging.info(
-            "[API]: Trying to reconnect in %s seconds",
-            retry_time,
-        )
-
-
-def logging_not_empty(debug: bool) -> None:
-    """Log the queue is not empty."""
-    if debug:
-        logging.info("[API]: Data queue is not empty, waiting for last timestamp")
-
-
-def log_interrupt_error(error, debug):
-    if debug:
-        logging.info(
-            "[API]: Interuption in sending or receiving data to the cloud: %s",
-            error,
-        )
-
-
-def log_error_in_sending_stop(error, debug):
-    if debug:
-        logging.info(
-            "[API]: Error in sending stop signal to the cloud: %s",
-            error,
-        )
-
-
-def log_error_in_sending_stop_ble(error, debug):
-    if debug:
-        logging.info(
-            "[BLE]: Error in loading stop signal to the cloud: %s",
-            error,
-        )
-
-
-def logging_connection_closed(debug):
-    if debug:
-        logging.info("[API]: Websocket client connection closed")
-
-
-def logging_reconnection(debug):
-    if debug:
-        logging.info("[API]: Ping successful, connection alive and continue..")
-        logging.info("Try to ping websocket successful")
-
-
-def logging_empty(debug):
-    if debug:
-        logging.info("[API]: Device queue is empty, sending computer time")
-
-
-def logging_cloud_termination(debug):
-    if debug:
-        logging.info("[API]: Terminating cloud connection")
-
-
-def logging_gaieerror(error, retry_time, debug):
-    if debug:
-        logging.info("[API]: Interruption in connecting to the cloud: %s", error)
-        logging.info("[API]: Retrying connection in %s sec ", retry_time)
-
-
-def logging_connection_refused(error, retry_time, debug):
-    if debug:
-        logging.info("[API]: Interruption in connecting to the cloud: %s", error)
-        logging.info(
-            "Cannot connect to API endpoint. Please check the URL and try again."
-        )
-        logging.info("Retrying connection in {} seconds".format(retry_time))
-
-
-def logging_cancelled_error(error, debug):
-    if debug:
-        logging.info(
-            "[API]: Error in sending data to the cloud: %s",
-            error,
-        )
-        logging.info("[API]: Re-establishing cloud connection in exeption")
-        logging.info("[API]: Fetching last package from queue")
-
-
-def logging_connecting_to_cloud(debug):
-    if debug:
-        logging.info("[API]: Connecting to cloud...")
-
-
-def logging_waiting_for_stop_receipt(debug):
-    if debug:
-        logging.info("[API]: Waiting for stop receipt")
-
-
-def logging_api_completed(debug):
-    if debug:
-        logging.info("[API]: -----------  API client is COMPLETED ----------- ")
-
-
-def logging_succesfull_stop(debug):
-    if debug:
-        logging.info("[BLE]: Recording successfully stopped")
-
-
-def logging_searching(debug):
-    if debug:
-        logging.info("[BLE]: Searching for MAC address")
-
-
-def logging_device_info(debug, mac_address, firmware_decoded):
-    if debug:
-        logging.info("[BLE] Device ID (based on MAC address is): %s", mac_address)
-        logging.info("[BLE]: Firmware version: %s", firmware_decoded)
-
-
-def logging_device_not_found(debug):
-    if debug:
-        logging.info("[BLE]: No IGEB device found, exiting ..")
-
-
-def logging_device_found(debug, ble_device_list):
-    if debug:
-        logging.info(
-            "[BLE]: One IGEB device found, assinging address %s", ble_device_list[0]
-        )
-
-
-def logging_device_address(debug, device_address):
-    if debug:
-        logging.info("[BLE]: Received address as %s", device_address)
-
-
-def logging_trying_to_connect(debug, device_address):
-    if debug:
-        logging.info("[BLE]: Trying to connect to %s.....", device_address)
-
-
-def logging_connected(debug, device_address):
-    if debug:
-        logging.info("[BLE]: Connected to %s", device_address)
-
-
-def logging_disconnected_recognised(debug):
-    if debug:
-        logging.info("[BLE]: Callback function recognised a disconnection.")
-
-
-def logging_batterylevel(debug, battery_level):
-    if debug:
-        logging.info(
-            "[BLE]: Battery level: %d%%",
-            int.from_bytes(battery_level, byteorder="little"),
-        )
-
-
-def logging_sending_start(debug):
-    if debug:
-        logging.info("[BLE]: Sending start commands")
-
-
-def logging_subscribing_eeg_notification(debug):
-    if debug:
-        logging.info("[BLE]: Subscribing EEG notification")
-
-
-def logging_subscribing_battery_notification(debug):
-    if debug:
-        logging.info("[BLE]: Subscribing battery notification")
-
-
-def logging_sending_stop(debug):
-    if debug:
-        logging.info("[BLE]: Stop command loaded into queue")
-
-
-def logging_giving_time_api(debug):
-    if debug:
-        logging.info("[BLE]: Giving time to API client to send data")
-
-
-def logging_sending_stop_device(debug):
-    if debug:
-        logging.info("[BLE]: Sending stop command to device")
-
-
-def logging_sending_disconnect(debug):
-    if debug:
-        logging.info("[BLE]: Sending disconnect command to device")
-
-
-def logging_turn_ble_on(debug):
-    if debug:
-        logging.info("[BLE]: Turning BLE on")
-
-
-def logging_turn_led_on(debug):
-    if debug:
-        logging.info("[BLE]: Turning LED on")
-
-
-def logging_recording_successfully_stopped(debug):
-    if debug:
-        logging.info("[BLE]: Recording successfully stopped")
-
-
-def logging_keyboard_interrupt(debug):
-    if debug:
-        logging.info("[BLE]: KeyboardInterrupt applied, terminating...")
-        logging.info(
-            "[BLE]: Sending stop signal to device and cloud, please wait a moment ..."
-        )
-
-
-def logging_stop_send(debug):
-    if debug:
-        logging.info(
-            "[API]: Sending stop signal to device and cloud, please wait a moment ..."
-        )
-
-
-def logging_device_lost_give_up(debug):
-    if debug:
-        logging.info("[BLE]: Device lost, terminating...")
-
-
-def logging_trying_to_connect_again(debug, try_to_connect_timeout):
-    if debug:
-        logging.warning(
-            " [BLE] Connection lost, will try to reconnect %s more times",
-            try_to_connect_timeout,
-        )
-
-
-def logging_device_connected_general(debug):
-    if debug:
-        logging.info("[BLE]: Device connected")
-
-
-def logging_recording_started(debug):
-    if debug:
-        logging.info("[BLE]: Recording successfully started")
-
-
-def logging_time_reached(debug, original_time):
-    if debug:
-        logging.info(
-            "[BLE]: Recording stopped, time reached : %s",
-            round(time.time() - original_time, 2),
-        )
-
-
-def logging_timeout_reached(debug):
-    if debug:
-        logging.info("[BLE]: Time out reached")
-
-
-def logging_ble_client_lost(debug, error):
-    if debug:
-        logging.error("[BLE]: Error in bluetooth client: %s", error)
-
-
-def logging_ensuring_ble_disconnected(debug):
-    if debug:
-        logging.info("[BLE]: Ensuring device is disconnected")
-
-
-def logging_device_info_uuid(debug, service):
-    if debug:
-        logging.info("[Service] %s: %s", service.uuid, service.description)
-
-
-def logging_device_info_characteristic(debug, char, value):
-    if debug:
-        logging.info(
-            "\t[Characteristic] %s: (Handle: %s) (%s) \
-                | Name: %s, Value: %s ",
-            char.uuid,
-            char.handle,
-            ",".join(char.properties),
-            char.description,
-            value,
-        )
-
-
-def logging_device_description_list(debug, char, value):
-    if debug:
-        logging.info("%s : %s", char.description, str(value))
-
-
-def logging_device_connection_failed(debug, err):
-    if debug:
-        logging.error("[BLE]: Device connection failed - %s", err)
-
-
-def logging_reading_battery_level(debug):
-    if debug:
-        logging.info("[BLE]: Reading battery level")
-
-
-def logging_getting_impedance(debug, impedance_display_time):
-    if debug:
-        logging.info("[BLE]: Getting impedance measurement")
-        logging.info(
-            "[BLE]: Impedance display time: %s seconds", impedance_display_time
-        )
-
-
-def logging_starting_impedance_measurement(debug):
-    if debug:
-        logging.info("[BLE]: Starting impedance measurement")
-
-
-def logging_subscribing_impedance_notification(debug):
-    if debug:
-        logging.info("[BLE]: Subscribing impedance measurement")
-
-
-# create logging functions for start impedance command, displaying impedance and stop impedance command
-def logging_starting_impedance_measurement_commands(debug):
-    if debug:
-        logging.info("[BLE]: Sending start impedance commands")
-
-
-def logging_displaying_impedance(debug):
-    if debug:
-        logging.info("[BLE]: Displaying impedance measurement")
-
-
-def logging_stopping_impedance_measurement(debug):
-    if debug:
-        logging.info("[BLE]: Stopping impedance measurement")
-
-
-def logging_ble_complete(debug):
-    if debug:
-        logging.info("[BLE]: -----------  BLE client is COMPLETED ----------- ")
-
-
-def loggig_ble_init(debug):
-    if debug:
-        logging.info("[BLE]: BLE client initiliazed")
-
-
-def logging_batterylevel_int(debug, value):
-    if debug:
-        logging.info("Battery level: %s%%", value)
-
-
-def logging_cloud_not_receiving(debug, credit_reimbursement):
-    # This wifi connection works with a credit system. If a receipt is found, then the credits are replenished.
-    # with one credit per package in the receipt. For each message without a receipt, the credits are reduced by one.
-    # If the credits are reduced to zero, the package that is sent is the fake data package until a receipt is received.
-    # In which case the credits are replenished and the real data is sent.
-    if debug:
-        logging.warning("Data is not being received by cloud")
-        logging.warning(
-            f"Resending last package again in {credit_reimbursement} seconds"
-        )
+"""
+This module contains the functions that are used to log the debug messages.
+"""
+import logging
+import time
+
+
+def log_first_message(data_model, package_receipt, debug):
+    if debug:
+        logging.info("[API]: First package sent")
+        logging.info(
+            "[API]: data_model.stop = %s",
+            data_model.stop,
+        )
+        logging.info(
+            "[API]: data_model.deviceID = %s",
+            data_model.deviceID,
+        )
+        logging.info(
+            "[API]: data_model.recordingID = %s",
+            data_model.recordingID,
+        )
+        logging.info(
+            "[API]: First package receipt: %s",
+            package_receipt,
+        )
+
+
+def log_final_message(data_model, package_receipt, debug):
+    if debug:
+        logging.info("[API]: Last package sent")
+        logging.info(
+            "[API]: data_model.stop = %s",
+            data_model.stop,
+        )
+        logging.info(
+            "[API]: data_model.deviceID = %s",
+            data_model.deviceID,
+        )
+        logging.info(
+            "[API]: data_model.recordingID = %s",
+            data_model.recordingID,
+        )
+        logging.info(
+            "[API]: Last package receipt: %s",
+            package_receipt,
+        )
+        logging.info("[API]: Cloud connection sucesfully terminated")
+        logging.info("[API]: Breaking inner loop of API client")
+
+
+def logging_connection(websocket_resource_url, debug):
+    if debug:
+        logging.info(
+            "[API]: Connected to websocket resource url: %s",
+            websocket_resource_url,
+        )
+        logging.info("[API]: Sending data to the cloud")
+
+
+def logging_break(debug):
+    if debug:
+        logging.info("[API]: Breaking API client while loop")
+
+
+def logging_ping_error(error, retry_time, debug):
+    if debug:
+        logging.info("[API]: Ping interuption: %s", error)
+        logging.info("[API]: Ping failed, connection closed")
+        logging.info(
+            "[API]: Trying to reconnect in %s seconds",
+            retry_time,
+        )
+
+
+def logging_not_empty(debug: bool) -> None:
+    """Log the queue is not empty."""
+    if debug:
+        logging.info("[API]: Data queue is not empty, waiting for last timestamp")
+
+
+def log_interrupt_error(error, debug):
+    if debug:
+        logging.info(
+            "[API]: Interuption in sending or receiving data to the cloud: %s",
+            error,
+        )
+
+
+def log_error_in_sending_stop(error, debug):
+    if debug:
+        logging.info(
+            "[API]: Error in sending stop signal to the cloud: %s",
+            error,
+        )
+
+
+def log_error_in_sending_stop_ble(error, debug):
+    if debug:
+        logging.info(
+            "[BLE]: Error in loading stop signal to the cloud: %s",
+            error,
+        )
+
+
+def logging_connection_closed(debug):
+    if debug:
+        logging.info("[API]: Websocket client connection closed")
+
+
+def logging_reconnection(debug):
+    if debug:
+        logging.info("[API]: Ping successful, connection alive and continue..")
+        logging.info("Try to ping websocket successful")
+
+
+def logging_empty(debug):
+    if debug:
+        logging.info("[API]: Device queue is empty, sending computer time")
+
+
+def logging_cloud_termination(debug):
+    if debug:
+        logging.info("[API]: Terminating cloud connection")
+
+
+def logging_gaieerror(error, retry_time, debug):
+    if debug:
+        logging.info("[API]: Interruption in connecting to the cloud: %s", error)
+        logging.info("[API]: Retrying connection in %s sec ", retry_time)
+
+
+def logging_connection_refused(error, retry_time, debug):
+    if debug:
+        logging.info("[API]: Interruption in connecting to the cloud: %s", error)
+        logging.info(
+            "Cannot connect to API endpoint. Please check the URL and try again."
+        )
+        logging.info("Retrying connection in {} seconds".format(retry_time))
+
+
+def logging_cancelled_error(debug):
+    if debug:
+        logging.info(
+            "[API]: Error in sending data to the cloud: %s"
+        )
+        logging.info("[API]: Re-establishing cloud connection in exeption")
+        logging.info("[API]: Fetching last package from queue")
+
+
+def logging_connecting_to_cloud(debug):
+    if debug:
+        logging.info("[API]: Connecting to cloud...")
+
+
+def logging_waiting_for_stop_receipt(debug):
+    if debug:
+        logging.info("[API]: Waiting for stop receipt")
+
+
+def logging_api_completed(debug):
+    if debug:
+        logging.info("[API]: -----------  API client is COMPLETED ----------- ")
+
+
+def logging_succesfull_stop(debug):
+    if debug:
+        logging.info("[BLE]: Recording successfully stopped")
+
+
+def logging_searching(debug):
+    if debug:
+        logging.info("[BLE]: Searching for MAC address")
+
+
+def logging_device_info(debug, mac_address, firmware_decoded):
+    if debug:
+        logging.info("[BLE] Device ID (based on MAC address is): %s", mac_address)
+        logging.info("[BLE]: Firmware version: %s", firmware_decoded)
+
+
+def logging_device_not_found(debug, break_time):
+    if debug:
+        logging.info(f"[BLE]: No IGEB device found, trying again in {break_time} seconds")
+
+
+def logging_device_found(debug, ble_device_list):
+    if debug:
+        logging.info(
+            "[BLE]: One IGEB device found, assinging address %s", ble_device_list[0]
+        )
+
+
+def logging_device_address(debug, device_address):
+    if debug:
+        logging.info("[BLE]: Received address as %s", device_address)
+
+
+def logging_trying_to_connect(debug, device_address):
+    if debug:
+        logging.info("[BLE]: Trying to connect to %s.....", device_address)
+
+
+def logging_connected(debug, device_address):
+    if debug:
+        logging.info("[BLE]: Connected to %s", device_address)
+
+
+def logging_disconnected_recognised(debug):
+    if debug:
+        logging.info("[BLE]: Callback function recognised a disconnection.")
+
+
+def logging_batterylevel(debug, battery_level):
+    if debug:
+        logging.info(
+            "[BLE]: Battery level: %d%%",
+            int.from_bytes(battery_level, byteorder="little"),
+        )
+
+
+def logging_sending_start(debug):
+    if debug:
+        logging.info("[BLE]: Sending start commands")
+
+
+def logging_subscribing_eeg_notification(debug):
+    if debug:
+        logging.info("[BLE]: Subscribing EEG notification")
+
+
+def logging_subscribing_battery_notification(debug):
+    if debug:
+        logging.info("[BLE]: Subscribing battery notification")
+
+
+def logging_sending_stop(debug):
+    if debug:
+        logging.info("[BLE]: Stop command loaded into queue")
+
+
+def logging_giving_time_api(debug):
+    if debug:
+        logging.info("[BLE]: Giving time to API client to send data")
+
+
+def logging_sending_stop_device(debug):
+    if debug:
+        logging.info("[BLE]: Sending stop command to device")
+
+
+def logging_sending_disconnect(debug):
+    if debug:
+        logging.info("[BLE]: Sending disconnect command to device")
+
+
+def logging_turn_ble_on(debug):
+    if debug:
+        logging.info("[BLE]: Turning BLE on")
+
+
+def logging_turn_led_on(debug):
+    if debug:
+        logging.info("[BLE]: Turning LED on")
+
+
+def logging_recording_successfully_stopped(debug):
+    if debug:
+        logging.info("[BLE]: Recording successfully stopped")
+
+
+def logging_keyboard_interrupt(debug):
+    if debug:
+        logging.info("[BLE]: KeyboardInterrupt applied, terminating...")
+        logging.info(
+            "[BLE]: Sending stop signal to device and cloud, please wait a moment ..."
+        )
+
+
+def logging_stop_send(debug):
+    if debug:
+        logging.info(
+            "[API]: Sending stop signal to device and cloud, please wait a moment ..."
+        )
+
+
+def logging_device_lost_give_up(debug):
+    if debug:
+        logging.info("[BLE]: Device lost, terminating...")
+
+
+def logging_trying_to_connect_again(debug, try_to_connect_timeout):
+    if debug:
+        logging.warning(
+            " [BLE] Connection lost, will try to reconnect %s more times",
+            try_to_connect_timeout,
+        )
+
+
+def logging_device_connected_general(debug):
+    if debug:
+        logging.info("[BLE]: Device connected")
+
+
+def logging_recording_started(debug):
+    if debug:
+        logging.info("[BLE]: Recording successfully started")
+
+
+def logging_time_reached(debug, original_time):
+    if debug:
+        logging.info(
+            "[BLE]: Recording stopped, time reached : %s",
+            round(time.time() - original_time, 2),
+        )
+
+
+def logging_timeout_reached(debug):
+    if debug:
+        logging.info("[BLE]: Time out reached")
+
+
+def logging_ble_client_lost(debug, error):
+    if debug:
+        logging.error("[BLE]: Error in bluetooth client: %s", error)
+
+
+def logging_ensuring_ble_disconnected(debug):
+    if debug:
+        logging.info("[BLE]: Ensuring device is disconnected")
+
+
+def logging_device_info_uuid(debug, service):
+    if debug:
+        logging.info("[Service] %s: %s", service.uuid, service.description)
+
+
+def logging_device_info_characteristic(debug, char, value):
+    if debug:
+        logging.info(
+            "\t[Characteristic] %s: (Handle: %s) (%s) \
+                | Name: %s, Value: %s ",
+            char.uuid,
+            char.handle,
+            ",".join(char.properties),
+            char.description,
+            value,
+        )
+
+
+def logging_device_description_list(debug, char, value):
+    if debug:
+        logging.info("%s : %s", char.description, str(value))
+
+
+def logging_device_connection_failed(debug, err):
+    if debug:
+        logging.error("[BLE]: Device connection failed - %s", err)
+
+
+def logging_reading_battery_level(debug):
+    if debug:
+        logging.info("[BLE]: Reading battery level")
+
+
+def logging_getting_impedance(debug, impedance_display_time):
+    if debug:
+        logging.info("[BLE]: Getting impedance measurement")
+        logging.info(
+            "[BLE]: Impedance display time: %s seconds", impedance_display_time
+        )
+
+
+def logging_starting_impedance_measurement(debug):
+    if debug:
+        logging.info("[BLE]: Starting impedance measurement")
+
+
+def logging_subscribing_impedance_notification(debug):
+    if debug:
+        logging.info("[BLE]: Subscribing impedance measurement")
+
+
+# create logging functions for start impedance command, displaying impedance and stop impedance command
+def logging_starting_impedance_measurement_commands(debug):
+    if debug:
+        logging.info("[BLE]: Sending start impedance commands")
+
+
+def logging_displaying_impedance(debug):
+    if debug:
+        logging.info("[BLE]: Displaying impedance measurement")
+
+
+def logging_stopping_impedance_measurement(debug):
+    if debug:
+        logging.info("[BLE]: Stopping impedance measurement")
+
+
+def logging_ble_complete(debug):
+    if debug:
+        logging.info("[BLE]: -----------  BLE client is COMPLETED ----------- ")
+
+
+def loggig_ble_init(debug):
+    if debug:
+        logging.info("[BLE]: BLE client initiliazed")
+
+
+def logging_batterylevel_int(debug, value):
+    if debug:
+        logging.info("Battery level: %s%%", value)
+
+
+def logging_cloud_not_receiving(debug, credit_reimbursement):
+    # This wifi connection works with a credit system. If a receipt is found, then the credits are replenished.
+    # with one credit per package in the receipt. For each message without a receipt, the credits are reduced by one.
+    # If the credits are reduced to zero, the package that is sent is the fake data package until a receipt is received.
+    # In which case the credits are replenished and the real data is sent.
+    if debug:
+        logging.warning("Data is not being received by cloud")
+        logging.warning(
+            f"Resending last package again in {credit_reimbursement} seconds"
+        )
```

### Comparing `idun_guardian_client-1.1b4/src/idun_guardian_client/igeb_api.py` & `idun_guardian_client-1.1b9/src/idun_guardian_client/igeb_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,516 +1,516 @@
-"""
-Guardian API websocket utilities.
-"""
-import os
-import json
-from dataclasses import dataclass, asdict
-import socket
-import datetime
-import asyncio
-from typing import Union
-import requests
-import websockets
-import time
-from typing import Optional
-from dotenv import load_dotenv
-
-from .config import settings
-from .igeb_utils import unpack_from_queue
-from .mock_utils import mock_cloud_package
-from .debug_logs import *
-
-
-load_dotenv()
-
-FILTER_PACKAGE = "bp_filter_eeg"
-PACKAGE_RECEIPT = "SequenceNumber"
-
-
-class GuardianAPI:
-    """Main Guardian API client."""
-
-    def __init__(self, debug: bool = True) -> None:
-        """Initialize Guardian API client.
-
-        Args:
-            debug (bool, optional): Enable debug logging. Defaults to True.
-        """
-        self.debug: bool = debug
-        self.ping_timeout: int = 2
-        self.retry_time: int = 2
-        self.base64string_len: int = 236
-        self.first_message_check = True
-        self.final_message_sent = False
-        self.payload_valid = True
-        self.sample_rate = 250
-        self.sentinal = object()
-        self.encrypted_buffer_size = 3750  # 5 minutes => (5 * 60 * 250) / 20 = 3750
-        self.decrypted_buffer_size = 75000  # 5 minutes => (5 * 60 * 250) = 75000
-        self.encrypted_data_queue: asyncio.Queue = asyncio.Queue(
-            maxsize=self.encrypted_buffer_size
-        )
-        self.decrypted_data_queue: asyncio.Queue = asyncio.Queue(
-            maxsize=self.decrypted_buffer_size
-        )
-        self.initial_receipt_timeout = 15
-        self.runtime_receipt_timeout: float = 1  # Increase if slow connection
-        self.current_timeout = self.initial_receipt_timeout
-        self.initial_bi_directional_timeout = 15
-        self.runtime_bi_directional_timeout: float = 5  # Increase if slow connection
-        self.sending_time_limit = 0.01
-        self.bi_directional_timeout = self.initial_bi_directional_timeout
-        self.last_saved_time = time.time()
-        self.connected = False
-        self.data_model = GuardianDataModel(None, None, None, None, None, False)
-        self.websocket: Optional[websockets.WebSocketClientProtocol] = None  # type: ignore
-        self.final_receipt_got = False
-
-    async def connect_ws_api(
-        self,
-        data_queue: asyncio.Queue,
-        device_id: str = "deviceMockID",
-        recording_id: str = "dummy_recID",
-        impedance_measurement: bool = False,
-    ) -> None:
-        """Connect to the Guardian API websocket.
-
-        Args:
-            data_queue (asyncio.Queue): Data queue from the BLE client
-            deviceID (str, optional): Device ID. Defaults to "deviceMockID".
-            recordingID (str, optional): Recording ID. Defaults to "dummy_recID".
-
-        Raises:
-            Exception: If the websocket connection fails
-        """
-
-        def reset_data_model():
-            self.data_model.payload = None
-            self.data_model.impedance = None
-
-        async def pack_encrypted_queue():
-            if not self.encrypted_data_queue.full():
-                await self.encrypted_data_queue.put(
-                    [self.data_model.deviceTimestamp, self.data_model.payload]
-                )
-            else:
-                await self.encrypted_data_queue.get()
-
-        def pack_decrypted_queue(message):
-            if not self.decrypted_data_queue.full():
-                self.decrypted_data_queue.put_nowait(message[FILTER_PACKAGE])
-            else:
-                self.decrypted_data_queue.get_nowait()
-
-        async def unpack_and_load_data():
-            """Get data from the queue and pack it into a dataclass"""
-            data_valid = False
-            reset_data_model()
-            package = await data_queue.get()
-            (
-                device_timestamp,
-                device_id,
-                data,
-                stop,
-                impedance,
-            ) = unpack_from_queue(package)
-
-            if data is not None:
-                if len(data) == self.base64string_len:
-                    self.data_model.payload = data
-                    data_valid = True
-
-            if impedance is not None:
-                if isinstance(impedance, int):
-                    self.data_model.impedance = impedance
-                    data_valid = True
-
-            if device_timestamp is not None:
-                self.data_model.deviceTimestamp = device_timestamp
-
-            if device_id is not None:
-                self.data_model.deviceID = device_id
-
-            if stop is not None:
-                self.data_model.stop = stop
-                if stop is True:
-                    data_valid = True
-
-            return data_valid
-
-        async def create_timestamp(debug):
-            """Create a timestamp for the data"""
-            if data_queue.empty():
-                logging_empty(debug)  # Fetch the current time from the device
-                device_timestamp = datetime.datetime.now().astimezone().isoformat()
-            else:
-                logging_not_empty(debug)
-                package = (
-                    await data_queue.get()
-                )  # Fetch the timestamp from the BLE package
-                (device_timestamp, _, _, _, _) = unpack_from_queue(package)
-            return device_timestamp
-
-        async def unpack_and_load_data_termination():
-            """Get data from the queue and pack it into a dataclass"""
-            logging_cloud_termination(self.debug)
-            self.data_model.payload = "STOP_CANCELLED"
-            self.data_model.stop = True
-            device_timestamp = await create_timestamp(self.debug)
-            if device_timestamp is not None:
-                self.data_model.deviceTimestamp = device_timestamp
-
-        async def send_messages():
-            while True:
-
-                if not self.connected:
-                    break
-
-                if await unpack_and_load_data():
-                    await asyncio.shield(
-                        asyncio.sleep(self.sending_time_limit)
-                    )  # Wait as to not overload the cloud
-                    await asyncio.shield(
-                        self.websocket.send(json.dumps(asdict(self.data_model)))
-                    )
-                    await asyncio.shield(pack_encrypted_queue())
-
-                if self.data_model.stop:
-                    logging_stop_send(self.debug)
-                    self.current_timeout = (
-                        1000  # Wait until necessary for the stop to be sent
-                    )
-                    self.final_message_sent = True
-                    while not self.final_receipt_got:
-                        # It will loop in here and not update the
-                        # data until the stop is sent
-                        logging_waiting_for_stop_receipt(self.debug)
-                        await asyncio.sleep(1)
-                    break
-
-        async def receive_messages():
-            self.last_saved_time = time.time()
-            while True:
-
-                if not self.connected:
-                    break
-
-                message_str = await asyncio.shield(
-                    asyncio.wait_for(
-                        self.websocket.recv(), timeout=self.current_timeout
-                    )
-                )
-
-                if FILTER_PACKAGE in message_str:
-                    self.bi_directional_timeout = self.runtime_bi_directional_timeout
-                    message = json.loads(message_str)
-                    self.last_saved_time = time.time()
-                    pack_decrypted_queue(message)
-
-                elif PACKAGE_RECEIPT in message_str:
-                    self.current_timeout = self.runtime_receipt_timeout
-                    if self.first_message_check:
-                        self.first_message_check = False
-                        log_first_message(
-                            self.data_model,
-                            message_str,
-                            self.debug,
-                        )
-                    if self.final_message_sent:
-                        log_final_message(
-                            self.data_model,
-                            message_str,
-                            self.debug,
-                        )
-                        self.final_receipt_got = True
-                        break
-
-                bi_directional_timeout(impedance_measurement)
-
-        def bi_directional_timeout(impedance_measurement):
-            time_without_data = time.time() - self.last_saved_time
-            if (
-                time_without_data > self.bi_directional_timeout
-                and not impedance_measurement
-            ):
-                raise asyncio.TimeoutError
-
-        def once_initialise_variables():
-            # initiate flags
-            self.first_message_check = True
-            self.final_message_sent = False
-            self.data_model = GuardianDataModel(
-                None, device_id, recording_id, None, None, False
-            )
-
-        def on_connection_initialise_variables():
-            self.first_message_check = True
-            self.connected = True
-            self.bi_directional_timeout = self.initial_bi_directional_timeout
-            self.current_timeout = self.initial_receipt_timeout
-
-        async def handle_cancelled_error(error):
-            while True:
-                try:
-                    async with websockets.connect(  # type: ignore
-                        settings.WS_IDENTIFIER
-                    ) as self.websocket:
-                        logging_cancelled_error(error, self.debug)
-                        await unpack_and_load_data_termination()
-                        await self.websocket.send(json.dumps(asdict(self.data_model)))
-                        package_receipt = await self.websocket.recv()
-                        log_final_message(
-                            self.data_model,
-                            package_receipt,
-                            self.debug,
-                        )
-                        self.final_message_sent = True
-                        break
-                except Exception as error:
-                    await asyncio.sleep(self.ping_timeout)
-                    log_error_in_sending_stop(error, self.debug)
-                    continue
-
-        once_initialise_variables()
-
-        while True:
-            logging_connecting_to_cloud(self.debug)
-            try:
-                async with websockets.connect(settings.WS_IDENTIFIER) as self.websocket:  # type: ignore
-                    try:
-                        on_connection_initialise_variables()
-                        # for the websocket we want to increase to initial timeout each time
-                        logging_connection(settings.WS_IDENTIFIER, self.debug)
-                        send_task = asyncio.create_task(send_messages())
-                        receive_task = asyncio.create_task(receive_messages())
-                        await asyncio.gather(send_task, receive_task)
-
-                    except (
-                        websockets.exceptions.ConnectionClosed,  # type: ignore
-                    ) as error:
-                        try:
-                            logging_connection_closed(self.debug)
-                            self.connected = False
-                            await asyncio.shield(asyncio.sleep(self.ping_timeout))
-                            logging_reconnection(self.debug)
-                            self.bi_directional_timeout = (
-                                self.initial_bi_directional_timeout
-                            )
-                            continue
-                        except asyncio.CancelledError as error:
-                            await handle_cancelled_error(error)
-
-                    except (asyncio.TimeoutError) as error:
-                        try:
-                            log_interrupt_error(error, self.debug)
-                            self.connected = False
-                            await asyncio.shield(asyncio.sleep(self.ping_timeout))
-                            logging_reconnection(self.debug)
-                            self.bi_directional_timeout = (
-                                self.initial_bi_directional_timeout
-                            )
-                            continue
-                        except asyncio.CancelledError as error:
-                            await handle_cancelled_error(error)
-
-                    except asyncio.CancelledError as error:
-                        await handle_cancelled_error(error)
-
-                    finally:
-                        # Otherwise new tasks will be created which is a problem
-                        try:
-                            if not send_task.done():
-                                send_task.cancel()
-                            if not receive_task.done():
-                                receive_task.cancel()
-                        except Exception as error:
-                            print("These tasks does not exist yet")
-
-            except socket.gaierror as error:
-                logging_gaieerror(error, self.retry_time, self.debug)
-                await asyncio.sleep(self.retry_time)
-                continue
-
-            except ConnectionRefusedError as error:
-                logging_connection_refused(error, self.retry_time, self.debug)
-                await asyncio.sleep(self.retry_time)
-                continue
-
-            except Exception as error:
-                log_interrupt_error(error, self.debug)
-
-            finally:
-                # Otherwise new tasks will be created which is a problem
-                try:
-                    if not send_task.done():
-                        send_task.cancel()
-                    if not receive_task.done():
-                        receive_task.cancel()
-                except Exception as error:
-                    print("These tasks does not exist yet")
-
-            if self.final_message_sent:
-                logging_break(self.debug)
-                break
-
-        logging_api_completed(self.debug)
-
-    def get_recordings_info_all(
-        self, device_id: str = "mock-device-0", first_to_last=False, password: str = ""
-    ) -> list:
-        recordings_url = f"{settings.REST_API_LOGIN}recordings"
-        if password == "":
-            password = input("\nEnter your new passsword here: ")
-        with requests.Session() as session:
-            result = session.get(recordings_url, auth=(device_id, password))
-            if result.status_code == 200:
-                print("Recording list retrieved successfully")
-                recordings = result.json()
-                recordings.sort(
-                    key=lambda x: datetime.datetime.strptime(
-                        x["startDeviceTimestamp"], "%Y-%m-%dT%H:%M:%S.%fZ"
-                    ),
-                    reverse=first_to_last,
-                )
-                print(json.dumps(recordings, indent=4, sort_keys=True))
-                return result.json()
-            elif result.status_code == 401:
-                print(f"Password for {device_id} is incorrect")
-                return []
-            elif result.status_code == 403:
-                print(
-                    "Wrong device ID, you can find the device ID in",
-                    " the logs in the format XX-XX-XX-XX-XX-XX",
-                )
-                return []
-            elif result.status_code == 412:
-                print(
-                    f"Device {device_id} is not registered",
-                )
-                return []
-            elif result.status_code == 404:
-                print(f"No recording found for device {device_id}")
-                return []
-            elif result.status_code == 502:
-                print(f"Device {device_id} does not exist")
-                return []
-            else:
-                print("Loading recording list failed")
-                return []
-
-    def get_recording_info_by_id(
-        self, device_id: str, recording_id: str = "recordingId-0", password: str = ""
-    ) -> list:
-        recordings_url = f"{settings.REST_API_LOGIN}recordings/{recording_id}"
-
-        if password == "":
-            password = input("\nEnter your new passsword here: ")
-        with requests.Session() as session:
-            result = session.get(recordings_url, auth=(device_id, password))
-            if result.status_code == 200:
-                print("Recording ID file found")
-                print(json.dumps(result.json(), indent=4, sort_keys=True))
-                return result.json()
-            elif result.status_code == 401:
-                print(f"Password for {device_id} is incorrect")
-                return []
-            elif result.status_code == 403:
-                print(
-                    "Wrong device ID, you can find the device ID in",
-                    " the logs in the format XX-XX-XX-XX-XX-XX",
-                )
-                return []
-            elif result.status_code == 412:
-                print(
-                    f"Device {device_id} not registered",
-                )
-                return []
-            elif result.status_code == 404:
-                print(f"No recording found for {device_id} and {recording_id}")
-                return []
-            elif result.status_code == 502:
-                print(f"Device {device_id} does not exits")
-                return []
-            else:
-                print("Recording not found")
-                print(result.status_code)
-                print(result.json())
-                return []
-
-    def download_recording_by_id(
-        self, device_id: str, recording_id: str = "recordingId-0", password: str = ""
-    ) -> None:
-        """Download the recording by ID and save it to the recordings folder"""
-
-        recordings_folder_name = "recordings"
-        recording_subfolder_name = recording_id
-
-        if password == "":
-            password = input("\nEnter your new passsword here: ")
-        recording_types = ["eeg", "imu"]
-        for data_type in recording_types:
-            with requests.Session() as session:
-
-                record_url_first = f"{settings.REST_API_LOGIN}recordings/"
-                record_url_second = f"{recording_id}/download/{data_type}"
-                record_url = record_url_first + record_url_second
-                result = session.get(record_url, auth=(device_id, password))
-
-                if result.status_code == 200:
-
-                    print(f"Recording ID file found, downloading {data_type} data")
-                    print(result.json())
-
-                    # Creating folder for recording
-                    folder_path = os.path.join(
-                        recordings_folder_name, recording_subfolder_name
-                    )
-                    if not os.path.exists(folder_path):
-                        os.makedirs(folder_path)
-
-                    # get url from responsex
-                    url = result.json()["downloadUrl"]
-                    result = session.get(url)
-                    filename = f"{recording_id}_{data_type}.csv"
-                    file_path = os.path.join(folder_path, filename)
-
-                    print(f"Writing to file: {file_path}")
-                    with open(file_path, "wb") as file:
-                        file.write(result.content)
-
-                    print("Downloading complete for recording ID: ", recording_id)
-
-                elif result.status_code == 401:
-                    if data_type == "eeg":
-                        print(f"Password for {device_id} is incorrect")
-
-                elif result.status_code == 403:
-                    if data_type == "eeg":
-                        print(
-                            "Wrong device ID, you can find the device ID in",
-                            " the logs in the format XX-XX-XX-XX-XX-XX",
-                        )
-                elif result.status_code == 412:
-                    if data_type == "eeg":
-                        print(f"Device {device_id} is not registered")
-                elif result.status_code == 404:
-                    print(f"No {data_type} recording found for this device ID")
-                elif result.status_code == 502:
-                    if data_type == "eeg":
-                        print(f"Device {device_id} does not exist")
-                else:
-                    if data_type == "eeg":
-                        print("Data download failed")
-                        print(result.status_code)
-                        print(result.json())
-
-
-@dataclass
-class GuardianDataModel:
-    """Data model for Guardian data"""
-
-    deviceTimestamp: Union[str, None]
-    deviceID: Union[str, None]
-    recordingID: Union[str, None]
-    payload: Union[str, None]  # This is a base64 encoded bytearray as a string
-    impedance: Union[int, None]
-    stop: Union[bool, None]
+"""
+Guardian API websocket utilities.
+"""
+import os
+import json
+from dataclasses import dataclass, asdict
+import socket
+import datetime
+import asyncio
+from typing import Union
+import requests
+import websockets
+import time
+from typing import Optional
+from dotenv import load_dotenv
+
+from .config import settings
+from .igeb_utils import unpack_from_queue
+from .mock_utils import mock_cloud_package
+from .debug_logs import *
+
+
+load_dotenv()
+
+FILTER_PACKAGE = "bp_filter_eeg"
+PACKAGE_RECEIPT = "SequenceNumber"
+
+
+class GuardianAPI:
+    """Main Guardian API client."""
+
+    def __init__(self, debug: bool = True) -> None:
+        """Initialize Guardian API client.
+
+        Args:
+            debug (bool, optional): Enable debug logging. Defaults to True.
+        """
+        self.debug: bool = debug
+        self.ping_timeout: int = 2
+        self.retry_time: int = 2
+        self.base64string_len: int = 236
+        self.first_message_check = True
+        self.final_message_sent = False
+        self.payload_valid = True
+        self.sample_rate = 250
+        self.sentinal = object()
+        self.encrypted_buffer_size = 3750  # 5 minutes => (5 * 60 * 250) / 20 = 3750
+        self.decrypted_buffer_size = 75000  # 5 minutes => (5 * 60 * 250) = 75000
+        self.encrypted_data_queue: asyncio.Queue = asyncio.Queue(
+            maxsize=self.encrypted_buffer_size
+        )
+        self.decrypted_data_queue: asyncio.Queue = asyncio.Queue(
+            maxsize=self.decrypted_buffer_size
+        )
+        self.initial_receipt_timeout = 15
+        self.runtime_receipt_timeout: float = 1  # Increase if slow connection
+        self.current_timeout = self.initial_receipt_timeout
+        self.initial_bi_directional_timeout = 15
+        self.runtime_bi_directional_timeout: float = 5  # Increase if slow connection
+        self.sending_time_limit = 0.01
+        self.bi_directional_timeout = self.initial_bi_directional_timeout
+        self.last_saved_time = time.time()
+        self.connected = False
+        self.data_model = GuardianDataModel(None, None, None, None, None, False)
+        self.websocket: Optional[websockets.WebSocketClientProtocol] = None  # type: ignore
+        self.final_receipt_got = False
+
+    async def connect_ws_api(
+        self,
+        data_queue: asyncio.Queue,
+        device_id: str = "deviceMockID",
+        recording_id: str = "dummy_recID",
+        impedance_measurement: bool = False,
+    ) -> None:
+        """Connect to the Guardian API websocket.
+
+        Args:
+            data_queue (asyncio.Queue): Data queue from the BLE client
+            deviceID (str, optional): Device ID. Defaults to "deviceMockID".
+            recordingID (str, optional): Recording ID. Defaults to "dummy_recID".
+
+        Raises:
+            Exception: If the websocket connection fails
+        """
+
+        def reset_data_model():
+            self.data_model.payload = None
+            self.data_model.impedance = None
+
+        async def pack_encrypted_queue():
+            if not self.encrypted_data_queue.full():
+                await self.encrypted_data_queue.put(
+                    [self.data_model.deviceTimestamp, self.data_model.payload]
+                )
+            else:
+                await self.encrypted_data_queue.get()
+
+        def pack_decrypted_queue(message):
+            if not self.decrypted_data_queue.full():
+                self.decrypted_data_queue.put_nowait(message[FILTER_PACKAGE])
+            else:
+                self.decrypted_data_queue.get_nowait()
+
+        async def unpack_and_load_data():
+            """Get data from the queue and pack it into a dataclass"""
+            data_valid = False
+            reset_data_model()
+            package = await data_queue.get()
+            (
+                device_timestamp,
+                device_id,
+                data,
+                stop,
+                impedance,
+            ) = unpack_from_queue(package)
+
+            if data is not None:
+                if len(data) == self.base64string_len:
+                    self.data_model.payload = data
+                    data_valid = True
+
+            if impedance is not None:
+                if isinstance(impedance, int):
+                    self.data_model.impedance = impedance
+                    data_valid = True
+
+            if device_timestamp is not None:
+                self.data_model.deviceTimestamp = device_timestamp
+
+            if device_id is not None:
+                self.data_model.deviceID = device_id
+
+            if stop is not None:
+                self.data_model.stop = stop
+                if stop is True:
+                    data_valid = True
+
+            return data_valid
+
+        async def create_timestamp(debug):
+            """Create a timestamp for the data"""
+            if data_queue.empty():
+                logging_empty(debug)  # Fetch the current time from the device
+                device_timestamp = datetime.datetime.now().astimezone().isoformat()
+            else:
+                logging_not_empty(debug)
+                package = (
+                    await data_queue.get()
+                )  # Fetch the timestamp from the BLE package
+                (device_timestamp, _, _, _, _) = unpack_from_queue(package)
+            return device_timestamp
+
+        async def unpack_and_load_data_termination():
+            """Get data from the queue and pack it into a dataclass"""
+            logging_cloud_termination(self.debug)
+            self.data_model.payload = "STOP_CANCELLED"
+            self.data_model.stop = True
+            device_timestamp = await create_timestamp(self.debug)
+            if device_timestamp is not None:
+                self.data_model.deviceTimestamp = device_timestamp
+
+        async def send_messages():
+            while True:
+
+                if not self.connected:
+                    break
+
+                if await unpack_and_load_data():
+                    await asyncio.shield(
+                        asyncio.sleep(self.sending_time_limit)
+                    )  # Wait as to not overload the cloud
+                    await asyncio.shield(
+                        self.websocket.send(json.dumps(asdict(self.data_model)))
+                    )
+                    await asyncio.shield(pack_encrypted_queue())
+
+                if self.data_model.stop:
+                    logging_stop_send(self.debug)
+                    self.current_timeout = (
+                        1000  # Wait until necessary for the stop to be sent
+                    )
+                    self.final_message_sent = True
+                    while not self.final_receipt_got:
+                        # It will loop in here and not update the
+                        # data until the stop is sent
+                        logging_waiting_for_stop_receipt(self.debug)
+                        await asyncio.sleep(1)
+                    break
+
+        async def receive_messages():
+            self.last_saved_time = time.time()
+            while True:
+
+                if not self.connected:
+                    break
+
+                message_str = await asyncio.shield(
+                    asyncio.wait_for(
+                        self.websocket.recv(), timeout=self.current_timeout
+                    )
+                )
+
+                if FILTER_PACKAGE in message_str:
+                    self.bi_directional_timeout = self.runtime_bi_directional_timeout
+                    message = json.loads(message_str)
+                    self.last_saved_time = time.time()
+                    pack_decrypted_queue(message)
+
+                elif PACKAGE_RECEIPT in message_str:
+                    self.current_timeout = self.runtime_receipt_timeout
+                    if self.first_message_check:
+                        self.first_message_check = False
+                        log_first_message(
+                            self.data_model,
+                            message_str,
+                            self.debug,
+                        )
+                    if self.final_message_sent:
+                        log_final_message(
+                            self.data_model,
+                            message_str,
+                            self.debug,
+                        )
+                        self.final_receipt_got = True
+                        break
+
+                bi_directional_timeout(impedance_measurement)
+
+        def bi_directional_timeout(impedance_measurement):
+            time_without_data = time.time() - self.last_saved_time
+            if (
+                time_without_data > self.bi_directional_timeout
+                and not impedance_measurement
+            ):
+                raise asyncio.TimeoutError
+
+        def once_initialise_variables():
+            # initiate flags
+            self.first_message_check = True
+            self.final_message_sent = False
+            self.data_model = GuardianDataModel(
+                None, device_id, recording_id, None, None, False
+            )
+
+        def on_connection_initialise_variables():
+            self.first_message_check = True
+            self.connected = True
+            self.bi_directional_timeout = self.initial_bi_directional_timeout
+            self.current_timeout = self.initial_receipt_timeout
+
+        async def handle_cancelled_error():
+            while True:
+                try:
+                    async with websockets.connect(  # type: ignore
+                        settings.WS_IDENTIFIER
+                    ) as self.websocket:
+                        logging_cancelled_error(self.debug)
+                        await unpack_and_load_data_termination()
+                        await self.websocket.send(json.dumps(asdict(self.data_model)))
+                        package_receipt = await self.websocket.recv()
+                        log_final_message(
+                            self.data_model,
+                            package_receipt,
+                            self.debug,
+                        )
+                        self.final_message_sent = True
+                        break
+                except Exception as err:
+                    await asyncio.sleep(self.ping_timeout)
+                    log_error_in_sending_stop(err, self.debug)
+                    continue
+
+        once_initialise_variables()
+
+        while True:
+            logging_connecting_to_cloud(self.debug)
+            try:
+                async with websockets.connect(settings.WS_IDENTIFIER) as self.websocket:  # type: ignore
+                    try:
+                        on_connection_initialise_variables()
+                        # for the websocket we want to increase to initial timeout each time
+                        logging_connection(settings.WS_IDENTIFIER, self.debug)
+                        send_task = asyncio.create_task(send_messages())
+                        receive_task = asyncio.create_task(receive_messages())
+                        await asyncio.gather(send_task, receive_task)
+
+                    except (
+                        websockets.exceptions.ConnectionClosed,  # type: ignore
+                    ) as error:
+                        try:
+                            logging_connection_closed(self.debug)
+                            self.connected = False
+                            await asyncio.shield(asyncio.sleep(self.ping_timeout))
+                            logging_reconnection(self.debug)
+                            self.bi_directional_timeout = (
+                                self.initial_bi_directional_timeout
+                            )
+                            continue
+                        except asyncio.CancelledError:
+                            await handle_cancelled_error()
+
+                    except asyncio.TimeoutError as error:
+                        try:
+                            log_interrupt_error(error, self.debug)
+                            self.connected = False
+                            await asyncio.shield(asyncio.sleep(self.ping_timeout))
+                            logging_reconnection(self.debug)
+                            self.bi_directional_timeout = (
+                                self.initial_bi_directional_timeout
+                            )
+                            continue
+                        except asyncio.CancelledError:
+                            await handle_cancelled_error()
+
+                    except asyncio.CancelledError:
+                        await handle_cancelled_error()
+
+                    finally:
+                        # Otherwise new tasks will be created which is a problem
+                        try:
+                            if not send_task.done():
+                                send_task.cancel()
+                            if not receive_task.done():
+                                receive_task.cancel()
+                        except Exception as error:
+                            print("These tasks does not exist yet")
+
+            except socket.gaierror as error:
+                logging_gaieerror(error, self.retry_time, self.debug)
+                await asyncio.sleep(self.retry_time)
+                continue
+
+            except ConnectionRefusedError as error:
+                logging_connection_refused(error, self.retry_time, self.debug)
+                await asyncio.sleep(self.retry_time)
+                continue
+
+            except Exception as error:
+                log_interrupt_error(error, self.debug)
+
+            finally:
+                # Otherwise new tasks will be created which is a problem
+                try:
+                    if not send_task.done():
+                        send_task.cancel()
+                    if not receive_task.done():
+                        receive_task.cancel()
+                except Exception as error:
+                    print("These tasks does not exist yet")
+
+            if self.final_message_sent:
+                logging_break(self.debug)
+                break
+
+        logging_api_completed(self.debug)
+
+    def get_recordings_info_all(
+        self, device_id: str = "mock-device-0", first_to_last=False, password: str = ""
+    ) -> list:
+        recordings_url = f"{settings.REST_API_LOGIN}recordings"
+        if password == "":
+            password = input("\nEnter your new passsword here: ")
+        with requests.Session() as session:
+            result = session.get(recordings_url, auth=(device_id, password))
+            if result.status_code == 200:
+                print("Recording list retrieved successfully")
+                recordings = result.json()
+                recordings.sort(
+                    key=lambda x: datetime.datetime.strptime(
+                        x["startDeviceTimestamp"], "%Y-%m-%dT%H:%M:%S.%fZ"
+                    ),
+                    reverse=first_to_last,
+                )
+                print(json.dumps(recordings, indent=4, sort_keys=True))
+                return result.json()
+            elif result.status_code == 401:
+                print(f"Password for {device_id} is incorrect")
+                return []
+            elif result.status_code == 403:
+                print(
+                    "Wrong device ID, you can find the device ID in",
+                    " the logs in the format XX-XX-XX-XX-XX-XX",
+                )
+                return []
+            elif result.status_code == 412:
+                print(
+                    f"Device {device_id} is not registered",
+                )
+                return []
+            elif result.status_code == 404:
+                print(f"No recording found for device {device_id}")
+                return []
+            elif result.status_code == 502:
+                print(f"Device {device_id} does not exist")
+                return []
+            else:
+                print("Loading recording list failed")
+                return []
+
+    def get_recording_info_by_id(
+        self, device_id: str, recording_id: str = "recordingId-0", password: str = ""
+    ) -> list:
+        recordings_url = f"{settings.REST_API_LOGIN}recordings/{recording_id}"
+
+        if password == "":
+            password = input("\nEnter your new passsword here: ")
+        with requests.Session() as session:
+            result = session.get(recordings_url, auth=(device_id, password))
+            if result.status_code == 200:
+                print("Recording ID file found")
+                print(json.dumps(result.json(), indent=4, sort_keys=True))
+                return result.json()
+            elif result.status_code == 401:
+                print(f"Password for {device_id} is incorrect")
+                return []
+            elif result.status_code == 403:
+                print(
+                    "Wrong device ID, you can find the device ID in",
+                    " the logs in the format XX-XX-XX-XX-XX-XX",
+                )
+                return []
+            elif result.status_code == 412:
+                print(
+                    f"Device {device_id} not registered",
+                )
+                return []
+            elif result.status_code == 404:
+                print(f"No recording found for {device_id} and {recording_id}")
+                return []
+            elif result.status_code == 502:
+                print(f"Device {device_id} does not exits")
+                return []
+            else:
+                print("Recording not found")
+                print(result.status_code)
+                print(result.json())
+                return []
+
+    def download_recording_by_id(
+        self, device_id: str, recording_id: str = "recordingId-0", password: str = ""
+    ) -> None:
+        """Download the recording by ID and save it to the recordings folder"""
+
+        recordings_folder_name = "recordings"
+        recording_subfolder_name = recording_id
+
+        if password == "":
+            password = input("\nEnter your new passsword here: ")
+        recording_types = ["eeg", "imu"]
+        for data_type in recording_types:
+            with requests.Session() as session:
+
+                record_url_first = f"{settings.REST_API_LOGIN}recordings/"
+                record_url_second = f"{recording_id}/download/{data_type}"
+                record_url = record_url_first + record_url_second
+                result = session.get(record_url, auth=(device_id, password))
+
+                if result.status_code == 200:
+
+                    print(f"Recording ID file found, downloading {data_type} data")
+                    print(result.json())
+
+                    # Creating folder for recording
+                    folder_path = os.path.join(
+                        recordings_folder_name, recording_subfolder_name
+                    )
+                    if not os.path.exists(folder_path):
+                        os.makedirs(folder_path)
+
+                    # get url from responsex
+                    url = result.json()["downloadUrl"]
+                    result = session.get(url)
+                    filename = f"{recording_id}_{data_type}.csv"
+                    file_path = os.path.join(folder_path, filename)
+
+                    print(f"Writing to file: {file_path}")
+                    with open(file_path, "wb") as file:
+                        file.write(result.content)
+
+                    print("Downloading complete for recording ID: ", recording_id)
+
+                elif result.status_code == 401:
+                    if data_type == "eeg":
+                        print(f"Password for {device_id} is incorrect")
+
+                elif result.status_code == 403:
+                    if data_type == "eeg":
+                        print(
+                            "Wrong device ID, you can find the device ID in",
+                            " the logs in the format XX-XX-XX-XX-XX-XX",
+                        )
+                elif result.status_code == 412:
+                    if data_type == "eeg":
+                        print(f"Device {device_id} is not registered")
+                elif result.status_code == 404:
+                    print(f"No {data_type} recording found for this device ID")
+                elif result.status_code == 502:
+                    if data_type == "eeg":
+                        print(f"Device {device_id} does not exist")
+                else:
+                    if data_type == "eeg":
+                        print("Data download failed")
+                        print(result.status_code)
+                        print(result.json())
+
+
+@dataclass
+class GuardianDataModel:
+    """Data model for Guardian data"""
+
+    deviceTimestamp: Union[str, None]
+    deviceID: Union[str, None]
+    recordingID: Union[str, None]
+    payload: Union[str, None]  # This is a base64 encoded bytearray as a string
+    impedance: Union[int, None]
+    stop: Union[bool, None]
```

### Comparing `idun_guardian_client-1.1b4/src/idun_guardian_client/igeb_bluetooth.py` & `idun_guardian_client-1.1b9/src/idun_guardian_client/igeb_bluetooth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,764 +1,769 @@
-"""
-Guardian Bluetooth utils.
-"""
-import sys
-import asyncio
-import os
-from codecs import utf_8_encode
-import logging
-import time
-import base64
-import datetime
-from bleak import BleakClient, BleakScanner, exc
-
-from .config import settings
-from .debug_logs import *
-
-
-class GuardianBLE:
-    """Main Guardian BLE client."""
-
-    def __init__(self, address: str = "", debug: bool = True) -> None:
-        """Initialize the Guardian BLE client.
-
-        Args:
-            address (str, optional): BLE device address. Defaults to "".
-            debug (bool, optional): Debug mode. Defaults to True.
-        """
-        self.client: BleakClient
-
-        # Debugging mode
-        self.address = address
-        self.debug = debug
-        self.write_to_file: bool = debug
-
-        # Initial connection flags
-        self.initialise_connection: bool = True
-        self.connection_established = False
-        self.time_left = True
-        self.initial_time = True
-
-        # Bluetooth reconnect delay
-        self.original_time = time.time()
-        self.reconnect_try_amount = 50
-        self.try_to_connect_timeout = self.reconnect_try_amount
-
-        # Bluetooth timings
-        self.ble_delay = 1
-        self.ble_stop_delay = 1
-        self.device_lost = False
-
-        # API timeings
-        self.sent_final_package_time = 1
-
-        # The timing constants
-        self.sample_rate = 250
-        self.amount_samples_packet = 20
-        self.max_index = 256
-        self.prev_index = 0
-        self.prev_timestamp = 0
-
-        self.remaining_time = 0
-
-        self.get_ble_characteristic()
-
-        loggig_ble_init(self.debug)
-
-    def get_ble_characteristic(self) -> None:
-        """Get the environment variables."""
-        # General information
-        self.battery_id = settings.UUID_BATT_GDK
-        self.device_service = settings.UUID_DEVICE_SERVICE
-        self.mac_uuid = settings.UUID_MAC_ID
-        self.firmware_uuid = settings.UUID_FIRMWARE_VERSION
-
-        # EEG/IMU measurement
-        self.meas_eeg_id = settings.UUID_MEAS_EEGIMU
-        self.command_id = settings.UUID_CMD
-        self.start_cmd = settings.START_CMD
-        self.stop_cmd = settings.STOP_CMD
-
-        # Impedance measurement
-        self.meas_imp_id = settings.UUID_MEAS_IMP
-        self.start_imp_cmd = settings.START_IMP_CMD
-        self.stop_imp_cmd = settings.STOP_IMP_CMD
-        self.notch_freq_50_cfg = settings.NOTCH_FREQ_50_CFG
-        self.notch_freq_60_cfg = settings.NOTCH_FREQ_60_CFG
-
-        # LED control
-        self.cfg_id = settings.UUID_CFG
-        self.led_on_cfg = settings.LED_ON_CFG
-        self.led_off_cfg = settings.LED_OFF_CFG
-
-    async def get_ble_devices(self) -> list:
-        """
-        Scan for devices and return a list of devices.
-        """
-        devices_dict: dict = {}
-        ble_device_list: list = []
-        devices = await BleakScanner.discover()
-        igeb_name = "IGEB"
-        device_id = 0
-        print("\n----- Available devices -----\n")
-        print("Index | Name | Address")
-        print("----------------------------")
-        for _, device in enumerate(devices):
-            # print device discovered
-            if device.name == igeb_name:
-                print(f"{device_id}     | {device.name} | {device.address}")
-                devices_dict[device.address] = []
-                devices_dict[device.address].append(device.name)
-                ble_device_list.append(device.address)
-                device_id += 1
-        print("----------------------------\n")
-        return ble_device_list
-
-    async def get_device_mac(self) -> str:
-        """Get the device MAC address.
-        This is different from BLE device address
-        (UUID on Mac or MAC address on Windows)
-
-        Args:
-            device_name (str): Device name
-
-        Returns:
-            str: MAC address
-        """
-        async with BleakClient(self.address) as client:
-            logging_searching(self.debug)
-            value = bytes(await client.read_gatt_char(self.mac_uuid))
-            await asyncio.sleep(self.ble_delay)
-            firmware_version = bytes(await client.read_gatt_char(self.firmware_uuid))
-            mac_address = value.decode("utf-8")
-            firmware_decoded = firmware_version.decode("utf-8")
-            mac_address = mac_address.replace(":", "-")
-            logging_device_info(self.debug, mac_address, firmware_decoded)
-            return mac_address
-
-    async def search_device(self) -> str:
-        """This function searches for the device and returns the address of the device.
-        If the device is not found, it exits the program. If multiple devices are found,
-        it asks the user to select the device. If one device is found, it returns the
-        address of the device.
-
-        Returns:
-            _type_: _description_
-        """
-
-        ble_device_list = await self.get_ble_devices()
-
-        if len(ble_device_list) == 0:
-            logging_device_not_found(self.debug)
-            self.exit_system()
-        elif len(ble_device_list) == 1:
-            logging_device_found(self.debug, ble_device_list)
-            self.address = ble_device_list[0]
-        else:
-            index_str = input(
-                "Enter the index of the GDK device you want to connect to \
-                \nIf cannot find the device, please restart the program and try again: "
-            )
-            index = int(index_str)
-            self.address = ble_device_list[index]
-        logging_device_address(self.debug, self.address)
-        return self.address
-
-    def exit_system(self) -> None:
-        """Exit the system."""
-        try:
-            sys.exit(0)
-        except SystemExit:
-            os._exit(0)
-
-    async def connect_to_device(self):
-        """
-        This function initialises the connection to the device.
-        It finds the device using the address, sets up callback,
-        and connects to the device.
-        """
-        logging_trying_to_connect(self.debug, self.address)
-        device = await BleakScanner.find_device_by_address(self.address, timeout=20.0)
-        if not device:
-            raise exc.BleakError(
-                f"A device with address {self.address} could not be found."
-            )
-        self.client = BleakClient(
-            device, disconnected_callback=self.disconnected_callback
-        )
-        logging_trying_to_connect(self.debug, self.address)
-        await self.client.connect()
-        self.connection_established = True
-        logging_connected(self.debug, self.address)
-
-    def disconnected_callback(self, client):  # pylint: disable=unused-argument
-        """
-        Callback function when device is disconnected.
-
-        Args:
-            client (BleakClient): BleakClient object
-        """
-        logging_disconnected_recognised(self.debug)
-        self.connection_established = False
-        self.initialise_connection = True
-
-    async def run_ble_record(
-        self,
-        data_queue: asyncio.Queue,
-        record_time=60,
-        mac_id="MAC_ID",
-        led_sleep: bool = False,
-        impedance_measurement: bool = False,
-        mains_freq_60hz: bool = False,
-    ) -> None:
-        """
-        This function runs the recording of the data. It sets up the bluetooth
-        connection, starts the recording, and then reads the data and adds it to
-        the queue. The API class then reads the data from the queue and sends it
-        to the cloud.
-
-        Args:
-            data_queue (asyncio.Queue): Queue to store the data
-            record_time (_type_): The time to record for
-            mac_id (_type_): The MAC address of the device
-            led_sleep (_type_): Whether to turn off the LED
-
-        Raises:
-            BleakError: _description_
-        """
-
-        def time_stamp_creator(new_index):
-            """
-            This function creates a timestamp for the cloud based on the
-            time the recording started. Each time stamp is based on the index
-            of that is sent from the device. The index is the number of iterates
-            between 0 and 256. The time stamp is the 1/250s multiplied by the
-            index.
-
-            Args:
-                new_index (int): Index of the data point from the ble packet
-
-            Returns:
-                str: Timestamp in the format of YYYY-MM-DDTHH:MM:SS
-            """
-            index_diff = new_index - self.prev_index
-
-            if self.prev_timestamp == 0:
-                time_data = datetime.datetime.now().astimezone().isoformat()
-                # convert time_data to a float in seconds
-                time_data = time.mktime(
-                    datetime.datetime.strptime(
-                        time_data, "%Y-%m-%dT%H:%M:%S.%f%z"
-                    ).timetuple()
-                )
-                new_time_stamp = time_data
-            else:
-                multiplier = (index_diff + self.max_index) % self.max_index
-                new_time_stamp = (
-                    self.amount_samples_packet * (1 / self.sample_rate) * multiplier
-                ) + self.prev_timestamp
-
-            self.prev_index = new_index
-            self.prev_timestamp = new_time_stamp
-
-            time_stamp_isoformat = datetime.datetime.fromtimestamp(
-                new_time_stamp
-            ).isoformat()
-
-            return time_stamp_isoformat
-
-        async def data_handler(_, data):
-            """Data handler for the BLE client.
-                Data is put in a queue and forwarded to the API.
-
-            Args:
-                callback (handler Object): Handler object
-                data (bytes): Binary data package
-            """
-            data_base_64 = base64.b64encode(data).decode("ascii")
-            new_time_stamp = time_stamp_creator(data[1])
-
-            if self.write_to_file:
-                self.data_recording_logfile.write(f"{data_base_64},\n")
-
-            package = {
-                "timestamp": new_time_stamp,
-                "deviceID": mac_id,
-                "data": data_base_64,
-                "stop": False,
-            }
-            # print the size of the queue
-            # print(f"[BLE]: Queue size: {data_queue.qsize()}")
-            if not data_queue.full():
-                await asyncio.shield(data_queue.put(package))
-            else:
-                await asyncio.shield(data_queue.get())
-
-        async def battery_handler(_, data):
-            """Battery handler for the BLE client.
-            Args:
-                callback (handler Object): Handler object
-                data (bytes): Battery Level as uint8_t
-            """
-            logging_batterylevel(self.debug, data)
-
-        async def impedance_handler(_, data):
-            """Impedance handler for the BLE client.
-                Data is put in a queue and forwarded to the API.
-
-            Args:
-                callback (handler Object): Handler object
-                data (bytes): Binary data package with impedance values
-            """
-            data_int = int.from_bytes(data, byteorder="little")
-            print(f"[BLE]: Impedance value : {round(data_int/1000,2)} kOhms")
-            if self.write_to_file:
-                self.data_recording_logfile.write(f"{data_int}\n")
-
-            package = {
-                "timestamp": datetime.datetime.now().astimezone().isoformat(),
-                "deviceID": mac_id,
-                "stop": False,
-                "impedance": data_int,
-            }
-            # add the received impedance data to the queue
-            if not data_queue.full():
-                await data_queue.put(package)
-            else:
-                await data_queue.get()
-
-        async def send_start_commands_recording():
-            """Send start commands to the device."""
-            logging_sending_start(self.debug)
-
-            # ------------------ Configuration ------------------
-            if led_sleep:
-                await asyncio.sleep(self.ble_delay)
-                await self.client.write_gatt_char(
-                    self.cfg_id, utf_8_encode(self.led_off_cfg)[0]
-                )
-            # ------------------ Subscribe to notifications ------------------
-            # Notify the client that these two services are required
-            logging_subscribing_eeg_notification(self.debug)
-            await asyncio.sleep(self.ble_delay)
-            await self.client.start_notify(self.meas_eeg_id, data_handler)
-
-            logging_subscribing_battery_notification(self.debug)
-            await asyncio.sleep(self.ble_delay)
-            await self.client.start_notify(self.battery_id, battery_handler)
-
-            # ------------------ Start commands ------------------
-            # sleep so that cleint can respond
-            await asyncio.sleep(self.ble_delay)
-            # send start command for recording data
-            await self.client.write_gatt_char(
-                self.command_id, utf_8_encode(self.start_cmd)[0]
-            )
-
-        async def send_start_commands_impedance():
-            # ----------------- Configuration -----------------
-            if mains_freq_60hz:
-                await asyncio.sleep(self.ble_delay)
-                await self.client.write_gatt_char(
-                    self.cfg_id, utf_8_encode(self.notch_freq_60_cfg)[0]
-                )
-            else:
-                await asyncio.sleep(self.ble_delay)
-                await self.client.write_gatt_char(
-                    self.cfg_id, utf_8_encode(self.notch_freq_50_cfg)[0]
-                )
-
-            # ----------------- Subscribe -----------------
-            logging_subscribing_impedance_notification(self.debug)
-            await asyncio.sleep(self.ble_delay)
-            await self.client.start_notify(self.meas_imp_id, impedance_handler)
-
-            # ----------------- Send start command -----------------
-            logging_starting_impedance_measurement_commands(self.debug)
-            await asyncio.sleep(self.ble_delay)
-            await self.client.write_gatt_char(
-                self.command_id, utf_8_encode(self.start_imp_cmd)[0]
-            )
-
-        async def stop_impedance_timeout():
-            """Stop recording gracefully."""
-            # make sure the last data is now a stop command
-            package = {
-                "timestamp": datetime.datetime.now().astimezone().isoformat(),
-                "deviceID": mac_id,
-                "stop": True,
-            }
-            # ------------------ Load final stop package ------------------
-            if not data_queue.full():
-                await data_queue.put(package)
-            else:
-                await data_queue.get()
-                await data_queue.put(package)
-            logging_sending_stop(self.debug)
-            # ------------------ API should send already loaded package  ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # This gives time for the api to send already loaded data
-            logging_sending_stop_device(self.debug)
-            await asyncio.sleep(self.ble_delay)
-
-            await self.client.write_gatt_char(
-                self.command_id, utf_8_encode(self.stop_imp_cmd)[0]
-            )
-
-            # ------------------ Disconnect command to device ------------------
-            logging_sending_disconnect(self.debug)
-            await asyncio.sleep(self.ble_stop_delay)
-            await self.client.disconnect()
-            await asyncio.sleep(self.ble_stop_delay)
-
-            if self.write_to_file:
-                self.data_recording_logfile.close()
-            logging_recording_successfully_stopped(self.debug)
-
-        async def stop_recording_timeout():
-            """Stop recording gracefully."""
-
-            # make sure the last data is now a stop command
-            package = {
-                "timestamp": datetime.datetime.now().astimezone().isoformat(),
-                "deviceID": mac_id,
-                "data": "STOP_TIMEOUT",
-                "stop": True,
-            }
-            # ------------------ Load final stop package ------------------
-            if not data_queue.full():
-                await data_queue.put(package)
-            else:
-                await data_queue.get()
-                await data_queue.put(package)
-            logging_sending_stop(self.debug)
-            # ------------------ API should send already loaded package  ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # This gives time for the api to send already loaded data
-            logging_sending_stop_device(self.debug)
-            await asyncio.sleep(self.ble_delay)
-
-            await self.client.write_gatt_char(
-                self.command_id, utf_8_encode(self.stop_cmd)[0]
-            )
-
-            if led_sleep:
-                logging_turn_ble_on(self.debug)
-                await asyncio.sleep(self.ble_delay)
-                await self.client.write_gatt_char(
-                    self.cfg_id, utf_8_encode(self.led_on_cfg)[0]
-                )
-            # ------------------ Disconnect command to device ------------------
-            logging_sending_disconnect(self.debug)
-            await asyncio.sleep(self.ble_stop_delay)
-            await self.client.disconnect()
-            await asyncio.sleep(self.ble_stop_delay)
-
-            if self.write_to_file:
-                self.data_recording_logfile.close()
-            logging_recording_successfully_stopped(self.debug)
-
-        async def stop_impedance_cancelled_script():
-            """Stop recording abruptly."""
-            logging_keyboard_interrupt(self.debug)
-
-            # ------------------ Sending final API packages ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # Give API time to send last package
-            # With its own interupt handling
-            # ------------------ Send stop EEG recording command ------------------
-            logging_sending_stop_device(self.debug)
-            await asyncio.sleep(self.ble_delay)
-            await self.client.write_gatt_char(
-                self.command_id, utf_8_encode(self.stop_imp_cmd)[0]
-            )
-
-            # ------------------ Disconnecting commands ------------------
-            logging_sending_disconnect(self.debug)
-            await asyncio.sleep(self.ble_stop_delay)
-            await self.client.disconnect()
-            await asyncio.sleep(self.ble_stop_delay)
-            # ------------------ Closing file  ------------------
-            if self.write_to_file:
-                self.data_recording_logfile.close()
-            logging_recording_successfully_stopped(self.debug)
-            # ------------------ Sending final API packages ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # Give API time to send last package
-            # With its own interupt handling
-
-        async def stop_recording_cancelled_script():
-            """Stop recording abruptly."""
-            logging_keyboard_interrupt(self.debug)
-
-            # ------------------ Sending final API packages ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # Give API time to send last package
-            # With its own interupt handling
-            # ------------------ Send stop EEG recording command ------------------
-            logging_sending_stop_device(self.debug)
-            await asyncio.sleep(self.ble_delay)
-            await self.client.write_gatt_char(
-                self.command_id, utf_8_encode(self.stop_cmd)[0]
-            )
-            # ------------------ Configuring LED back on ------------------
-            if led_sleep:
-                logging_turn_led_on(self.debug)
-                await asyncio.sleep(self.ble_delay)
-                await self.client.write_gatt_char(
-                    self.cfg_id, utf_8_encode(self.led_on_cfg)[0]
-                )
-            # ------------------ Disconnecting commands ------------------
-            logging_sending_disconnect(self.debug)
-            await asyncio.sleep(self.ble_stop_delay)
-            await self.client.disconnect()
-            await asyncio.sleep(self.ble_stop_delay)
-            # ------------------ Closing file  ------------------
-            if self.write_to_file:
-                self.data_recording_logfile.close()
-            logging_recording_successfully_stopped(self.debug)
-            # ------------------ Sending final API packages ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # Give API time to send last package
-            # With its own interupt handling
-
-        async def stop_recording_device_lost():
-            """Stop recording device lost."""
-            logging_device_lost_give_up(self.debug)
-            # ------------------ Sending final API packages ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(self.ble_delay)  # Give API time to send last package
-            # ------------------ Loading last package ------------------
-            logging_sending_stop(self.debug)
-            package = {
-                "timestamp": datetime.datetime.now().astimezone().isoformat(),
-                "deviceID": mac_id,
-                "data": "STOP_DEVICE_LOST",
-                "stop": True,
-            }
-            # pack the stop command
-            if not data_queue.full():
-                await data_queue.put(package)
-            else:
-                await data_queue.get()
-                await data_queue.put(package)
-            # ------------------ Sending final API packages ------------------
-            logging_giving_time_api(self.debug)
-            await asyncio.sleep(
-                self.sent_final_package_time
-            )  # Give API time to send last package
-            # ------------------ Closing file ------------------
-            if self.write_to_file:
-                self.data_recording_logfile.close()
-
-            return True
-
-        async def bluetooth_reconnect():
-            """Set flags to reconnect to bluetooth device."""
-            self.try_to_connect_timeout = self.try_to_connect_timeout - 1
-            if self.try_to_connect_timeout <= 0:
-                self.device_lost = await stop_recording_device_lost()
-            logging_trying_to_connect_again(self.debug, self.try_to_connect_timeout)
-            self.connection_established = False
-            self.initialise_connection = True
-
-        def initialise_file():
-            """Initialise file for recording."""
-            if self.write_to_file:
-                if not os.path.exists("./logs"):
-                    os.makedirs("logs")
-
-                if not impedance_measurement:
-                    measurement_type = "rec"
-                else:
-                    measurement_type = "imp"
-
-                datestr = datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
-                recording_filename = f"./logs/IGEB-{measurement_type}-{datestr}.txt"
-                self.data_recording_logfile = open(
-                    recording_filename, "w", encoding="utf-8"
-                )
-
-        def initialise_timestamps():
-            if self.initial_time:
-                self.initial_time = False  # record that this is the initial time
-                self.original_time = time.time()
-
-        async def main_loop():
-            while True:
-                if self.connection_established:
-
-                    await asyncio.shield(
-                        asyncio.sleep(self.ble_delay)
-                    )  # sleep so that everything can happen
-                    self.remaining_time = record_time - (
-                        time.time() - self.original_time
-                    )
-                    print(f"Time left: {round(self.remaining_time)}s")
-
-                    if self.remaining_time <= 0:
-                        logging_time_reached(self.debug, self.original_time)
-                        if not impedance_measurement:
-                            await stop_recording_timeout()
-                        else:
-                            await stop_impedance_timeout()
-                        break
-
-                else:
-                    break
-
-        # >>>>>>>>>>>>>>>>>>>>> Start of recording process <<<<<<<<<<<<<<<<<<<<<<<<
-        # ------------------ Initialise values for timestamps ------------------
-        self.prev_timestamp = 0
-        self.prev_index = -1
-        # ------------------ Initialise time values for recording timeout ------------------
-        # This has been decoupled from the device timing for robustness
-        self.original_time = time.time()
-        self.initial_time = True
-        self.time_left = True
-        self.initial_time = True
-        # ------------------ Initialise connection values for trying to connect again ------------------
-        self.connection_established = False
-        self.try_to_connect_timeout = self.reconnect_try_amount
-        # ------------------ Initialise log file ------------------
-        initialise_file()
-
-        while True:
-            try:
-                if self.initialise_connection:
-                    self.initialise_connection = False
-                    await self.connect_to_device()
-
-                if self.client.is_connected:
-                    logging_device_connected_general(self.debug)
-
-                    if not impedance_measurement:
-                        await send_start_commands_recording()
-                    else:
-                        await send_start_commands_impedance()
-
-                    logging_recording_started(self.debug)
-                    self.try_to_connect_timeout = (
-                        self.reconnect_try_amount
-                    )  # reset counter
-                    # >>>>>>>>>>>>>>>>>>>>> Main loop <<<<<<<<<<<<<<<<<<<<<<<<
-                    initialise_timestamps()
-                    await asyncio.shield(main_loop())
-                    # >>>>>>>>>>>>>>>>>>>>> Main loop <<<<<<<<<<<<<<<<<<<<<<<<
-
-                if self.remaining_time <= 0:
-                    break
-
-                if not self.connection_established:
-                    logging_disconnected_recognised(self.debug)
-                    await bluetooth_reconnect()
-                    if self.device_lost:
-                        break
-
-            except asyncio.CancelledError:
-                if not impedance_measurement:
-                    await stop_recording_cancelled_script()
-                else:
-                    await stop_impedance_cancelled_script()
-                break
-
-            except Exception as error:
-                logging_ble_client_lost(self.debug, error)
-
-            finally:
-                logging_ensuring_ble_disconnected(self.debug)
-                await asyncio.sleep(self.ble_stop_delay)
-                await self.client.disconnect()
-                await asyncio.sleep(self.ble_stop_delay)
-                self.connection_established = False
-
-        logging_ble_complete(self.debug)
-
-    async def get_service_and_char(self) -> None:
-        """Get the services and characteristics of the device."""
-        try:
-            async with BleakClient(self.address) as client:
-                logging_device_connected_general(self.debug)
-
-                for service in client.services:
-                    logging_device_info_uuid(self.debug, service)
-
-                    for char in service.characteristics:
-                        if "read" in char.properties:
-                            try:
-                                value = bytes(await client.read_gatt_char(char.uuid))
-                            except exc.BleakError as err:
-                                value = str(err).encode()
-                        else:
-                            value = None
-                        logging_device_info_characteristic(self.debug, char, value)
-
-                await asyncio.sleep(self.ble_stop_delay)
-                await client.disconnect()
-                await asyncio.sleep(self.ble_stop_delay)
-                logging_sending_disconnect(self.debug)
-
-        except exc.BleakError as err:
-            logging_device_connection_failed(self.debug, err)
-
-    async def read_battery_level(self) -> None:
-        """Read the battery level of the device given pre-defined interval."""
-        logging_reading_battery_level(self.debug)
-
-        async with BleakClient(self.address) as client:
-            logging_device_connected_general(self.debug)
-
-            try:
-                await asyncio.sleep(self.ble_delay)
-                value = int.from_bytes(
-                    (await client.read_gatt_char(self.battery_id)), byteorder="little"
-                )
-                print("-----------------------------")
-                print(f"\nBattery level: {value}%\n")
-                print("-----------------------------")
-                logging_batterylevel_int(self.debug, value)
-
-                await asyncio.sleep(self.ble_stop_delay)
-                await client.disconnect()
-                await asyncio.sleep(self.ble_stop_delay)
-                logging_sending_disconnect(self.debug)
-
-            except exc.BleakError as err:
-                # log the error
-                logging_device_connection_failed(self.debug, err)
-
-    async def get_device_information(self) -> dict:
-        """Read the device information of the device."""
-
-        device_info = {}
-
-        async with BleakClient(self.address) as client:
-            logging_device_connected_general(self.debug)
-
-            for service in client.services:
-                if service.uuid == self.device_service:
-                    for char in service.characteristics:
-                        if "read" in char.properties:
-                            try:
-                                value = bytes(await client.read_gatt_char(char.uuid))
-                            except exc.BleakError as err:
-                                value = str(err).encode()
-                        else:
-                            value = None
-
-                        print(f"{ char.description}:{str(value)}")
-                        device_info[char.description] = str(value)
-                        logging_device_description_list(self.debug, char, value)
-
-        return device_info
+"""
+Guardian Bluetooth utils.
+"""
+import sys
+import asyncio
+import os
+from codecs import utf_8_encode
+import logging
+import time
+import base64
+import datetime
+from bleak import BleakClient, BleakScanner, exc
+
+from .config import settings
+from .debug_logs import *
+
+SEARCH_BREAK = 3
+
+class GuardianBLE:
+    """Main Guardian BLE client."""
+
+    def __init__(self, address: str = "", debug: bool = True) -> None:
+        """Initialize the Guardian BLE client.
+
+        Args:
+            address (str, optional): BLE device address. Defaults to "".
+            debug (bool, optional): Debug mode. Defaults to True.
+        """
+        self.client: BleakClient
+
+        # Debugging mode
+        self.address = address
+        self.debug = debug
+        self.write_to_file: bool = debug
+
+        # Initial connection flags
+        self.initialise_connection: bool = True
+        self.connection_established = False
+        self.time_left = True
+        self.initial_time = True
+
+        # Bluetooth reconnect delay
+        self.original_time = time.time()
+        self.reconnect_try_amount = 50
+        self.try_to_connect_timeout = self.reconnect_try_amount
+
+        # Bluetooth timings
+        self.ble_delay = 1
+        self.ble_stop_delay = 1
+        self.device_lost = False
+
+        # API timeings
+        self.sent_final_package_time = 1
+
+        # The timing constants
+        self.sample_rate = 250
+        self.amount_samples_packet = 20
+        self.max_index = 256
+        self.prev_index = 0
+        self.prev_timestamp = 0
+
+        self.remaining_time = 0
+
+        self.get_ble_characteristic()
+
+        loggig_ble_init(self.debug)
+
+    def get_ble_characteristic(self) -> None:
+        """Get the environment variables."""
+        # General information
+        self.battery_id = settings.UUID_BATT_GDK
+        self.device_service = settings.UUID_DEVICE_SERVICE
+        self.mac_uuid = settings.UUID_MAC_ID
+        self.firmware_uuid = settings.UUID_FIRMWARE_VERSION
+
+        # EEG/IMU measurement
+        self.meas_eeg_id = settings.UUID_MEAS_EEGIMU
+        self.command_id = settings.UUID_CMD
+        self.start_cmd = settings.START_CMD
+        self.stop_cmd = settings.STOP_CMD
+
+        # Impedance measurement
+        self.meas_imp_id = settings.UUID_MEAS_IMP
+        self.start_imp_cmd = settings.START_IMP_CMD
+        self.stop_imp_cmd = settings.STOP_IMP_CMD
+        self.notch_freq_50_cfg = settings.NOTCH_FREQ_50_CFG
+        self.notch_freq_60_cfg = settings.NOTCH_FREQ_60_CFG
+
+        # LED control
+        self.cfg_id = settings.UUID_CFG
+        self.led_on_cfg = settings.LED_ON_CFG
+        self.led_off_cfg = settings.LED_OFF_CFG
+
+    async def get_ble_devices(self) -> list:
+        """
+        Scan for devices and return a list of devices.
+        """
+        devices_dict: dict = {}
+        ble_device_list: list = []
+        devices = await BleakScanner.discover()
+        igeb_name = "IGEB"
+        device_id = 0
+        print("\n----- Available devices -----\n")
+        print("Index | Name | Address")
+        print("----------------------------")
+        for _, device in enumerate(devices):
+            # print device discovered
+            if device.name == igeb_name:
+                print(f"{device_id}     | {device.name} | {device.address}")
+                devices_dict[device.address] = []
+                devices_dict[device.address].append(device.name)
+                ble_device_list.append(device.address)
+                device_id += 1
+        print("----------------------------\n")
+        return ble_device_list
+
+    async def get_device_mac(self) -> str:
+        """Get the device MAC address.
+        This is different from BLE device address
+        (UUID on Mac or MAC address on Windows)
+
+        Args:
+            device_name (str): Device name
+
+        Returns:
+            str: MAC address
+        """
+        async with BleakClient(self.address) as client:
+            logging_searching(self.debug)
+            value = bytes(await client.read_gatt_char(self.mac_uuid))
+            await asyncio.sleep(self.ble_delay)
+            firmware_version = bytes(await client.read_gatt_char(self.firmware_uuid))
+            mac_address = value.decode("utf-8")
+            firmware_decoded = firmware_version.decode("utf-8")
+            mac_address = mac_address.replace(":", "-")
+            logging_device_info(self.debug, mac_address, firmware_decoded)
+            return mac_address
+
+    async def search_device(self) -> str:
+        """This function searches for the device and returns the address of the device.
+        If the device is not found, it exits the program. If multiple devices are found,
+        it asks the user to select the device. If one device is found, it returns the
+        address of the device.
+
+        Returns:
+            _type_: _description_
+        """
+
+        while True:
+
+            ble_device_list = await self.get_ble_devices()
+            if len(ble_device_list) == 0:
+                logging_device_not_found(self.debug,SEARCH_BREAK)
+                await asyncio.sleep(SEARCH_BREAK)
+
+            elif len(ble_device_list) == 1:
+                logging_device_found(self.debug, ble_device_list)
+                self.address = ble_device_list[0]
+                break
+            else:
+                index_str = input(
+                    "Enter the index of the GDK device you want to connect to \
+                    \nIf cannot find the device, please restart the program and try again: "
+                )
+                index = int(index_str)
+                self.address = ble_device_list[index]
+                break
+
+        logging_device_address(self.debug, self.address)
+
+        return self.address
+
+    def exit_system(self) -> None:
+        """Exit the system."""
+        try:
+            sys.exit(0)
+        except SystemExit:
+            os._exit(0)
+
+    async def connect_to_device(self):
+        """
+        This function initialises the connection to the device.
+        It finds the device using the address, sets up callback,
+        and connects to the device.
+        """
+        logging_trying_to_connect(self.debug, self.address)
+        device = await BleakScanner.find_device_by_address(self.address, timeout=20.0)
+        if not device:
+            raise exc.BleakError(
+                f"A device with address {self.address} could not be found."
+            )
+        self.client = BleakClient(
+            device, disconnected_callback=self.disconnected_callback
+        )
+        logging_trying_to_connect(self.debug, self.address)
+        await self.client.connect()
+        self.connection_established = True
+        logging_connected(self.debug, self.address)
+
+    def disconnected_callback(self, client):  # pylint: disable=unused-argument
+        """
+        Callback function when device is disconnected.
+
+        Args:
+            client (BleakClient): BleakClient object
+        """
+        logging_disconnected_recognised(self.debug)
+        self.connection_established = False
+        self.initialise_connection = True
+
+    async def run_ble_record(
+        self,
+        data_queue: asyncio.Queue,
+        record_time=60,
+        mac_id="MAC_ID",
+        led_sleep: bool = False,
+        impedance_measurement: bool = False,
+        mains_freq_60hz: bool = False,
+    ) -> None:
+        """
+        This function runs the recording of the data. It sets up the bluetooth
+        connection, starts the recording, and then reads the data and adds it to
+        the queue. The API class then reads the data from the queue and sends it
+        to the cloud.
+
+        Args:
+            data_queue (asyncio.Queue): Queue to store the data
+            record_time (_type_): The time to record for
+            mac_id (_type_): The MAC address of the device
+            led_sleep (_type_): Whether to turn off the LED
+
+        Raises:
+            BleakError: _description_
+        """
+
+        def time_stamp_creator(new_index):
+            """
+            This function creates a timestamp for the cloud based on the
+            time the recording started. Each time stamp is based on the index
+            of that is sent from the device. The index is the number of iterates
+            between 0 and 256. The time stamp is the 1/250s multiplied by the
+            index.
+
+            Args:
+                new_index (int): Index of the data point from the ble packet
+
+            Returns:
+                str: Timestamp in the format of YYYY-MM-DDTHH:MM:SS
+            """
+            index_diff = new_index - self.prev_index
+
+            if self.prev_timestamp == 0:
+                time_data = datetime.datetime.now().astimezone().isoformat()
+                # convert time_data to a float in seconds
+                time_data = time.mktime(
+                    datetime.datetime.strptime(
+                        time_data, "%Y-%m-%dT%H:%M:%S.%f%z"
+                    ).timetuple()
+                )
+                new_time_stamp = time_data
+            else:
+                multiplier = (index_diff + self.max_index) % self.max_index
+                new_time_stamp = (
+                    self.amount_samples_packet * (1 / self.sample_rate) * multiplier
+                ) + self.prev_timestamp
+
+            self.prev_index = new_index
+            self.prev_timestamp = new_time_stamp
+
+            time_stamp_isoformat = datetime.datetime.fromtimestamp(
+                new_time_stamp
+            ).isoformat()
+
+            return time_stamp_isoformat
+
+        async def data_handler(_, data):
+            """Data handler for the BLE client.
+                Data is put in a queue and forwarded to the API.
+
+            Args:
+                callback (handler Object): Handler object
+                data (bytes): Binary data package
+            """
+            data_base_64 = base64.b64encode(data).decode("ascii")
+            new_time_stamp = time_stamp_creator(data[1])
+
+            if self.write_to_file:
+                self.data_recording_logfile.write(f"{data_base_64},\n")
+
+            package = {
+                "timestamp": new_time_stamp,
+                "deviceID": mac_id,
+                "data": data_base_64,
+                "stop": False,
+            }
+            if not data_queue.full():
+                await asyncio.shield(data_queue.put(package))
+            else:
+                await asyncio.shield(data_queue.get())
+
+        async def battery_handler(_, data):
+            """Battery handler for the BLE client.
+            Args:
+                callback (handler Object): Handler object
+                data (bytes): Battery Level as uint8_t
+            """
+            logging_batterylevel(self.debug, data)
+
+        async def impedance_handler(_, data):
+            """Impedance handler for the BLE client.
+                Data is put in a queue and forwarded to the API.
+
+            Args:
+                callback (handler Object): Handler object
+                data (bytes): Binary data package with impedance values
+            """
+            data_int = int.from_bytes(data, byteorder="little")
+            print(f"[BLE]: Impedance value : {round(data_int/1000,2)} kOhms")
+            if self.write_to_file:
+                self.data_recording_logfile.write(f"{data_int}\n")
+
+            package = {
+                "timestamp": datetime.datetime.now().astimezone().isoformat(),
+                "deviceID": mac_id,
+                "stop": False,
+                "impedance": data_int,
+            }
+            # add the received impedance data to the queue
+            if not data_queue.full():
+                await data_queue.put(package)
+            else:
+                await data_queue.get()
+
+        async def send_start_commands_recording():
+            """Send start commands to the device."""
+            logging_sending_start(self.debug)
+
+            # ------------------ Configuration ------------------
+            if led_sleep:
+                await asyncio.sleep(self.ble_delay)
+                await self.client.write_gatt_char(
+                    self.cfg_id, utf_8_encode(self.led_off_cfg)[0]
+                )
+            # ------------------ Subscribe to notifications ------------------
+            # Notify the client that these two services are required
+            logging_subscribing_eeg_notification(self.debug)
+            await asyncio.sleep(self.ble_delay)
+            await self.client.start_notify(self.meas_eeg_id, data_handler)
+
+            logging_subscribing_battery_notification(self.debug)
+            await asyncio.sleep(self.ble_delay)
+            await self.client.start_notify(self.battery_id, battery_handler)
+
+            # ------------------ Start commands ------------------
+            # sleep so that cleint can respond
+            await asyncio.sleep(self.ble_delay)
+            # send start command for recording data
+            await self.client.write_gatt_char(
+                self.command_id, utf_8_encode(self.start_cmd)[0]
+            )
+
+        async def send_start_commands_impedance():
+            # ----------------- Configuration -----------------
+            if mains_freq_60hz:
+                await asyncio.sleep(self.ble_delay)
+                await self.client.write_gatt_char(
+                    self.cfg_id, utf_8_encode(self.notch_freq_60_cfg)[0]
+                )
+            else:
+                await asyncio.sleep(self.ble_delay)
+                await self.client.write_gatt_char(
+                    self.cfg_id, utf_8_encode(self.notch_freq_50_cfg)[0]
+                )
+
+            # ----------------- Subscribe -----------------
+            logging_subscribing_impedance_notification(self.debug)
+            await asyncio.sleep(self.ble_delay)
+            await self.client.start_notify(self.meas_imp_id, impedance_handler)
+
+            # ----------------- Send start command -----------------
+            logging_starting_impedance_measurement_commands(self.debug)
+            await asyncio.sleep(self.ble_delay)
+            await self.client.write_gatt_char(
+                self.command_id, utf_8_encode(self.start_imp_cmd)[0]
+            )
+
+        async def stop_impedance_timeout():
+            """Stop recording gracefully."""
+            # make sure the last data is now a stop command
+            package = {
+                "timestamp": datetime.datetime.now().astimezone().isoformat(),
+                "deviceID": mac_id,
+                "stop": True,
+            }
+            # ------------------ Load final stop package ------------------
+            if not data_queue.full():
+                await data_queue.put(package)
+            else:
+                await data_queue.get()
+                await data_queue.put(package)
+            logging_sending_stop(self.debug)
+            # ------------------ API should send already loaded package  ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # This gives time for the api to send already loaded data
+            logging_sending_stop_device(self.debug)
+            await asyncio.sleep(self.ble_delay)
+
+            await self.client.write_gatt_char(
+                self.command_id, utf_8_encode(self.stop_imp_cmd)[0]
+            )
+
+            # ------------------ Disconnect command to device ------------------
+            logging_sending_disconnect(self.debug)
+            await asyncio.sleep(self.ble_stop_delay)
+            await self.client.disconnect()
+            await asyncio.sleep(self.ble_stop_delay)
+
+            if self.write_to_file:
+                self.data_recording_logfile.close()
+            logging_recording_successfully_stopped(self.debug)
+
+        async def stop_recording_timeout():
+            """Stop recording gracefully."""
+
+            # make sure the last data is now a stop command
+            package = {
+                "timestamp": datetime.datetime.now().astimezone().isoformat(),
+                "deviceID": mac_id,
+                "data": "STOP_TIMEOUT",
+                "stop": True,
+            }
+            # ------------------ Load final stop package ------------------
+            if not data_queue.full():
+                await data_queue.put(package)
+            else:
+                await data_queue.get()
+                await data_queue.put(package)
+            logging_sending_stop(self.debug)
+            # ------------------ API should send already loaded package  ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # This gives time for the api to send already loaded data
+            logging_sending_stop_device(self.debug)
+            await asyncio.sleep(self.ble_delay)
+
+            await self.client.write_gatt_char(
+                self.command_id, utf_8_encode(self.stop_cmd)[0]
+            )
+
+            if led_sleep:
+                logging_turn_ble_on(self.debug)
+                await asyncio.sleep(self.ble_delay)
+                await self.client.write_gatt_char(
+                    self.cfg_id, utf_8_encode(self.led_on_cfg)[0]
+                )
+            # ------------------ Disconnect command to device ------------------
+            logging_sending_disconnect(self.debug)
+            await asyncio.sleep(self.ble_stop_delay)
+            await self.client.disconnect()
+            await asyncio.sleep(self.ble_stop_delay)
+
+            if self.write_to_file:
+                self.data_recording_logfile.close()
+            logging_recording_successfully_stopped(self.debug)
+
+        async def stop_impedance_cancelled_script():
+            """Stop recording abruptly."""
+            logging_keyboard_interrupt(self.debug)
+
+            # ------------------ Sending final API packages ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # Give API time to send last package
+            # With its own interupt handling
+            # ------------------ Send stop EEG recording command ------------------
+            logging_sending_stop_device(self.debug)
+            await asyncio.sleep(self.ble_delay)
+            await self.client.write_gatt_char(
+                self.command_id, utf_8_encode(self.stop_imp_cmd)[0]
+            )
+
+            # ------------------ Disconnecting commands ------------------
+            logging_sending_disconnect(self.debug)
+            await asyncio.sleep(self.ble_stop_delay)
+            await self.client.disconnect()
+            await asyncio.sleep(self.ble_stop_delay)
+            # ------------------ Closing file  ------------------
+            if self.write_to_file:
+                self.data_recording_logfile.close()
+            logging_recording_successfully_stopped(self.debug)
+            # ------------------ Sending final API packages ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # Give API time to send last package
+            # With its own interupt handling
+
+        async def stop_recording_cancelled_script():
+            """Stop recording abruptly."""
+            logging_keyboard_interrupt(self.debug)
+
+            # ------------------ Sending final API packages ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # Give API time to send last package
+            # With its own interupt handling
+            # ------------------ Send stop EEG recording command ------------------
+            logging_sending_stop_device(self.debug)
+            await asyncio.sleep(self.ble_delay)
+            await self.client.write_gatt_char(
+                self.command_id, utf_8_encode(self.stop_cmd)[0]
+            )
+            # ------------------ Configuring LED back on ------------------
+            if led_sleep:
+                logging_turn_led_on(self.debug)
+                await asyncio.sleep(self.ble_delay)
+                await self.client.write_gatt_char(
+                    self.cfg_id, utf_8_encode(self.led_on_cfg)[0]
+                )
+            # ------------------ Disconnecting commands ------------------
+            logging_sending_disconnect(self.debug)
+            await asyncio.sleep(self.ble_stop_delay)
+            await self.client.disconnect()
+            await asyncio.sleep(self.ble_stop_delay)
+            # ------------------ Closing file  ------------------
+            if self.write_to_file:
+                self.data_recording_logfile.close()
+            logging_recording_successfully_stopped(self.debug)
+            # ------------------ Sending final API packages ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # Give API time to send last package
+            # With its own interupt handling
+
+        async def stop_recording_device_lost():
+            """Stop recording device lost."""
+            logging_device_lost_give_up(self.debug)
+            # ------------------ Sending final API packages ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(self.ble_delay)  # Give API time to send last package
+            # ------------------ Loading last package ------------------
+            logging_sending_stop(self.debug)
+            package = {
+                "timestamp": datetime.datetime.now().astimezone().isoformat(),
+                "deviceID": mac_id,
+                "data": "STOP_DEVICE_LOST",
+                "stop": True,
+            }
+            # pack the stop command
+            if not data_queue.full():
+                await data_queue.put(package)
+            else:
+                await data_queue.get()
+                await data_queue.put(package)
+            # ------------------ Sending final API packages ------------------
+            logging_giving_time_api(self.debug)
+            await asyncio.sleep(
+                self.sent_final_package_time
+            )  # Give API time to send last package
+            # ------------------ Closing file ------------------
+            if self.write_to_file:
+                self.data_recording_logfile.close()
+
+            return True
+
+        async def bluetooth_reconnect():
+            """Set flags to reconnect to bluetooth device."""
+            self.try_to_connect_timeout = self.try_to_connect_timeout - 1
+            if self.try_to_connect_timeout <= 0:
+                self.device_lost = await stop_recording_device_lost()
+            logging_trying_to_connect_again(self.debug, self.try_to_connect_timeout)
+            self.connection_established = False
+            self.initialise_connection = True
+
+        def initialise_file():
+            """Initialise file for recording."""
+            if self.write_to_file:
+                if not os.path.exists("./logs"):
+                    os.makedirs("logs")
+
+                if not impedance_measurement:
+                    measurement_type = "rec"
+                else:
+                    measurement_type = "imp"
+
+                datestr = datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
+                recording_filename = f"./logs/IGEB-{measurement_type}-{datestr}.txt"
+                self.data_recording_logfile = open(
+                    recording_filename, "w", encoding="utf-8"
+                )
+
+        def initialise_timestamps():
+            if self.initial_time:
+                self.initial_time = False  # record that this is the initial time
+                self.original_time = time.time()
+
+        async def main_loop():
+            while True:
+                if self.connection_established:
+
+                    await asyncio.shield(
+                        asyncio.sleep(self.ble_delay)
+                    )  # sleep so that everything can happen
+                    self.remaining_time = record_time - (
+                        time.time() - self.original_time
+                    )
+                    print(f"Time left: {round(self.remaining_time)}s")
+
+                    if self.remaining_time <= 0:
+                        logging_time_reached(self.debug, self.original_time)
+                        if not impedance_measurement:
+                            await stop_recording_timeout()
+                        else:
+                            await stop_impedance_timeout()
+                        break
+
+                else:
+                    break
+
+        # >>>>>>>>>>>>>>>>>>>>> Start of recording process <<<<<<<<<<<<<<<<<<<<<<<<
+        # ------------------ Initialise values for timestamps ------------------
+        self.prev_timestamp = 0
+        self.prev_index = -1
+        # ------------------ Initialise time values for recording timeout ------------------
+        # This has been decoupled from the device timing for robustness
+        self.original_time = time.time()
+        self.initial_time = True
+        self.time_left = True
+        self.initial_time = True
+        # ------------------ Initialise connection values for trying to connect again ------------------
+        self.connection_established = False
+        self.try_to_connect_timeout = self.reconnect_try_amount
+        # ------------------ Initialise log file ------------------
+        initialise_file()
+
+        while True:
+            try:
+                if self.initialise_connection:
+                    self.initialise_connection = False
+                    await self.connect_to_device()
+
+                if self.client.is_connected:
+                    logging_device_connected_general(self.debug)
+
+                    if not impedance_measurement:
+                        await send_start_commands_recording()
+                    else:
+                        await send_start_commands_impedance()
+
+                    logging_recording_started(self.debug)
+                    self.try_to_connect_timeout = (
+                        self.reconnect_try_amount
+                    )  # reset counter
+                    # >>>>>>>>>>>>>>>>>>>>> Main loop <<<<<<<<<<<<<<<<<<<<<<<<
+                    initialise_timestamps()
+                    await asyncio.shield(main_loop())
+                    # >>>>>>>>>>>>>>>>>>>>> Main loop <<<<<<<<<<<<<<<<<<<<<<<<
+
+                if self.remaining_time <= 0:
+                    break
+
+                if not self.connection_established:
+                    logging_disconnected_recognised(self.debug)
+                    await bluetooth_reconnect()
+                    if self.device_lost:
+                        break
+
+            except asyncio.CancelledError:
+                if not impedance_measurement:
+                    await stop_recording_cancelled_script()
+                else:
+                    await stop_impedance_cancelled_script()
+                break
+
+            except Exception as error:
+                logging_ble_client_lost(self.debug, error)
+
+            finally:
+                logging_ensuring_ble_disconnected(self.debug)
+                await asyncio.sleep(self.ble_stop_delay)
+                await self.client.disconnect()
+                await asyncio.sleep(self.ble_stop_delay)
+                self.connection_established = False
+
+        logging_ble_complete(self.debug)
+
+    async def get_service_and_char(self) -> None:
+        """Get the services and characteristics of the device."""
+        try:
+            async with BleakClient(self.address) as client:
+                logging_device_connected_general(self.debug)
+
+                for service in client.services:
+                    logging_device_info_uuid(self.debug, service)
+
+                    for char in service.characteristics:
+                        if "read" in char.properties:
+                            try:
+                                value = bytes(await client.read_gatt_char(char.uuid))
+                            except exc.BleakError as err:
+                                value = str(err).encode()
+                        else:
+                            value = None
+                        logging_device_info_characteristic(self.debug, char, value)
+
+                await asyncio.sleep(self.ble_stop_delay)
+                await client.disconnect()
+                await asyncio.sleep(self.ble_stop_delay)
+                logging_sending_disconnect(self.debug)
+
+        except exc.BleakError as err:
+            logging_device_connection_failed(self.debug, err)
+
+    async def read_battery_level(self) -> None:
+        """Read the battery level of the device given pre-defined interval."""
+        logging_reading_battery_level(self.debug)
+
+        async with BleakClient(self.address) as client:
+            logging_device_connected_general(self.debug)
+
+            try:
+                await asyncio.sleep(self.ble_delay)
+                value = int.from_bytes(
+                    (await client.read_gatt_char(self.battery_id)), byteorder="little"
+                )
+                print("-----------------------------")
+                print(f"\nBattery level: {value}%\n")
+                print("-----------------------------")
+                logging_batterylevel_int(self.debug, value)
+
+                await asyncio.sleep(self.ble_stop_delay)
+                await client.disconnect()
+                await asyncio.sleep(self.ble_stop_delay)
+                logging_sending_disconnect(self.debug)
+
+            except exc.BleakError as err:
+                # log the error
+                logging_device_connection_failed(self.debug, err)
+
+    async def get_device_information(self) -> dict:
+        """Read the device information of the device."""
+
+        device_info = {}
+
+        async with BleakClient(self.address) as client:
+            logging_device_connected_general(self.debug)
+
+            for service in client.services:
+                if service.uuid == self.device_service:
+                    for char in service.characteristics:
+                        if "read" in char.properties:
+                            try:
+                                value = bytes(await client.read_gatt_char(char.uuid))
+                            except exc.BleakError as err:
+                                value = str(err).encode()
+                        else:
+                            value = None
+
+                        print(f"{ char.description}:{str(value)}")
+                        device_info[char.description] = str(value)
+                        logging_device_description_list(self.debug, char, value)
+
+        return device_info
```

### Comparing `idun_guardian_client-1.1b4/src/idun_guardian_client/igeb_utils.py` & `idun_guardian_client-1.1b9/src/idun_guardian_client/igeb_utils.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-"""
-Misc utility functions
-"""
-
-import platform
-
-
-def check_platform():
-    """
-    Check if the script is running on a cross platform
-
-    Returns:
-        bool: True if running on cross platform
-    """
-    if platform.system() == "Darwin":
-        return "Darwin"
-    elif platform.system() == "Linux":
-        return "Linux"
-    elif platform.system() == "Windows":
-        return "Windows"
-    else:
-        raise Exception("Unsupported platform")
-
-
-def check_valid_mac(mac_address: str) -> bool:
-    """Check if mac address is valid
-
-    Args:
-        mac_address (str): Mac address
-
-    Returns:
-        bool: True if mac address is valid
-    """
-    if len(mac_address) != 17:
-        return False
-    if mac_address.count(":") != 5:
-        return False
-    print("Mac address is valid")
-    return True
-
-
-def check_valid_uuid(uuid: str) -> bool:
-    """Check if uuid is valid
-
-    Args:
-        uuid (str): UUID
-    """
-    if len(uuid) != 36:
-        return False
-    if uuid.count("-") != 4:
-        return False
-    return True
-
-
-def unpack_from_queue(package):
-    """Unpack data from the queue filled with BLE data
-
-    Args:
-        package (dict): BLE data package
-
-    Returns:
-        timestamp: Timestamp of the data
-        deviceID: Device ID of the data
-        data: Data from the BLE package
-        stop: Boolean to stop the cloud streaming
-        impedance: Impedance data
-    """
-    # check if "timestamp" is in the package
-    if "timestamp" in package:
-        timestamp = package["timestamp"]
-    else:
-        timestamp = None
-
-    # chek if deviceID is in the package
-    if "deviceID" in package:
-        device_id = package["deviceID"]
-    else:
-        device_id = None
-
-    # check if "data" is in the package
-    if "data" in package:
-        data = package["data"]
-    else:
-        data = None
-
-    # check if "type" is in the package
-    if "stop" in package:
-        stop = package["stop"]
-    else:
-        stop = None
-
-    # check if impedance is in the package
-    if "impedance" in package:
-        impedance = package["impedance"]
-    else:
-        impedance = None
-
-    return (timestamp, device_id, data, stop, impedance)
-
-
-async def unpack_and_load_data(data_model, data_queue):
-    """Get data from the queue and pack it into a dataclass"""
-    package = await data_queue.get()
-    (
-        device_timestamp,
-        device_id,
-        data,
-        stop,
-        impedance,
-    ) = unpack_from_queue(package)
-
-    if data is not None:
-        data_model.payload = data
-    if device_timestamp is not None:
-        data_model.deviceTimestamp = device_timestamp
-    if device_id is not None:
-        data_model.deviceID = device_id
-    if stop is not None:
-        data_model.stop = stop
-    if impedance is not None:
-        data_model.impedance = impedance
-    return data_model, data_queue
+"""
+Misc utility functions
+"""
+
+import platform
+
+
+def check_platform():
+    """
+    Check if the script is running on a cross platform
+
+    Returns:
+        bool: True if running on cross platform
+    """
+    if platform.system() == "Darwin":
+        return "Darwin"
+    elif platform.system() == "Linux":
+        return "Linux"
+    elif platform.system() == "Windows":
+        return "Windows"
+    else:
+        raise Exception("Unsupported platform")
+
+
+def check_valid_mac(mac_address: str) -> bool:
+    """Check if mac address is valid
+
+    Args:
+        mac_address (str): Mac address
+
+    Returns:
+        bool: True if mac address is valid
+    """
+    if len(mac_address) != 17:
+        return False
+    if mac_address.count(":") != 5:
+        return False
+    print("Mac address is valid")
+    return True
+
+
+def check_valid_uuid(uuid: str) -> bool:
+    """Check if uuid is valid
+
+    Args:
+        uuid (str): UUID
+    """
+    if len(uuid) != 36:
+        return False
+    if uuid.count("-") != 4:
+        return False
+    return True
+
+
+def unpack_from_queue(package):
+    """Unpack data from the queue filled with BLE data
+
+    Args:
+        package (dict): BLE data package
+
+    Returns:
+        timestamp: Timestamp of the data
+        deviceID: Device ID of the data
+        data: Data from the BLE package
+        stop: Boolean to stop the cloud streaming
+        impedance: Impedance data
+    """
+    # check if "timestamp" is in the package
+    if "timestamp" in package:
+        timestamp = package["timestamp"]
+    else:
+        timestamp = None
+
+    # chek if deviceID is in the package
+    if "deviceID" in package:
+        device_id = package["deviceID"]
+    else:
+        device_id = None
+
+    # check if "data" is in the package
+    if "data" in package:
+        data = package["data"]
+    else:
+        data = None
+
+    # check if "type" is in the package
+    if "stop" in package:
+        stop = package["stop"]
+    else:
+        stop = None
+
+    # check if impedance is in the package
+    if "impedance" in package:
+        impedance = package["impedance"]
+    else:
+        impedance = None
+
+    return (timestamp, device_id, data, stop, impedance)
+
+
+async def unpack_and_load_data(data_model, data_queue):
+    """Get data from the queue and pack it into a dataclass"""
+    package = await data_queue.get()
+    (
+        device_timestamp,
+        device_id,
+        data,
+        stop,
+        impedance,
+    ) = unpack_from_queue(package)
+
+    if data is not None:
+        data_model.payload = data
+    if device_timestamp is not None:
+        data_model.deviceTimestamp = device_timestamp
+    if device_id is not None:
+        data_model.deviceID = device_id
+    if stop is not None:
+        data_model.stop = stop
+    if impedance is not None:
+        data_model.impedance = impedance
+    return data_model, data_queue
```

### Comparing `idun_guardian_client-1.1b4/src/idun_guardian_client/test_producer_consumer.py` & `idun_guardian_client-1.1b9/src/idun_guardian_client/test_producer_consumer.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import asyncio, random
-
-
-async def rnd_sleep(t):
-    # sleep for T seconds on average
-    await asyncio.sleep(t * random.random() * 2)
-
-
-async def producer(queue):
-    while True:
-        # produce a token and send it to a consumer
-        token = random.random()
-        print(f"produced {token}")
-        if token < 0.05:
-            break
-        await queue.put(token)
-        await rnd_sleep(0.1)
-
-
-async def consumer(queue):
-    while True:
-        token = await queue.get()
-        # process the token received from a producer
-        await rnd_sleep(0.3)
-        queue.task_done()
-        print(f"consumed {token}")
-
-
-async def main():
-    queue = asyncio.Queue()
-
-    # fire up the both producers and consumers
-    producers = [asyncio.create_task(producer(queue)) for _ in range(3)]
-    consumers = [asyncio.create_task(consumer(queue)) for _ in range(10)]
-
-    # with both producers and consumers running, wait for
-    # the producers to finish
-    await asyncio.gather(*producers)
-    print("---- done producing")
-
-    # wait for the remaining tasks to be processed
-    await queue.join()
-
-    # cancel the consumers, which are now idle
-    for c in consumers:
-        c.cancel()
-
-
-asyncio.run(main())
+import asyncio, random
+
+
+async def rnd_sleep(t):
+    # sleep for T seconds on average
+    await asyncio.sleep(t * random.random() * 2)
+
+
+async def producer(queue):
+    while True:
+        # produce a token and send it to a consumer
+        token = random.random()
+        print(f"produced {token}")
+        if token < 0.05:
+            break
+        await queue.put(token)
+        await rnd_sleep(0.1)
+
+
+async def consumer(queue):
+    while True:
+        token = await queue.get()
+        # process the token received from a producer
+        await rnd_sleep(0.3)
+        queue.task_done()
+        print(f"consumed {token}")
+
+
+async def main():
+    queue = asyncio.Queue()
+
+    # fire up the both producers and consumers
+    producers = [asyncio.create_task(producer(queue)) for _ in range(3)]
+    consumers = [asyncio.create_task(consumer(queue)) for _ in range(10)]
+
+    # with both producers and consumers running, wait for
+    # the producers to finish
+    await asyncio.gather(*producers)
+    print("---- done producing")
+
+    # wait for the remaining tasks to be processed
+    await queue.join()
+
+    # cancel the consumers, which are now idle
+    for c in consumers:
+        c.cancel()
+
+
+asyncio.run(main())
```

### Comparing `idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/PKG-INFO` & `idun_guardian_client-1.1b9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,268 +1,268 @@
-Metadata-Version: 2.1
-Name: idun-guardian-client
-Version: 1.1b4
-Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
-Author-email: IDUN Technologies <contact@iduntechnologies.com>
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: Other/Proprietary License
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Natural Language :: English
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
-# User guide and documentation
-
-## What can you do with the Python SDK?
-
-1. You can use the Python SDK to search for the device.
-2. You can use the Python SDK to connect and record data from the earbud.
-3. You can download the data to your local machine.
-
----
-
-## Prerequisites
-
-- [Python 3.10](https://www.python.org/downloads/release/python-3100), if you already have another python version installed and you do not want to create a virtual environment to run the SDK, then you have to install Python 3.10 and [set it as your default Python](https://www.youtube.com/watch?v=zriWqGNJg4k).
-    - If you have conflicts with other packages when installing the Python SDK:
-        -  Use [Conda](https://www.anaconda.com/products/distribution) which will create an environment and configure your python version to the correct one with the following command: 
-        
-        ```bash
-        conda create -n idun_env python=3.10
-        ```
-        or
-        - Use [Pipenv](https://pypi.org/project/pipenv/) which will create your virtual environment manually using the following command.
-        ```bash
-        pipenv install --python 3.10
-        ```
----
-
-## Quick installation guide
-
-1. Create a new repository or folder
-2. Open the terminal in the same folder location or direct to that location within an already open terminal. For Windows you can use command prompt or Anaconda prompt, and Mac OS you can use the terminal or Anaconda prompt.
-
-3. First activate the virtual environment if you have created one by using the following command, this command must always be run before using the python SDK:
-    ```bash
-    conda activate idun_env
-    ```
-    or
-    ```bash
-    pipenv shell
-    ```
-
-4. After the environment is activated, install the Python SDK using the following command:
-    - With a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) use the following command:
-    ```bash
-    pip install idun-guardian-client
-    ```
-    or
-    - With a [pipenv environment](https://pypi.org/project/pipenv/) use the following command:
-    ```bash
-    pipenv install idun-guardian-client
-    ```
-
-5. After installing the package, make sure that the dependencies are correctly installed by running the following command and inspecting the packages installed in the terminal output:
-
-    ```bash
-    pip list
-    ```
-
----
-
-## How to use the Python SDK
-
-You can also download all the SDK example files from our [GitHub repository](https://github.com/iduntech/idun-guardian-client-examples.git), or copy and paste it from the examples below.
-
-### Example 1: Search for the device
-
-1. Create a new file inside the folder where you created your environment and name it `search.py`
-2. Open the terminal in the folder and activate your virtual environment using the steps from the [Quick installation guide](#quick-installation-guide).
-3. Open the `search.py` file and copy the code from step 1 below.
-4. Activate the virtual environment **only** if you have not already done so by using:
-
-    ```bash
-    conda activate idun_env
-    ```
-    or
-    ```bash
-    pipenv shell
-    ```
-4. Run the following command in the terminal to run the code after you have activate the enviroment:
-    ```bash
-    python search.py
-    ```
-
-#### Recommendation of steps to follow which is elaborated further below
-
-1. Search for the device
-2. Check the battery level
-3. Check the impedance
-4. Record data from the earbud
-5. Download the data from the cloud using the recording ID
-
-### **1. Search the earbud manually**
-
-- To search for the earbud, you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-bci = GuardianClient()
-
-device_address = asyncio.run(bci.search_device())
-```
-
-- Follow the steps in the terminal to search for the earbud with the name `IGEB`
-- If there are more than one IGEB device in the area, you will be asked to select the device you want to connect to connect to, a list such as below will pop up in the terminal:
-
-    - For Windows:
-    ```bash
-    ----- Available devices -----
-
-    Index | Name | Address
-    ----------------------------
-    0     | IGEB | XX:XX:XX:XX:XX:XX
-    1     | IGEB | XX:XX:XX:XX:XX:XX
-    2     | IGEB | XX:XX:XX:XX:XX:XX
-    ----------------------------
-    ```
-    - For Mac OS:
-    ```bash
-    ----- Available devices -----
-    Index | Name | UUID
-    ----------------------------
-    0    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
-    1    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
-    2    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
-    ----------------------------
-    ```
-
-- Enter the index number of the device you want to connect to.
-
-
-### **2. Check battery level**
-
-- To read out the battery level, you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-bci = GuardianClient()
-bci.address = asyncio.run(bci.search_device())
-
-asyncio.run(bci.start_battery())
-```
-
-### **3. Check impedance values**
-
-- To read out the impedance values, you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-IMPEDANCE_DURATION = 5  # duration of impedance measurement in seconds
-MAINS_FREQUENCY_60Hz = False
-# mains frequency in Hz (50 or 60), for Europe 50Hz, for US 60Hz
-
-
-# Get device address
-bci = GuardianClient()
-bci.address = asyncio.run(bci.search_device())
-
-# start a recording session
-asyncio.run(
-    bci.start_recording(
-        recording_timer=IMPEDANCE_DURATION,
-        mains_freq_60hz=MAINS_FREQUENCY_60Hz,
-        impedance_measurement=True)
-)
-```
-
-### **4. Start a recording**
-
-- To start a recording with a pre-defined timer (e.g. `100` in seconds), you need to run the following command in your python shell or in your python script:
-
-```python
-import asyncio
-from idun_guardian_client import GuardianClient
-
-EXPERIMENT: str = "Sleeping"
-RECORDING_TIMER: int = 36000 # 10 hours in seconds
-LED_SLEEP: bool = False
-SENDING_TIMEOUT: float = 2 # No sending receipt time before interrupt
-BI_DIRECTIONAL_TIMEOUT: float = 20 # No bi-directional data receiving before interrupt
-
-# start a recording session
-bci = GuardianClient()
-bci.address = asyncio.run(bci.search_device())
-
-# start a recording session
-asyncio.run(
-    bci.start_recording(
-        recording_timer=RECORDING_TIMER,
-        led_sleep=LED_SLEEP,
-        experiment=EXPERIMENT,
-        sending_timout=SENDING_TIMEOUT,
-        bi_directional_receiving_timeout=BI_DIRECTIONAL_TIMEOUT,
-    )
-)
-
-```
-
-- To stop the recording, either wait for the timer to run out or interrupt the recording
-    - with Mac OS enter the cancellation command in the terminal running the script, this would be `Ctrl+.` or `Ctrl+C`
-    - with Windows enter the cancellation command in the terminal running the script, this would be `Ctrl+C` or `Ctrl+Shift+C`
-
-### **4. Get all recorded info**
-
-- To download the data, you need to first get the list of all your recordings and choose the one you would like to download
-- Run the following command in your python shell or in your python script:
-
-```python
-from idun_guardian_client.igeb_api import GuardianAPI
-
-api = GuardianAPI()
-
-# get a list of all recordings
-recording_list = api.get_recordings_info_all(device_id = "XX-XX-XX-XX-XX-XX") # Device ID is derived from the MAC address of the earbud and in the log file
-
-```
-
-### **5. Get recording info**
-
-- To list the information on a specific recording, you need to run the following command in your python shell or in your python script:
-
-```python
-from idun_guardian_client.igeb_api import GuardianAPI
-
-api = GuardianAPI()
-
-# get single recording
-api.get_recording_info_by_id(
-    device_id = "XX-XX-XX-XX-XX-XX",
-    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
-)
-
-```
-
-### **5. Download recording**
-
-- To download the data insert the `device_id` along with the `recording_id` and run the following command in your python shell or in your python script
-
-```python
-from idun_guardian_client.igeb_api import GuardianAPI
-
-api = GuardianAPI()
-
-# download recording
-api.download_recording_by_id(
-    device_id = "XX-XX-XX-XX-XX-XX",
-    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxx"
-)
-# The info about th recording can be found in the log file
-```
+Metadata-Version: 2.1
+Name: idun_guardian_client
+Version: 1.1b9
+Summary: Python SDK for communication with the IDUN Guardian earbuds and IDUN cloud
+Author-email: IDUN Technologies <contact@iduntechnologies.com>
+Classifier: Development Status :: 1 - Planning
+Classifier: License :: Other/Proprietary License
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Natural Language :: English
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
+# User guide and documentation
+
+## What can you do with the Python SDK?
+
+1. You can use the Python SDK to search for the device.
+2. You can use the Python SDK to connect and record data from the earbud.
+3. You can download the data to your local machine.
+
+---
+
+## Prerequisites
+
+- [Python 3.10](https://www.python.org/downloads/release/python-3100), if you already have another python version installed and you do not want to create a virtual environment to run the SDK, then you have to install Python 3.10 and [set it as your default Python](https://www.youtube.com/watch?v=zriWqGNJg4k).
+    - If you have conflicts with other packages when installing the Python SDK:
+        -  Use [Conda](https://www.anaconda.com/products/distribution) which will create an environment and configure your python version to the correct one with the following command: 
+        
+        ```bash
+        conda create -n idun_env python=3.10
+        ```
+        or
+        - Use [Pipenv](https://pypi.org/project/pipenv/) which will create your virtual environment manually using the following command.
+        ```bash
+        pipenv install --python 3.10
+        ```
+---
+
+## Quick installation guide
+
+1. Create a new repository or folder
+2. Open the terminal in the same folder location or direct to that location within an already open terminal. For Windows you can use command prompt or Anaconda prompt, and Mac OS you can use the terminal or Anaconda prompt.
+
+3. First activate the virtual environment if you have created one by using the following command, this command must always be run before using the python SDK:
+    ```bash
+    conda activate idun_env
+    ```
+    or
+    ```bash
+    pipenv shell
+    ```
+
+4. After the environment is activated, install the Python SDK using the following command:
+    - With a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) use the following command:
+    ```bash
+    pip install idun-guardian-client
+    ```
+    or
+    - With a [pipenv environment](https://pypi.org/project/pipenv/) use the following command:
+    ```bash
+    pipenv install idun-guardian-client
+    ```
+
+5. After installing the package, make sure that the dependencies are correctly installed by running the following command and inspecting the packages installed in the terminal output:
+
+    ```bash
+    pip list
+    ```
+
+---
+
+## How to use the Python SDK
+
+You can also download all the SDK example files from our [GitHub repository](https://github.com/iduntech/idun-guardian-client-examples.git), or copy and paste it from the examples below.
+
+### Example 1: Search for the device
+
+1. Create a new file inside the folder where you created your environment and name it `search.py`
+2. Open the terminal in the folder and activate your virtual environment using the steps from the [Quick installation guide](#quick-installation-guide).
+3. Open the `search.py` file and copy the code from step 1 below.
+4. Activate the virtual environment **only** if you have not already done so by using:
+
+    ```bash
+    conda activate idun_env
+    ```
+    or
+    ```bash
+    pipenv shell
+    ```
+4. Run the following command in the terminal to run the code after you have activate the enviroment:
+    ```bash
+    python search.py
+    ```
+
+#### Recommendation of steps to follow which is elaborated further below
+
+1. Search for the device
+2. Check the battery level
+3. Check the impedance
+4. Record data from the earbud
+5. Download the data from the cloud using the recording ID
+
+### **1. Search the earbud manually**
+
+- To search for the earbud, you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+bci = GuardianClient()
+
+device_address = asyncio.run(bci.search_device())
+```
+
+- Follow the steps in the terminal to search for the earbud with the name `IGEB`
+- If there are more than one IGEB device in the area, you will be asked to select the device you want to connect to connect to, a list such as below will pop up in the terminal:
+
+    - For Windows:
+    ```bash
+    ----- Available devices -----
+
+    Index | Name | Address
+    ----------------------------
+    0     | IGEB | XX:XX:XX:XX:XX:XX
+    1     | IGEB | XX:XX:XX:XX:XX:XX
+    2     | IGEB | XX:XX:XX:XX:XX:XX
+    ----------------------------
+    ```
+    - For Mac OS:
+    ```bash
+    ----- Available devices -----
+    Index | Name | UUID
+    ----------------------------
+    0    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
+    1    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
+    2    | IGEB | XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
+    ----------------------------
+    ```
+
+- Enter the index number of the device you want to connect to.
+
+
+### **2. Check battery level**
+
+- To read out the battery level, you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+bci = GuardianClient()
+bci.address = asyncio.run(bci.search_device())
+
+asyncio.run(bci.start_battery())
+```
+
+### **3. Check impedance values**
+
+- To read out the impedance values, you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+IMPEDANCE_DURATION = 5  # duration of impedance measurement in seconds
+MAINS_FREQUENCY_60Hz = False
+# mains frequency in Hz (50 or 60), for Europe 50Hz, for US 60Hz
+
+
+# Get device address
+bci = GuardianClient()
+bci.address = asyncio.run(bci.search_device())
+
+# start a recording session
+asyncio.run(
+    bci.start_recording(
+        recording_timer=IMPEDANCE_DURATION,
+        mains_freq_60hz=MAINS_FREQUENCY_60Hz,
+        impedance_measurement=True)
+)
+```
+
+### **4. Start a recording**
+
+- To start a recording with a pre-defined timer (e.g. `100` in seconds), you need to run the following command in your python shell or in your python script:
+
+```python
+import asyncio
+from idun_guardian_client import GuardianClient
+
+EXPERIMENT: str = "Sleeping"
+RECORDING_TIMER: int = 36000 # 10 hours in seconds
+LED_SLEEP: bool = False
+SENDING_TIMEOUT: float = 2 # No sending receipt time before interrupt
+BI_DIRECTIONAL_TIMEOUT: float = 20 # No bi-directional data receiving before interrupt
+
+# start a recording session
+bci = GuardianClient()
+bci.address = asyncio.run(bci.search_device())
+
+# start a recording session
+asyncio.run(
+    bci.start_recording(
+        recording_timer=RECORDING_TIMER,
+        led_sleep=LED_SLEEP,
+        experiment=EXPERIMENT,
+        sending_timout=SENDING_TIMEOUT,
+        bi_directional_receiving_timeout=BI_DIRECTIONAL_TIMEOUT,
+    )
+)
+
+```
+
+- To stop the recording, either wait for the timer to run out or interrupt the recording
+    - with Mac OS enter the cancellation command in the terminal running the script, this would be `Ctrl+.` or `Ctrl+C`
+    - with Windows enter the cancellation command in the terminal running the script, this would be `Ctrl+C` or `Ctrl+Shift+C`
+
+### **4. Get all recorded info**
+
+- To download the data, you need to first get the list of all your recordings and choose the one you would like to download
+- Run the following command in your python shell or in your python script:
+
+```python
+from idun_guardian_client.igeb_api import GuardianAPI
+
+api = GuardianAPI()
+
+# get a list of all recordings
+recording_list = api.get_recordings_info_all(device_id = "XX-XX-XX-XX-XX-XX") # Device ID is derived from the MAC address of the earbud and in the log file
+
+```
+
+### **5. Get recording info**
+
+- To list the information on a specific recording, you need to run the following command in your python shell or in your python script:
+
+```python
+from idun_guardian_client.igeb_api import GuardianAPI
+
+api = GuardianAPI()
+
+# get single recording
+api.get_recording_info_by_id(
+    device_id = "XX-XX-XX-XX-XX-XX",
+    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
+)
+
+```
+
+### **5. Download recording**
+
+- To download the data insert the `device_id` along with the `recording_id` and run the following command in your python shell or in your python script
+
+```python
+from idun_guardian_client.igeb_api import GuardianAPI
+
+api = GuardianAPI()
+
+# download recording
+api.download_recording_by_id(
+    device_id = "XX-XX-XX-XX-XX-XX",
+    recording_id = "xxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxx"
+)
+# The info about th recording can be found in the log file
+```
```

### Comparing `idun_guardian_client-1.1b4/src/idun_guardian_client.egg-info/SOURCES.txt` & `idun_guardian_client-1.1b9/src/idun_guardian_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idun_guardian_client-1.1b4/tests/test_utils.py` & `idun_guardian_client-1.1b9/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from idun_guardian_client import igeb_utils
-
-
-def test_check_platform():
-    """
-    GIVEN None
-    WHEN check_platform is called
-    THEN a string is returned
-    """
-
-    import platform
-
-    assert isinstance(igeb_utils.check_platform(), str)
-    assert platform.system() == igeb_utils.check_platform()
-
-
-def test_check_valid_mac():
-    """
-    GIVEN a string
-    WHEN check_valid_mac is called
-    THEN a boolean is returned
-    """
-    assert isinstance(igeb_utils.check_valid_mac("00:00:00:00:00:00"), bool)
-    assert igeb_utils.check_valid_mac("00000000-0000-0000-0000-000000000000") == False
-
-
-def test_check_valid_uuid():
-    """
-    GIVEN a string
-    WHEN check_valid_uuid is called
-    THEN a boolean is returned
-    """
-    assert isinstance(
-        igeb_utils.check_valid_uuid("00000000-0000-0000-0000-000000000000"), bool
-    )
-    assert igeb_utils.check_valid_uuid("00:00:00:00:00:00") == False
-
-
-def generate_mock_data_array():
-    """
-    GIVEN None
-    WHEN generate_mock_data is called
-    THEN a dict is returned
-    """
-    assert isinstance(igeb_utils.generate_mock_data(), dict)
+from idun_guardian_client import igeb_utils
+
+
+def test_check_platform():
+    """
+    GIVEN None
+    WHEN check_platform is called
+    THEN a string is returned
+    """
+
+    import platform
+
+    assert isinstance(igeb_utils.check_platform(), str)
+    assert platform.system() == igeb_utils.check_platform()
+
+
+def test_check_valid_mac():
+    """
+    GIVEN a string
+    WHEN check_valid_mac is called
+    THEN a boolean is returned
+    """
+    assert isinstance(igeb_utils.check_valid_mac("00:00:00:00:00:00"), bool)
+    assert igeb_utils.check_valid_mac("00000000-0000-0000-0000-000000000000") == False
+
+
+def test_check_valid_uuid():
+    """
+    GIVEN a string
+    WHEN check_valid_uuid is called
+    THEN a boolean is returned
+    """
+    assert isinstance(
+        igeb_utils.check_valid_uuid("00000000-0000-0000-0000-000000000000"), bool
+    )
+    assert igeb_utils.check_valid_uuid("00:00:00:00:00:00") == False
+
+
+def generate_mock_data_array():
+    """
+    GIVEN None
+    WHEN generate_mock_data is called
+    THEN a dict is returned
+    """
+    assert isinstance(igeb_utils.generate_mock_data(), dict)
```

