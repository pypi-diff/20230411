# Comparing `tmp/mozark_sdk-0.4.tar.gz` & `tmp/mozark-sdk-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozark_sdk-0.4.tar", last modified: Wed Dec 28 11:17:49 2022, max compression
+gzip compressed data, was "mozark-sdk-0.5.tar", last modified: Tue Apr 11 06:32:40 2023, max compression
```

## Comparing `mozark_sdk-0.4.tar` & `mozark-sdk-0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sumitkumargupta   (501) staff       (20)        0 2022-12-28 11:17:49.729912 mozark_sdk-0.4/
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)     1062 2022-12-27 13:24:43.000000 mozark_sdk-0.4/LICENSE.txt
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)      842 2022-12-28 11:17:49.730000 mozark_sdk-0.4/PKG-INFO
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)      730 2022-12-28 06:55:45.000000 mozark_sdk-0.4/README.md
-drwxr-xr-x   0 sumitkumargupta   (501) staff       (20)        0 2022-12-28 11:17:49.728910 mozark_sdk-0.4/mozark_sdk/
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)        0 2022-12-26 05:13:05.000000 mozark_sdk-0.4/mozark_sdk/__init__.py
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)    29794 2022-12-28 10:49:23.000000 mozark_sdk-0.4/mozark_sdk/client.py
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)     2813 2022-12-28 02:05:16.000000 mozark_sdk-0.4/mozark_sdk/device.py
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)     7142 2022-12-28 10:50:58.000000 mozark_sdk-0.4/mozark_sdk/executetest.py
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)     6381 2022-12-28 07:55:38.000000 mozark_sdk-0.4/mozark_sdk/file.py
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)     1548 2022-12-28 07:01:28.000000 mozark_sdk-0.4/mozark_sdk/project.py
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)      778 2022-12-26 05:13:42.000000 mozark_sdk-0.4/mozark_sdk/schedule.py
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)     8181 2022-12-27 09:58:21.000000 mozark_sdk-0.4/mozark_sdk/testanalytics.py
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)     4621 2022-12-28 02:40:26.000000 mozark_sdk-0.4/mozark_sdk/tray.py
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)      947 2022-12-27 05:33:27.000000 mozark_sdk-0.4/mozark_sdk/user.py
-drwxr-xr-x   0 sumitkumargupta   (501) staff       (20)        0 2022-12-28 11:17:49.729769 mozark_sdk-0.4/mozark_sdk.egg-info/
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)      842 2022-12-28 11:17:49.000000 mozark_sdk-0.4/mozark_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)      430 2022-12-28 11:17:49.000000 mozark_sdk-0.4/mozark_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)        1 2022-12-28 11:17:49.000000 mozark_sdk-0.4/mozark_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)       37 2022-12-28 11:17:49.000000 mozark_sdk-0.4/mozark_sdk.egg-info/requires.txt
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)       11 2022-12-28 11:17:49.000000 mozark_sdk-0.4/mozark_sdk.egg-info/top_level.txt
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)       79 2022-12-28 11:17:49.730229 mozark_sdk-0.4/setup.cfg
--rw-r--r--   0 sumitkumargupta   (501) staff       (20)     1361 2022-12-28 11:17:00.000000 mozark_sdk-0.4/setup.py
+drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-04-11 06:32:40.627141 mozark-sdk-0.5/
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     1062 2023-04-01 18:14:03.000000 mozark-sdk-0.5/LICENSE.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      842 2023-04-11 06:32:40.627141 mozark-sdk-0.5/PKG-INFO
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     7542 2023-04-01 18:14:03.000000 mozark-sdk-0.5/README.md
+drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-04-11 06:32:40.623141 mozark-sdk-0.5/mozark-sdk/
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)        0 2023-04-01 18:14:03.000000 mozark-sdk-0.5/mozark-sdk/__init__.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    39744 2023-04-06 08:34:52.000000 mozark-sdk-0.5/mozark-sdk/client.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     4737 2023-04-05 09:59:13.000000 mozark-sdk-0.5/mozark-sdk/device.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    17986 2023-04-06 08:38:18.000000 mozark-sdk-0.5/mozark-sdk/executetest.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    11228 2023-04-05 06:30:41.000000 mozark-sdk-0.5/mozark-sdk/file.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     3926 2023-04-01 18:14:03.000000 mozark-sdk-0.5/mozark-sdk/project.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      778 2023-04-01 18:14:03.000000 mozark-sdk-0.5/mozark-sdk/schedule.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)    31570 2023-04-01 18:14:03.000000 mozark-sdk-0.5/mozark-sdk/test_analytics.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     6704 2023-04-01 18:14:03.000000 mozark-sdk-0.5/mozark-sdk/tray.py
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      877 2023-04-01 18:14:03.000000 mozark-sdk-0.5/mozark-sdk/user.py
+drwxrwxr-x   0 ashwin    (1000) ashwin    (1000)        0 2023-04-11 06:32:40.627141 mozark-sdk-0.5/mozark_sdk.egg-info/
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      842 2023-04-11 06:32:40.000000 mozark-sdk-0.5/mozark_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)      431 2023-04-11 06:32:40.000000 mozark-sdk-0.5/mozark_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)        1 2023-04-11 06:32:40.000000 mozark-sdk-0.5/mozark_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       37 2023-04-11 06:32:40.000000 mozark-sdk-0.5/mozark_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       11 2023-04-11 06:32:40.000000 mozark-sdk-0.5/mozark_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)       79 2023-04-11 06:32:40.627141 mozark-sdk-0.5/setup.cfg
+-rw-rw-r--   0 ashwin    (1000) ashwin    (1000)     1481 2023-04-11 06:28:39.000000 mozark-sdk-0.5/setup.py
```

### Comparing `mozark_sdk-0.4/LICENSE.txt` & `mozark-sdk-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mozark_sdk-0.4/PKG-INFO` & `mozark-sdk-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mozark_sdk
-Version: 0.4
+Name: mozark-sdk
+Version: 0.5
 Summary: Automation test APIs
 Home-page: https://mozark.ai
 Author: Mozark
 Author-email: mozark-aws-staging@mozark.ai
 License: MIT
 Keywords: MOZARK,AUTOMATION,EXPERIENCE
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mozark_sdk-0.4/mozark_sdk/client.py` & `mozark-sdk-0.5/mozark-sdk/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import configparser
 from pathlib import Path
 
+from mozark_sdk.user import User
+from mozark_sdk.project import Project
 from mozark_sdk.file import File
-from mozark_sdk.executetest import TestExecute
 from mozark_sdk.device import Device
-from mozark_sdk.testanalytics import TestAnalytics
-
-import requests
-
-from mozark_sdk.project import Project
 from mozark_sdk.tray import Tray
+from mozark_sdk.executetest import TestExecute
+from mozark_sdk.test_analytics import TestAnalytics
 
 
 class Client:
     config = None
 
     def __init__(self):
         self.set_config()
@@ -22,93 +20,78 @@
         config = configparser.ConfigParser()
         config_file = Path.home() / ".mozark" / "config"
         config.read(config_file)
         api_url = config.get("default", "MOZARK_APP_TESTING_URL")
         username = config.get("default", "MOZARK_APP_TESTING_USERNAME")
         password = config.get("default", "MOZARK_APP_TESTING_PASSWORD")
         client_id = config.get("default", "MOZARK_APP_TESTING_CLIENTID")
-        config = {"username": username, "password": password, "api_url": api_url, "client_id": client_id}
-        print(str(config))
+        base_download_dir = config.get("default", "BASE_DOWNLOAD_DIR")
+        config = {"username": username, "password": password, "api_url": api_url, "client_id": client_id,
+                  "base_download_dir": base_download_dir}
         self.config = config
 
     def get_config(self):
         return self.config
 
     def login(self):
-        new_headers = {'X-Amz-Target': 'AWSCognitoIdentityProviderService.InitiateAuth',
-                       'Content-Type': 'application/x-amz-json-1.1'}
-
-        login_url = "https://cognito-idp.ap-south-1.amazonaws.com/"
-        print(login_url)
-        data = {
-            "AuthParameters": {
-                "USERNAME": self.config.get("username"),
-                "PASSWORD": self.config.get("password")
-            },
-            "AuthFlow": "USER_PASSWORD_AUTH",
-            "ClientId": self.config.get("client_id")
-        }
-        print(str(data))
-        resp = requests.post(login_url, json=data, headers=new_headers)
-        api_access_token = resp.json()['AuthenticationResult']['IdToken']
+        user = User(self)
+        api_access_token = user.login()
         self.config["api_access_token"] = api_access_token
-        print(str(self.config))
 
     def logout(self):
-        pass
+        self.config["api_access_token"] = ""
 
     # Project
 
     def create_project(self, project_name=None, project_description=None):
         """Create a new project
         Args:
             project_name (str): unique project name
             project_description (str): short description for a project
 
         Returns:
             message (str): 'Success' if successful, 'Failure' along with failure reason
 
             "Failure: Project with `{project_name}` already exists." - in case if project with the given name already exists
         """
-        project = Project()
-        status_message = project.create_project(project, project_name, project_description)
+        project = Project(self)
+        status_message = project.create_project(project_name, project_description)
         return status_message
-        # pass
 
     def get_project_info(self, project_name=None):
         """ Returns project information -
         Args:
             project_name (str): project name
 
         Returns:
             project (dict): contains projectName, projectDescription, and unique ID
             {
                 "projectName": "",
                 "projectDescription": "",
                 "projectUUID": ""
             }
+
+            errorMessage (str): 'Failure: Project with name `{project_name}` not found.'
         """
-        project = Project()
-        status_message = project.get_projects(project, project_name)
+        project = Project(self)
+        status_message = project.get_project_info(project_name=project_name)
         return status_message
-        # pass
 
-    # def rename_project(self, project_name_old=None, project_name_new=None):
-    #     pass
+    def delete_project(self, project_name=None):
+        """ Delete project with given project name
 
-    # def delete_project(self, project_name=None):
-    #     """ Delete project with given project name
-    #
-    #     Args:
-    #         project_name (str): project name
-    #
-    #     Returns:
-    #         message (str): 'Success' if successful, 'Failure' along with failure reason
-    #     """
-    #     pass
+        Args:
+            project_name (str): project name
+
+        Returns:
+            message (str): 'Success' if successful, 'Failure' along with failure reason
+        """
+        project = Project(self)
+        status_message = project.delete_project(project_name=project_name)
+        return status_message
 
     def get_project_list(self):
         """ Returns list of all projects
 
         Returns:
             projects (list): list of project dict
 
@@ -121,430 +104,259 @@
                 {
                     "projectName": "xyz",
                     "projectDescription": "xyz desc",
                     "projectUUID": "aabbcd"
                 }
             ]
 
+            errorMessage (str): "Failure: Project list is empty."
+
         """
         project = Project(client=self)
-        status_message = project.get_projects(project)
+        status_message = project.get_project_list()
         return status_message
-        # pass
 
-    # Android Application
+    # Application
 
-    def upload_android_application(self, project_name=None, file_path=None):
-        """ Upload android application(.apk) from given file path
+    def upload_application(self, file_category=None, project_name=None, file_path=None):
+        """ Upload android or ios application(.apk or .ipa) from given file path
 
         Args:
+            file_category (str): Mandatory 'android-application' or 'ios-application'
             project_name (str): Container project for the application
             file_path (str): relative or absolute path of the file
 
         Returns:
             message (str): 'Success' if uploaded successfully, 'Failure' along with failure reason
 
-            "Failure: File with `{file_name}` already exists." - in case if file with checksum already exists
+            "Success: File `" + file_name + "` uploaded successfully."
+            "Failure: File `" + file_name + "` not uploaded."
+            "Error: File `" + file_name + "` already exists."
+            "File Not Found Error: File `" + file_name + "` File not found or wrong path."
+
         """
         file = File(client=self)
-        status = file.upload_android_application(project_name=project_name, file_path=file_path)
+        status = file.upload_application(file_category=file_category, project_name=project_name, file_path=file_path)
         return status
 
-    def get_android_application_info(self, file_name=None):
-        """ Returns android file information
+    def get_application_info(self, file_name=None):
+        """ Returns file information
 
         Args:
             file_name (str): unique file name
 
         Returns:
             fileinfo (dict): dictionary containing the metadata about the file
 
             {
                 "fileName" : "",
-                "fileCategory": "android-application",
+                "fileCategory": "android-application | ios-application",
                 "md5": "",
                 "fileURL": "",
                 "fileUUID": "",
                 "packageName": ""
             }
-        """
-        # pass
-        file = File(client=self)
-        app_list = file.list_android_application(file, file_name=file_name)
-        return app_list
 
-    # def rename_android_application(self, file_name_old=None, file_name_new=None):
-    #     pass
-
-    def delete_android_application(self, file_id=None):
-        # pass
-        file = File(client=self)
-        status = file.delete_file(file, file_id=file_id)
-        return status
-
-    def get_android_application_list(self, project_name=None):
-        """ Returns list of all android application file information
-
-        Returns:
-            fileinfo (list): dictionary containing the metadata about the file
+            errorMessage (str): "Failure: File with name `{file_name}` not found."
 
-            [
-                {
-                    "fileName" : "",
-                    "fileCategory": "android-application",
-                    "md5": "",
-                    "fileURL": "",
-                    "fileUUID": "",
-                    "packageName": ""
-                },
-                {
-                    "fileName" : "",
-                    "fileCategory": "android-application",
-                    "md5": "",
-                    "fileURL": "",
-                    "fileUUID": "",
-                    "packageName": ""
-                }
-            ]
+            Note:
+                "packageName" is present in case of 'android-application'
         """
-        # pass
         file = File(client=self)
-        app_list = file.list_android_application(file, project_name=project_name)
+        app_list = file.get_application_info(file_name=file_name)
         return app_list
 
-    # iOS Application
-    def upload_ios_application(self, project_name=None, file_path=None):
-        """ Upload ios application(.ipa) from given file path
-
+    def delete_application(self, file_name=None):
+        """ Delete application with given file name
         Args:
-            project_name (str): Container project for the application
-            file_path (str): relative or absolute path of the file
+            file_name (str): unique file name
 
         Returns:
-            message (str): 'Success' if uploaded successfully, 'Failure' along with failure reason
-
-            "Failure: File with `{file_name}` already exists." - in case if file with checksum already exists
+            "Success: File `" + file_name + "` deleted successfully."
+            "Failure: File `" + file_name + "` not deleted."
         """
-        # pass
         file = File(client=self)
-        status = file.upload_ios_application(project_name=project_name, file_path=file_path)
+        status = file.delete_file(file_name=file_name)
         return status
 
-    def get_ios_application_info(self, file_name=None):
-        """ Returns ios application file information
+    def get_application_list(self, file_category=None, project_name=None):
+        """ Returns list of all application file information
 
         Args:
-            file_name (str): unique file name
-
-        Returns:
-            fileinfo (dict): dictionary containing the metadata about the file
-
-            {
-                "fileName" : "",
-                "fileCategory": "ios-application",
-                "md5": "",
-                "fileURL": "",
-                "fileUUID": "",
-                "packageName": ""
-            }
-        """
-        # pass
-        file = File(client=self)
-        app_list = file.list_ios_application(file, file_name=file_name)
-        return app_list
-
-    # def rename_ios_application(self, file_name_old=None, file_name_new=None):
-    #     pass
-
-    def delete_ios_application(self, file_id=None):
-        # pass
-        file = File(client=self)
-        status = file.delete_file(file, file_id=file_id)
-        return status
-
-    def get_ios_application_list(self, project_name=None):
-        """ Returns list of all ios application file information
+            file_category (str): mandatory 'android-application' or 'ios-application'
+            project_name (str): optional project_name to filter the android application files
 
         Returns:
             fileinfo (list): dictionary containing the metadata about the file
 
             [
                 {
                     "fileName" : "",
-                    "fileCategory": "ios-application",
+                    "fileCategory": "android-application",
                     "md5": "",
                     "fileURL": "",
                     "fileUUID": "",
-                    "packageName": ""
+                    "packageName": "",
+                    "projectName": ""
                 },
                 {
                     "fileName" : "",
                     "fileCategory": "ios-application",
                     "md5": "",
                     "fileURL": "",
                     "fileUUID": "",
-                    "packageName": ""
+                    "projectName": ""
                 }
             ]
+
+            Note: "projectName" will be present in response if passed in a filter, else the value will be ""
         """
-        # pass
         file = File(client=self)
-        app_list = file.list_ios_application(file, project_name=project_name)
+        app_list = file.get_application_list(file_category=file_category, project_name=project_name)
         return app_list
 
-    # Android Native Test Application
+    # Native Test Application
 
-    def upload_android_native_test_application(self, project_name=None, file_path=None):
-        """ Upload android native test application(.apk) from given file path
+    def upload_native_test_application(self, file_category=None, project_name=None, file_path=None):
+        """ Upload native test application(.apk or .ipa) from given file path
 
         Args:
+            file_category (str): Mandatory 'android-application' or 'ios-application'
             project_name (str): Container project for the application
             file_path (str): relative or absolute path of the file
 
         Returns:
             message (str): 'Success' if uploaded successfully, 'Failure' along with failure reason
 
-            "Failure: File with `{file_name}` already exists." - in case if file with checksum already exists
+            "Success: File `" + file_name + "` uploaded successfully."
+            "Failure: File `" + file_name + "` not uploaded."
+            "Error: File `" + file_name + "` already exists."
         """
-        # pass
         file = File(client=self)
-        status = file.upload_android_native_test_application(project_name=project_name, file_path=file_path)
+        status = file.upload_native_test_application(file_category=file_category,
+                                                     project_name=project_name,
+                                                     file_path=file_path)
         return status
 
-    def get_android_native_test_application_info(self, file_name=None):
-        """ Returns android native test application file information
+    def get_native_test_application_info(self, file_name=None):
+        """ Returns file information
 
         Args:
             file_name (str): unique file name
 
         Returns:
             fileinfo (dict): dictionary containing the metadata about the file
 
             {
                 "fileName" : "",
-                "fileCategory": "android-test-application",
+                "fileCategory": "android-test-application | ios-test-application",
                 "md5": "",
                 "fileURL": "",
                 "fileUUID": "",
                 "testCodePackageName": "",
-                "testRunnerName": ""
+                "testRunnerName": "",
+                "XCTestRunFileUrl": ""
             }
-        """
-        # pass
-        file = File(client=self)
-        app_list = file.list_android_native_test_application(file, file_name=file_name)
-        return app_list
 
-    # def rename_android_native_test_application(self, file_name_old=None, file_name_new=None):
-    #     pass
-
-    def delete_android_native_test_application(self, file_id=None):
-        # pass
-        file = File(client=self)
-        status = file.delete_file(file, file_id=file_id)
-        return status
+            errorMessage (str): "Failure: File with name `{file_name}` not found."
 
-    def get_android_native_test_application_list(self, project_name=None, file_name=None):
-        """ Returns list of all android native test application file information
+            Note:
+                "testCodePackageName" and "testRunnerName" is present in case of 'android-test-application'
+                "XCTestRunFileUrl" is present in case of 'ios-test-application'
 
-        Returns:
-            fileinfo (list): dictionary containing the metadata about the file
-
-            [
-                {
-                    "fileName" : "",
-                    "fileCategory": "android-test-application",
-                    "md5": "",
-                    "fileURL": "",
-                    "fileUUID": "",
-                    "testCodePackageName": "",
-                    "testRunnerName": ""
-                },
-                {
-                    "fileName" : "",
-                    "fileCategory": "android-test-application",
-                    "md5": "",
-                    "fileURL": "",
-                    "fileUUID": "",
-                    "testCodePackageName": "",
-                    "testRunnerName": ""
-                }
-            ]
         """
-        # pass
         file = File(client=self)
-        app_list = file.list_android_native_test_application(file, project_name=project_name, file_name=file_name)
+        app_list = file.get_native_test_application_info(file_name=file_name)
         return app_list
 
-    # iOS Application
-    def upload_ios_native_test_application(self, project_name=None, file_path=None):
-        """ Upload ios native test application(.ipa) from given file path
-
+    def delete_native_test_application(self, file_name=None):
+        """ Delete native test application with given file name
         Args:
-            project_name (str): Container project for the application
-            file_path (str): relative or absolute path of the file
-
-        Returns:
-            message (str): 'Success' if uploaded successfully, 'Failure' along with failure reason
-
-            "Failure: File with `{file_name}` already exists." - in case if file with checksum already exists
-        """
-        # pass
-        file = File(client=self)
-        status = file.upload_ios_native_test_application(project_name=project_name, file_path=file_path)
-        return status
-
-    def get_ios_native_test_application_info(self, file_name=None):
-        """ Returns ios native test application file information
-
-        Args:
-            project_name (str): project names
             file_name (str): unique file name
 
         Returns:
-            fileinfo (dict): dictionary containing the metadata about the file
-
-            {
-                "fileName" : "",
-                "fileCategory": "ios-test-application",
-                "md5": "",
-                "fileURL": "",
-                "fileUUID": "",
-                "XCTestRunFileUrl": ""
-            }
+            "Success: File `" + file_name + "` deleted successfully."
+            "Failure: File `" + file_name + "` not deleted."
         """
-        # pass
         file = File(client=self)
-        status = file.list_ios_native_test_application(file_name=file_name)
+        status = file.delete_file(file_name=file_name)
         return status
 
-    # def rename_ios_native_test_application(self, file_name_old=None, file_name_new=None):
-    #     pass
-
-    def delete_ios_native_test_application(self, file_id=None):
-        # pass
-        file = File(client=self)
-        status = file.delete_file(file, file_id=file_id)
-        return status
+    def get_native_test_application_list(self, file_category=None, project_name=None):
+        """ Returns list of all application file information
 
-    def get_ios_native_test_application_list(self, project_name=None):
-        """ Returns list of all ios native test application file information
+        Args:
+            file_category (str): mandatory 'android-application' or 'ios-application'
+            project_name (str): optional project_name to filter the android application files
 
         Returns:
             fileinfo (list): dictionary containing the metadata about the file
 
             [
                 {
                     "fileName" : "",
-                    "fileCategory": "ios-test-application",
+                    "fileCategory": "android-test-application",
                     "md5": "",
                     "fileURL": "",
                     "fileUUID": "",
-                    "XCTestRunFileUrl": ""
+                    "testCodePackageName": "",
+                    "testRunnerName": "",
+                    "projectName": ""
                 },
                 {
                     "fileName" : "",
                     "fileCategory": "ios-test-application",
                     "md5": "",
                     "fileURL": "",
                     "fileUUID": "",
                     "XCTestRunFileUrl": ""
+                    "projectName": ""
                 }
             ]
+
+            Note: "projectName" will be present in response if passed in a filter, else the value will be ""
         """
-        # pass
         file = File(client=self)
-        status = file.list_ios_native_test_application(project_name=project_name)
-        return status
+        app_list = file.get_native_test_application_list(file_category=file_category, project_name=project_name)
+        return app_list
 
     # Device
+    def add_device(self, device_parameter=None):
+        """ Add Devices
 
-    def get_device_info(self, device_serial=None):
-        """ Returns device information given a device serial
-
-        Args:
-            device_serial (str): unique device serial
+                Args:
+                    device_parameter(json): device details
 
-        Returns:
-            device_info (dict): dictionary containing the information about the device
+                Returns:
+                    message (str): 'Success'
 
-            {
-                "deviceSerial": "",
-                "deviceBrand": "",
-                "deviceCity": "",
-                "deviceCountry": "",
-                "deviceModelName": "",
-                "deviceModelNumber": "",
-                "devicePlatform": "android | ios",
-                "deviceOSVersion": "",
-                "deviceSDKVersion": ["", ""],
-                "deviceUUID": "",
-                "deviceNetwork": ""
-            }
-        """
-        pass
-
-    # def get_device_busy_slots(self, devices=None):
-    #     pass
-
-    def get_android_device_list(self):
-        """ Returns device information of all android devices
-
-        Returns:
-            device_info (list): list of dictionary containing the information about the device
-
-            [
-                {
-                    "deviceSerial": "",
-                    "deviceBrand": "",
-                    "deviceCity": "",
-                    "deviceCountry": "",
-                    "deviceModelName": "",
-                    "deviceModelNumber": "",
-                    "devicePlatform": "android",
-                    "deviceOSVersion": "",
-                    "deviceSDKVersion": ["", ""],
-                    "deviceUUID": "",
-                    "deviceNetwork": ""
-                },
-                {
-                    "deviceSerial": "",
-                    "deviceBrand": "",
-                    "deviceCity": "",
-                    "deviceCountry": "",
-                    "deviceModelName": "",
-                    "deviceModelNumber": "",
-                    "devicePlatform": "android",
-                    "deviceOSVersion": "",
-                    "deviceSDKVersion": ["", ""],
-                    "deviceUUID": "",
-                    "deviceNetwork": ""
-                }
-            ]
-        """
-        # pass
+                    "Failure: Device with name " + device_parameter["serial"] + " already exists."
+                """
         device = Device(client=self)
-        device_list = device.get_devices(device, "android")
-        return device_list
+        device_added = device.add_device(device_parameter=device_parameter)
+        return device_added
 
-    def get_ios_device_list(self):
-        """ Returns device information of all iOS devices
+    def get_device_list(self, platform=None, device_serial=None):
+        """ Returns device information of all devices for a given platform or device_serial
+        Args:
+            platform (str): device platform type: 'android', 'ios', or 'living-room'
+            device_serial (str): unique device serial
 
         Returns:
             device_info (list): list of dictionary containing the information about the device
 
             [
                 {
                     "deviceSerial": "",
                     "deviceBrand": "",
                     "deviceCity": "",
                     "deviceCountry": "",
                     "deviceModelName": "",
                     "deviceModelNumber": "",
-                    "devicePlatform": "ios",
+                    "devicePlatform": "android",
                     "deviceOSVersion": "",
                     "deviceSDKVersion": ["", ""],
                     "deviceUUID": "",
                     "deviceNetwork": ""
                 },
                 {
                     "deviceSerial": "",
@@ -554,41 +366,14 @@
                     "deviceModelName": "",
                     "deviceModelNumber": "",
                     "devicePlatform": "ios",
                     "deviceOSVersion": "",
                     "deviceSDKVersion": ["", ""],
                     "deviceUUID": "",
                     "deviceNetwork": ""
-                }
-            ]
-        """
-        # pass
-        device = Device(client=self)
-        device_list = device.get_devices(device, "ios")
-        return device_list
-
-    def get_living_room_device_list(self):
-        """ Returns device information of all living room devices
-
-        Returns:
-            device_info (list): list of dictionary containing the information about the device
-
-            [
-                {
-                    "deviceSerial": "",
-                    "deviceBrand": "",
-                    "deviceCity": "",
-                    "deviceCountry": "",
-                    "deviceModelName": "",
-                    "deviceModelNumber": "",
-                    "devicePlatform": "living-room",
-                    "deviceOSVersion": "",
-                    "deviceSDKVersion": ["", ""],
-                    "deviceUUID": "",
-                    "deviceNetwork": ""
                 },
                 {
                     "deviceSerial": "",
                     "deviceBrand": "",
                     "deviceCity": "",
                     "deviceCountry": "",
                     "deviceModelName": "",
@@ -597,97 +382,142 @@
                     "deviceOSVersion": "",
                     "deviceSDKVersion": ["", ""],
                     "deviceUUID": "",
                     "deviceNetwork": ""
                 }
             ]
         """
-        # pass
         device = Device(client=self)
-        device_list = device.get_lr_devices()
+        device_list = device.get_devices(platform=platform, device_serial=device_serial)
         return device_list
 
-    def create_tray(self, tray_name=None, platform=None, device_list=None):
+    # def get_device_busy_slots(self, devices=None):
+    #     pass
+
+    def create_tray(self, platform=None, tray_name=None, device_list=None):
         """ Create tray for a given device platform category
 
         Args:
-            tray_name (str): Unique tray name
-            device_list (str): device list
             platform(str): type of devices
+            tray_name (str): Unique tray name(without spaces)
+            device_list (list): device list
 
         Returns:
             message (str): 'Success' if tray is created successfully, 'Failure' along with failure reason
 
-            "Failure: Tray with `{tray_name}` already exists" - in case if a tray with a given name already exists
+            "Failure: Tray with `{tray_name}` already exists." - in case if a tray with a given name already exists
         """
-        # pass
         tray = Tray(client=self)
-        status = tray.create_tray(name=tray_name, platform=platform, device_list=device_list)
+        status = tray.create_tray(platform=platform, tray_name=tray_name, device_list=device_list)
         return status
 
-    def get_tray_list(self):
-        # pass
+    def get_tray_info(self, tray_name=None):
+        """ Returns tray information for a given tray name
+        Args:
+            tray_name (str): Tray Name
+
+        Returns:
+
+            tray_info(dict): tray information along with device info
+
+            {
+                "trayName": "",
+                "trayPlatform": "android",
+                "trayUUID": "",
+                "trayDevices" : [
+                    {
+                        "deviceSerial": "",
+                        "deviceBrand": "",
+                        "deviceCity": "",
+                        "deviceCountry": "",
+                        "deviceModelName": "",
+                        "deviceModelNumber": "",
+                        "devicePlatform": "android",
+                        "deviceOSVersion": "",
+                        "deviceSDKVersion": ["", ""],
+                        "deviceUUID": "",
+                        "deviceNetwork": ""
+                    },
+                    {
+                        "deviceSerial": "",
+                        "deviceBrand": "",
+                        "deviceCity": "",
+                        "deviceCountry": "",
+                        "deviceModelName": "",
+                        "deviceModelNumber": "",
+                        "devicePlatform": "android",
+                        "deviceOSVersion": "",
+                        "deviceSDKVersion": ["", ""],
+                        "deviceUUID": "",
+                        "deviceNetwork": ""
+                    }
+                ]
+            }
+        """
         tray = Tray(client=self)
-        status = tray.list_tray()
-        return status
+        tray_info = tray.get_tray_info(tray_name=tray_name)
+        return tray_info
 
-    def update_tray_devices(self, tray_id=None, device_list=None):
-        # pass
+    def update_tray(self, tray_name=None, device_list=None):
+        """ Update List of devices for a given tray name
+
+        Args:
+            tray_name(str): Tray name
+            device_list(list): Updated device list
+
+        Returns:
+            message (str): 'Success' if tray is updated successfully, 'Failure' along with failure reason
+
+            "Failure" in case of failure
+        """
         tray = Tray(client=self)
-        status = tray.update_tray(tray_id=tray_id, device_list=device_list)
+        status = tray.update_tray(tray_name=tray_name, device_list=device_list)
         return status
 
-    def delete_tray(self, tray_id=None):
-        # pass
+    def delete_tray(self, tray_name=None):
+        """ Delete tray with a given tray name
+
+        Args:
+            tray_name(str): Tray name
+
+        Returns:
+            message (str): 'Success' if tray is updated successfully, 'Failure' along with failure reason
+
+            "Failure" in case of failure
+        """
         tray = Tray(client=self)
-        status = tray.delete_tray(tray_id=tray_id)
+        status = tray.delete_tray(tray_name=tray_name)
         return status
 
-    def get_device_list_by_tray(self, tray_id=None):
-        """ Returns device information of all devices added as part of a given tray
-
+    def get_tray_list(self):
+        """ Get tray list
         Returns:
-            device_info (list): list of dictionary containing the information about the device
+            tray_list(list): List of tray info
 
             [
                 {
-                    "deviceSerial": "",
-                    "deviceBrand": "",
-                    "deviceCity": "",
-                    "deviceCountry": "",
-                    "deviceModelName": "",
-                    "deviceModelNumber": "",
-                    "devicePlatform": "android",
-                    "deviceOSVersion": "",
-                    "deviceSDKVersion": ["", ""],
-                    "deviceUUID": "",
-                    "deviceNetwork": ""
+                    "trayName": "",
+                    "trayPlatform": "android",
+                    "trayUUID": ""
                 },
                 {
-                    "deviceSerial": "",
-                    "deviceBrand": "",
-                    "deviceCity": "",
-                    "deviceCountry": "",
-                    "deviceModelName": "",
-                    "deviceModelNumber": "",
-                    "devicePlatform": "android",
-                    "deviceOSVersion": "",
-                    "deviceSDKVersion": ["", ""],
-                    "deviceUUID": "",
-                    "deviceNetwork": ""
+                    "trayName": "",
+                    "trayPlatform": "ios",
+                    "trayUUID": ""
+                },
+                {
+                    "trayName": "",
+                    "trayPlatform": "living-room",
+                    "trayUUID": ""
                 }
             ]
         """
-
-        # pass
         tray = Tray(client=self)
-        status = tray.get_tray_info(tray_id=tray_id)
-        return status
-
-
+        tray_list = tray.get_tray_list()
+        return tray_list
 
     # Test Configuration & Test Parameters
 
     def get_supported_test_configuration(self, platform=None):
         mobile_test_configuration = {
             "captureHAR": False,
             "captureCPUMetrics": False,
@@ -698,21 +528,22 @@
             "recordDeviceScreen": False,
             "captureDeviceNetworkPackets": False
         }
         living_room_test_configuration = {
             "captureDeviceScreenShots": False,
             "recordDeviceScreen": False
         }
+        config = {}
         if platform == "android":
             config = mobile_test_configuration
         elif platform == "ios":
             config = mobile_test_configuration
         elif platform == "living-room":
             config = living_room_test_configuration
-        return mobile_test_configuration
+        return config
 
     def get_default_test_parameters(self):
         test_parameters = {
             "maxTestDuration": 5,
             "testFramework": "android-uiautomator",
             "projectName": "",
         }
@@ -720,153 +551,491 @@
 
     def get_mandatory_test_parameters(self, platform=None):
         pass
 
     # Test Execution
 
     def start_test_execution(self,
+                             project_name=None,
+                             test_framework=None,
+                             application_file_name=None,
+                             test_application_file_name=None,
                              devices=None,
-                             application_url=None,
-                             test_application_url=None,
                              test_configuration=None,
                              test_parameters=None
                              ):
-        # pass
+        """ Execute test now for a given configuration
+
+        Args:
+            project_name(str): project name
+            test_framework(str): supported test framework 'android-uiautomator' or 'ios-xcuitest'
+            application_file_name(str): file name of an application .apk or .ipa
+            test_application_file_name: file name of a test application .apk or .ipa
+            devices(list): list of device serial
+            test_configuration(dict): test configuration as a key value pairs
+            test_parameters(dict): test parameters as a key value pairs
+
+        Returns:
+            test_status(dict): test status containing the message and a test id to monitor
+
+            {
+                "message": "Success: Executed/Scheduled successfully",
+                "testId": ""
+            }
+        """
+        action = TestExecute(client=self)
+        status = action.execute_test_now(project_name=project_name,
+                                         test_framework=test_framework,
+                                         application_file_name=application_file_name,
+                                         test_application_file_name=test_application_file_name,
+                                         devices=devices,
+                                         test_configuration=test_configuration,
+                                         test_parameters=test_parameters
+                                         )
+        return status
+
+    def get_test_info(self, test_id=None):
+        """ get test info
+
+        Args:
+            test_id(str):
+
+        Returns:
+            {
+                "projectName" : "",
+                "testFramework": "android-uiautomator | ios-xcuitest | living-room-automate",
+                "applicationFileName": "",
+                "testApplicationFileName": "",
+                "device": "",
+                "testStartTime": "",
+                "testEndTime": "",
+                "testUUID": "",
+                "testStatus": "SCHEDULED | STARTED | COMPLETED | ABORTED | FAILED",
+                "testStatusDescription": ""
+            }
+
+        """
         action = TestExecute(client=self)
-        status = action.test_now(device_list=devices, application_url=application_url,
-                                 application_test_url=test_application_url,
-                                 test_configuration=test_configuration, test_parameters=test_parameters)
+        status = action.get_test_info(test_id=test_id)
         return status
 
     def abort_test_execution(self, test_id=None):
-        pass
+        """ Abort a test which is running
+
+        Args:
+            test_id(str):
+
+        Returns:
+            testStatus(str): 'Success' if aborted successfully. 'Failure' with failure reason
+        """
+        action = TestExecute(client=self)
+        status = action.abort_test(test_id=test_id)
+        return status
 
     def schedule_test_execution(self,
+                                project_name=None,
+                                test_framework=None,
+                                application_file_name=None,
+                                test_application_file_name=None,
                                 devices=None,
-                                application_url=None,
-                                test_application_url=None,
-                                schedule_configuration=None,
                                 test_configuration=None,
                                 test_parameters=None,
+                                start_date_time=None,
+                                end_date_time=None,
+                                interval=None
                                 ):
-        """
+        """ Execute test now for a given configuration
 
         Args:
-            devices:
-            application_url:
-            test_application_url:
-            test_framework:
-            test_configuration:
-            test_parameters:
-            test_start_datetime:
-            test_end_datetime:
-            interval:
+            project_name(str): project name
+            test_framework(str): supported test framework 'android-uiautomator' or 'ios-xcuitest'
+            application_file_name(str): file name of an application .apk or .ipa
+            test_application_file_name: file name of a test application .apk or .ipa
+            devices(list): list of device serial
+            test_configuration(dict): test configuration as a key value pairs
+            test_parameters(dict): test parameters as a key value pairs
+            start_date_time(datetime): schedule start date and time
+            end_date_time(datetime): schedule end date and time
+            interval(number): interval between two test runs
 
         Returns:
-            response (dict): unique schedule ID created if successful, else Error along with error message
+            test_status(dict): test status containing the message and a test id to monitor
 
             {
-                "message" = "Success",
-                "scheduleId" = ""
+                "message": "Success: Executed/Scheduled successfully",
+                "scheduleUUID": "",
+                "testRuns": [
+                    {
+                        "testUUID" : "",
+                        "testStartDateTime": "",
+                    },
+                    {
+                        "testUUID" : "",
+                        "testStartDateTime": "",
+                    }
+                ]
             }
 
         """
         action = TestExecute(client=self)
-        status = action.schedule_test(device_list=devices, application_url=application_url,
-                                      application_test_url=test_application_url,
-                                      schedule_configuration=schedule_configuration,
-                                      test_configuration=test_configuration, test_parameters=test_parameters)
-        return status
-
-    # def get_test_schedule_info(self, schedule_id=None):
-    #     f"""
-    #
-    #     Args:
-    #         schedule_id:
-    #
-    #     Returns:
-    #         schedule_info (dict):
-    #
-    #         {
-    #     "scheduleId" : "schedule_id",
-    #             test_ids : [
-    #                 "test_id1",
-    #                 "test_id2",
-    #                 "test_id3"
-    #             ]
-    #
-    #         }
-    #
-    #     """
-    #     pass
+        status = action.schedule_test_executions(project_name=project_name,
+                                                 test_framework=test_framework,
+                                                 application_file_name=application_file_name,
+                                                 test_application_file_name=test_application_file_name,
+                                                 devices=devices,
+                                                 test_configuration=test_configuration,
+                                                 test_parameters=test_parameters,
+                                                 start_date_time=start_date_time,
+                                                 end_date_time=end_date_time,
+                                                 interval=interval
+                                                 )
+        return status
 
-    def cancel_test_schedule(self, schedule_id=None):
-        # pass
+    def update_schedule(self, data=None, schedule_id=None):
         action = TestExecute(client=self)
-        status = action.delete_schedule(action, schedule_id=schedule_id)
+        """ Update schedule info
+
+                Args:
+                    schedule_id(str): schedule id
+                    data(json): parameter
+
+                Returns:
+                    schedule_update (dict): Schedule Update Successfully
+        """
+        status = action.update_schedule(data=data, schedule_id=schedule_id)
         return status
 
-    def get_test_schedule_list(self):
-        # pass
+    def update_test(self, data=None,test_id=None):
         action = TestExecute(client=self)
-        schedule_list = action.list_schedules(action)
+        """ Update test info
+
+                Args:
+                    test_id(str): test id
+                    data(json): parameter
+                    
+                Returns:
+                    test_update (dict): Test Update Successfully
+        """
+        status = action.update_test(data=data, test_id=test_id)
+        return status
+
+    def get_test_schedule_info(self, schedule_id=None):
+        """ get test schedule info
+
+        Args:
+            schedule_id(str): schedule id
+
+        Returns:
+            schedule_info (dict): schedule information containing the list of test info
+
+            {
+                "scheduleUUID": "",
+                "scheduleStartTime": "",
+                "scheduleEndTime": "",
+                "testInterval": "",
+                "testConfiguration": {}
+                "testParameters": {},
+                "projectName" : "",
+                "testFramework": "android-uiautomator | ios-xcuitest | living-room-automate",
+                "applicationFileName": "",
+                "testApplicationFileName": "",
+                "testInfo": [
+                    {
+                        "device": "",
+                        "testStartTime": "",
+                        "testEndTime": "",
+                        "testUUID": "",
+                        "testStatus": "SCHEDULED | STARTED | COMPLETED | ABORTED | FAILED",
+                        "testStatusDescription": ""
+                    },
+                    {
+                        "device": "",
+                        "testStartTime": "",
+                        "testEndTime": "",
+                        "testUUID": "",
+                        "testStatus": "SCHEDULED | STARTED | COMPLETED | ABORTED | FAILED",
+                        "testStatusDescription": ""
+                    }
+            }
+        """
+        action = TestExecute(client=self)
+        status = action.get_test_schedule_info(schedule_id=schedule_id)
+        return status
+
+    def delete_test_schedule(self, schedule_id=None):
+        """ Delete the test schedule
+
+        Args:
+            schedule_id(str):
+
+        Returns:
+            testScheduleStatus(str): 'Success' if deleted successfully. 'Failure' with failure reason
+        """
+        action = TestExecute(client=self)
+        status = action.delete_schedule(schedule_id=schedule_id)
+        return status
+
+    def get_test_schedule_list(self, from_date_time=None, to_date_time=None):
+        """ get list of test schedule info
+
+        Returns:
+            schedule_info(list): list of schedule info
+
+            [
+                {
+                    "scheduleUUID": "",
+                    "scheduleStartTime": "",
+                    "scheduleEndTime": "",
+                    "testInterval": "",
+                    "testConfiguration": {}
+                    "testParameters": {},
+                    "projectName" : "",
+                    "testFramework": "android-uiautomator | ios-xcuitest | living-room-automate",
+                    "applicationFileName": "",
+                    "testApplicationFileName": "",
+                    "testInfo": [
+                        {
+                            "device": "",
+                            "testStartTime": "",
+                            "testEndTime": "",
+                            "testUUID": "",
+                            "testStatus": "SCHEDULED | STARTED | COMPLETED | ABORTED | FAILED",
+                            "testStatusDescription": ""
+                        },
+                        {
+                            "device": "",
+                            "testStartTime": "",
+                            "testEndTime": "",
+                            "testUUID": "",
+                            "testStatus": "SCHEDULED | STARTED | COMPLETED | ABORTED | FAILED",
+                            "testStatusDescription": ""
+                        }
+                },
+                {
+                    "scheduleUUID": "",
+                    "scheduleStartTime": "",
+                    "scheduleEndTime": "",
+                    "testInterval": "",
+                    "testConfiguration": {}
+                    "testParameters": {},
+                    "projectName" : "",
+                    "testFramework": "android-uiautomator | ios-xcuitest | living-room-automate",
+                    "applicationFileName": "",
+                    "testApplicationFileName": "",
+                    "testInfo": [
+                        {
+                            "device": "",
+                            "testStartTime": "",
+                            "testEndTime": "",
+                            "testUUID": "",
+                            "testStatus": "SCHEDULED | STARTED | COMPLETED | ABORTED | FAILED",
+                            "testStatusDescription": ""
+                        },
+                        {
+                            "device": "",
+                            "testStartTime": "",
+                            "testEndTime": "",
+                            "testUUID": "",
+                            "testStatus": "SCHEDULED | STARTED | COMPLETED | ABORTED | FAILED",
+                            "testStatusDescription": ""
+                        }
+                }
+            ]
+        """
+        action = TestExecute(client=self)
+        schedule_list = action.get_test_schedule_list(from_date_time=from_date_time, to_date_time=to_date_time)
         return schedule_list
 
     # Test Analytics
+    def get_test_list(self, from_date_time=None, to_date_time=None):
+        """ get list of test info
 
-    def get_test_list(self):
-        # pass
+        Returns:
+            test_info(list): list of test info
+
+            [
+                {
+                    "projectName" : "",
+                    "testFramework": "android-uiautomator | ios-xcuitest | living-room-automate",
+                    "applicationFileName": "",
+                    "testApplicationFileName": "",
+                    "device": "",
+                    "testStartTime": "",
+                    "testEndTime": "",
+                    "testUUID": "",
+                    "testStatus": "SCHEDULED | STARTED | COMPLETED | ABORTED | FAILED",
+                    "testStatusDescription": ""
+                },
+                {
+                    "projectName" : "",
+                    "testFramework": "android-uiautomator | ios-xcuitest | living-room-automate",
+                    "applicationFileName": "",
+                    "testApplicationFileName": "",
+                    "device": "",
+                    "testStartTime": "",
+                    "testEndTime": "",
+                    "testUUID": "",
+                    "testStatus": "SCHEDULED | STARTED | COMPLETED | ABORTED | FAILED",
+                    "testStatusDescription": ""
+                }
+            ]
+        """
         analytics = TestAnalytics(client=self)
-        test_list = analytics.get_test_list(analytics)
+        test_list = analytics.get_test_list(from_date_time=from_date_time, to_date_time=to_date_time)
         return test_list
 
     def get_test_execution_info_full(self, test_id=None):
+        """ Get test execution info by test id
+
+        Args:
+            test_id: test id
+
+        Returns:
+            {
+                "testUUID": "",
+                "testStartDateTime": "",
+                "testEndDateTime": "",
+                "projectName": "",
+                "applicationFileName": "",
+                "testApplicationFileName": "",
+                "deviceSerial": "",
+                "deviceMake": "",
+                "deviceModel": "",
+                "deviceCity": "",
+                "deviceCountry": "",
+                "deviceNetwork": "",
+                "devicePlatform": "",
+                "deviceOSVersion": "",
+                "deviceNetworkOperator": "",
+                "testStatus": "",
+                "testStatusDescription": "",
+                "testCasesTotal": "",
+                "testCasesPassed": "",
+                "testCasesFailed": "",
+                "testCases": [
+                    {
+                        "testCaseName": "",
+                        "testCaseResult": "PASS | FAIL",
+                        "testCaseStartDateTime": "",
+                        "testCaseEndDateTime": "",
+                    },
+                    {
+                        "testCaseName": "",
+                        "testCaseResult": "PASS | FAIL",
+                        "testCaseStartDateTime": "",
+                        "testCaseEndDateTime": "",
+                    },
+                    {
+                        "testCaseName": "",
+                        "testCaseResult": "PASS | FAIL",
+                        "testCaseStartDateTime": "",
+                        "testCaseEndDateTime": "",
+                    }
+                ],
+                "userExperienceKpis": [
+                    {
+                        "kpiName": "",
+                        "kpiValue": "",
+                        "testCaseName": ""
+                    },
+                    {
+                        "kpiName": "",
+                        "kpiValue": "",
+                        "testCaseName": ""
+                    },
+                    {
+                        "kpiName": "",
+                        "kpiValue": "",
+                        "testCaseName": ""
+                    }
+                ],
+                "events": [
+                    {
+                        "eventName": "",
+                        "eventDateTime": "",
+                        "testCaseName": ""
+                    },
+                    {
+                        "eventName": "",
+                        "eventDateTime": "",
+                        "testCaseName": ""
+                    },
+                    {
+                        "eventName": "",
+                        "eventDateTime": "",
+                        "testCaseName": ""
+                    }
+                ]
+            }
+        """
         analytics = TestAnalytics(client=self)
-        test_info = analytics.get_test_information(analytics, test_id)
-        test_cases = analytics.get_test_testcases(analytics, test_id)
-        test_events = analytics.get_test_events(analytics, test_id)
-        test_kpis = analytics.get_test_kpis(analytics, test_id)
-        test_http_apis = analytics.get_test_apis(analytics, test_id)
-        test_screenshots = analytics.get_test_screenshot_list(analytics, test_id)
-        test_logs = analytics.get_test_output_file_list(analytics, test_id)
-
-        return {
-            "test_info": test_info,
-            "test_cases": test_cases,
-            "events": test_events,
-            "kpis": test_kpis,
-            "http_api": test_http_apis,
-            "screenshots": test_screenshots,
-            "logs": test_logs
-        }
+        result = analytics.get_test_execution_info_full(test_id=test_id)
+        return result
 
     def get_test_execution_info_by_section(self, test_id=None, section=None):
-        # Section = test_info, test_configuration, test_case_summary, test_cases, test_output_artifacts, events
-        # KPIs,
-        # pass
-        analytics = TestAnalytics(client=self)
-        response = None
-        if section == "test_info":
-            response = analytics.get_test_information(analytics, test_id)
-        elif section == "test_cases":
-            response = analytics.get_test_testcases(analytics, test_id)
-        elif section == "events":
-            response = analytics.get_test_events(analytics, test_id)
-        elif section == "kpis":
-            response = analytics.get_test_kpis(analytics, test_id)
-        elif section == "http_api":
-            response = analytics.get_test_apis(analytics, test_id)
-        elif section == "screenshots":
-            response = analytics.get_test_screenshot_list(analytics, test_id)
-        elif section == "logs":
-            response = analytics.get_test_output_file_list(analytics, test_id)
-        return response
+        """ Get Test Execution info by information section
 
-    def download_test_screenshot(self, test_id=None, image_name=None, file_name=None):
+        Args:
+            test_id(str): test id
+            section(str): supported info section names
+                        - 'basic_test_info'
+                        - 'test_configuration'
+                        - 'test_cases'
+                        - 'events'
+                        - 'kpis_user_experience'
+                        - 'kpis_api_performance_http'
+                        - 'files_device_screenshots'
+                        - 'files_device_screen_record'
+                        - 'files_har'
+                        - 'files_device_cpu_metrics'
+                        - 'files_device_memory_metrics'
+                        - 'files_device_battery_metrics'
+                        - 'files_device_graphics_metrics'
+                        - 'files_device_network_packets'
+                        - 'files_device_debug_logs'
+                        - 'files_test_execution_output'
+                        - 'files_test_framework_output'
+                        - 'kpis_system_performance_cpu_metrics'
+                        - 'kpis_system_performance_memory_metrics'
+                        - 'kpis_system_performance_battery_metrics'
+                        - 'kpis_app_performance_graphics_metrics'
+        Returns:
+            section_info(dict): section information
+        """
         analytics = TestAnalytics(client=self)
-        response = analytics.download_test_screenshot(test_id=test_id, file_name=image_name, output_file=file_name)
+        response = analytics.get_test_execution_info_by_section(test_id=test_id, section=section)
         return response
 
-    def download_test_log(self, test_id=None, log_name=None, file_name=None):
+    def download_by_section(self, test_id=None, section=None):
+        """ Download test analytics information as a json file, raw file, list of raw files
+
+        Args:
+            test_id(str): test id
+            section(str): supported info section names
+                        - 'basic_test_info'                         - json
+                        - 'test_configuration'                      - json
+                        - 'test_cases'                              - json
+                        - 'events'                                  - json
+                        - 'kpis_user_experience'                    - json
+                        - 'kpis_api_performance_http'               - json
+                        - 'files_device_screenshots'                - png
+                        - 'files_device_screen_record'              - mp4
+                        - 'files_har'                               - har
+                        - 'files_device_cpu_metrics'                - csv
+                        - 'files_device_memory_metrics'             - csv
+                        - 'files_device_battery_metrics'            - csv
+                        - 'files_device_graphics_metrics'           - csv
+                        - 'files_device_network_packets'            - pcap
+                        - 'files_device_debug_logs'                 - log
+                        - 'files_test_execution_output'             - log
+                        - 'files_test_framework_output'             - log | xml | json | html
+                        - 'kpis_system_performance_cpu_metrics'     - json
+                        - 'kpis_system_performance_memory_metrics'  - json
+                        - 'kpis_system_performance_battery_metrics' - json
+                        - 'kpis_app_performance_graphics_metrics'   - json
+        Returns:
+            message(str) : 'Success: File filename downloaded successfully.'
+                        : 'Failure: Error in downloading file filename.'
+        """
         analytics = TestAnalytics(client=self)
-        response = analytics.download_test_output_file(test_id=test_id, file_name=log_name, output_file=file_name)
+        response = analytics.download_by_section(test_id=test_id, section=section)
         return response
```

### Comparing `mozark_sdk-0.4/mozark_sdk/schedule.py` & `mozark-sdk-0.5/mozark-sdk/schedule.py`

 * *Files identical despite different names*

### Comparing `mozark_sdk-0.4/mozark_sdk/user.py` & `mozark-sdk-0.5/mozark-sdk/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,12 +18,11 @@
             },
             "AuthFlow": "USER_PASSWORD_AUTH",
             "ClientId": self.config.get("client_id")
         }
 
         resp = requests.post(login_url, json=data, headers=new_headers)
         api_access_token = resp.json()['AuthenticationResult']['IdToken']
-        self.config["api_access_token"] = api_access_token
-        return resp.status_code, resp.text
+        return api_access_token
 
     def logout(self):
         pass
```

### Comparing `mozark_sdk-0.4/mozark_sdk.egg-info/PKG-INFO` & `mozark-sdk-0.5/mozark_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozark-sdk
-Version: 0.4
+Version: 0.5
 Summary: Automation test APIs
 Home-page: https://mozark.ai
 Author: Mozark
 Author-email: mozark-aws-staging@mozark.ai
 License: MIT
 Keywords: MOZARK,AUTOMATION,EXPERIENCE
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mozark_sdk-0.4/setup.py` & `mozark-sdk-0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from distutils.core import setup
+# from distutils.core import setup
+from setuptools import setup
 
 setup(
-    name='mozark_sdk',
-    packages=['mozark_sdk'],
-    version='0.4',
+    name='mozark-sdk',
+    packages=['mozark-sdk'],
+    version='0.5',
     license='MIT',
     description='Automation test APIs',
     author='Mozark',
     author_email='mozark-aws-staging@mozark.ai',
     url='https://mozark.ai',
     # download_url='https://github.com/user/reponame/archive/v_01.tar.gz',  # I explain this later on
+    # long_description_content_type = "text/markdown",
     keywords=['MOZARK', 'AUTOMATION', 'EXPERIENCE'],
     install_requires=[
         'configparser==5.3.0',
         'requests==2.28.1'
     ],
+    description_file='README.md',
     classifiers=[
         'Development Status :: 3 - Alpha',
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',  # Define that your audience are developers
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',  # Again, pick a license
         'Programming Language :: Python :: 3',  # Specify which pyhton versions that you want to support
```

