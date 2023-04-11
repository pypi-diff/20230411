# Comparing `tmp/dcentralab_qa_infra_automation-0.1.1.tar.gz` & `tmp/dcentralab_qa_infra_automation-0.1.2.tar.gz`

## Comparing `dcentralab_qa_infra_automation-0.1.1.tar` & `dcentralab_qa_infra_automation-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/.idea/.gitignore
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/.idea/packaging.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/.idea/workspace.xml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/__init__.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/data/read_data.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/SetupDriverWithMetamaskExtension.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/.gitignore
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/misc.xml
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/packaging.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/__init__.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/data/read_data.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/Loggers.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/ReportLoggers.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/utils/WalletsActionsInterface.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/utils/enum/HTTPStatusCodes.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/utils/enum/NetworkTypes.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/utils/enum/Wallets.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/LICENSE
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/README.md
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 dcentralab_qa_infra_automation-0.1.2/PKG-INFO
```

### Comparing `dcentralab_qa_infra_automation-0.1.1/.idea/workspace.xml` & `dcentralab_qa_infra_automation-0.1.2/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/.idea/inspectionProfiles/Project_Default.xml` & `dcentralab_qa_infra_automation-0.1.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/data/read_data.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/data/read_data.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/drivers/BraveDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/drivers/ChromeDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/drivers/HelperFunctions.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/CreateTargetDirectory.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/HtmlReports.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/InitGlobalParameters.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/Loggers.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/Loggers.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/OpenSiteWithCRXExtension.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import pytest
 from dcentralab_qa_infra_automation.infra.CustomEventListener import CustomEventListener
 from selenium.webdriver.support.event_firing_webdriver import EventFiringWebDriver
-from webdriver_manager.chrome import ChromeDriverManager
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options as ChromeOptions
 from dcentralab_qa_infra_automation.drivers import ChromeDriver, BraveDriver
 
 """
 open site with extension via CRX. to any browser type.
 
 @Author: Efrat Cohen
 @Date: 12.2022
@@ -18,47 +15,27 @@
     """
     get crx extension file, setup driver - open the site with extension.
     store the driver to use him in different fixtures and pages.
     if brave browser injected - add the option to driver initialization
     :param request: the requesting test context
     """
     pytest.logger.info("Test: " + request.node.nodeid + " is started ")
-    # chrome_options = ChromeOptions()
-    # # In metamask wallet type
-    # if pytest.data_driven.get("wallet_type") == 'MetaMask':
-    #     chrome_options.add_extension(pytest.user_dir + pytest.properties.get("metamask.extension.crx"))
-    # elif pytest.data_driven.get("wallet_type") == 'Coinbase':
-    #     chrome_options.add_extension(pytest.user_dir + pytest.properties.get("coinbase.extension.crx"))
-
     # Init driver with extension based on injected driver type
     if pytest.data_driven.get("browser") == "brave":
         pytest.logger.info("brave browser type injected, initialize brave browser")
         driver = BraveDriver.initBraveDriverWithExtension()
     elif pytest.data_driven.get("browser") == "chrome":
         pytest.logger.info("chrome driver type injected, initialize chrome browser")
         driver = ChromeDriver.initChromeDriverWithExtension()
 
     # If no driver type injected - chrome is the default
     else:
         pytest.logger.info("no browser type injected, initialize default chrome browser")
         driver = ChromeDriver.initChromeDriverWithExtension()
 
-
-        # # On macOS - use mac brave path
-        # if pytest.data_driven.get("OS") == "windows":
-        #     chrome_options.binary_location = pytest.properties.get("brave.windows.path")
-        #     # On windowsOS - use windows brave path
-        # elif pytest.data_driven.get("OS") == "mac":
-        #     chrome_options.binary_location = pytest.properties.get("brave.mac.path")
-        #     # If no OS injected
-        # else:
-        #     pytest.logger.info("no OS type injected, brave did not add to chrome.")
-
-    # driver = webdriver.Chrome(ChromeDriverManager().install(), options=chrome_options)
-
     # Add event listener
     event_listener = CustomEventListener()
     event_firing_driver = EventFiringWebDriver(driver, event_listener)
 
     pytest.logger.info("driver :" + event_firing_driver.name + " had installed successfully")
     driver.maximize_window()
     pytest.logger.info("window had maximize")
```

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/ParameterInjection.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/Screenshot.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/fixtures/SetupDriver.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/infra/CustomEventListener.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py` & `dcentralab_qa_infra_automation-0.1.2/src/dcentralab_qa_infra_automation/utils/HTTPMethods.py`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/LICENSE` & `dcentralab_qa_infra_automation-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dcentralab_qa_infra_automation-0.1.1/pyproject.toml` & `dcentralab_qa_infra_automation-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcentralab_qa_infra_automation"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Efrat Cohen", email="efrat.cohen@verisoft.co" },
 ]
 description = "Selenium Python Framework developed by veriSoft"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dcentralab_qa_infra_automation-0.1.1/PKG-INFO` & `dcentralab_qa_infra_automation-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentralab_qa_infra_automation
-Version: 0.1.1
+Version: 0.1.2
 Summary: Selenium Python Framework developed by veriSoft
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Efrat Cohen <efrat.cohen@verisoft.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

