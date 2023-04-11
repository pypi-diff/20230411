# Comparing `tmp/elevenlabslib-0.4.1.tar.gz` & `tmp/elevenlabslib-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.4.1.tar", last modified: Thu Mar 30 11:09:40 2023, max compression
+gzip compressed data, was "elevenlabslib-0.4.2.tar", last modified: Tue Apr 11 21:11:05 2023, max compression
```

## Comparing `elevenlabslib-0.4.1.tar` & `elevenlabslib-0.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 11:09:40.365216 elevenlabslib-0.4.1/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     2484 2023-03-30 11:09:40.364216 elevenlabslib-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1905 2023-03-20 00:23:33.000000 elevenlabslib-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 11:09:40.350216 elevenlabslib-0.4.1/elevenlabslib/
--rw-rw-rw-   0        0        0     3858 2023-03-18 16:40:33.000000 elevenlabslib-0.4.1/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     2635 2023-03-18 16:40:43.000000 elevenlabslib-0.4.1/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    14203 2023-03-25 13:50:30.000000 elevenlabslib-0.4.1/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    32224 2023-03-25 13:50:30.000000 elevenlabslib-0.4.1/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      445 2023-03-25 13:50:30.000000 elevenlabslib-0.4.1/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     5624 2023-03-30 11:08:35.000000 elevenlabslib-0.4.1/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-03-30 11:09:40.363216 elevenlabslib-0.4.1/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     2484 2023-03-30 11:09:40.000000 elevenlabslib-0.4.1/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-03-30 11:09:40.000000 elevenlabslib-0.4.1/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 11:09:40.000000 elevenlabslib-0.4.1/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-03-30 11:09:40.000000 elevenlabslib-0.4.1/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-30 11:09:40.000000 elevenlabslib-0.4.1/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      777 2023-03-30 11:08:59.000000 elevenlabslib-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-30 11:09:40.365216 elevenlabslib-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 21:11:05.285869 elevenlabslib-0.4.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     2484 2023-04-11 21:11:05.285869 elevenlabslib-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1905 2023-03-20 00:23:33.000000 elevenlabslib-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 21:11:05.271868 elevenlabslib-0.4.2/elevenlabslib/
+-rw-rw-rw-   0        0        0     3858 2023-03-18 16:40:33.000000 elevenlabslib-0.4.2/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     2635 2023-03-18 16:40:43.000000 elevenlabslib-0.4.2/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    14203 2023-03-25 13:50:30.000000 elevenlabslib-0.4.2/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    31721 2023-04-11 21:06:56.000000 elevenlabslib-0.4.2/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      445 2023-03-25 13:50:30.000000 elevenlabslib-0.4.2/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     5624 2023-03-30 11:08:35.000000 elevenlabslib-0.4.2/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-11 21:11:05.284868 elevenlabslib-0.4.2/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     2484 2023-04-11 21:11:05.000000 elevenlabslib-0.4.2/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-04-11 21:11:05.000000 elevenlabslib-0.4.2/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 21:11:05.000000 elevenlabslib-0.4.2/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-11 21:11:05.000000 elevenlabslib-0.4.2/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 21:11:05.000000 elevenlabslib-0.4.2/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      777 2023-04-11 21:08:00.000000 elevenlabslib-0.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 21:11:05.285869 elevenlabslib-0.4.2/setup.cfg
```

### Comparing `elevenlabslib-0.4.1/LICENSE` & `elevenlabslib-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.4.1/PKG-INFO` & `elevenlabslib-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.4.1
+Version: 0.4.2
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `elevenlabslib-0.4.1/README.md` & `elevenlabslib-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.4.1/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.4.2/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.4.1/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.4.2/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.4.1/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.4.2/elevenlabslib/ElevenLabsUser.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.4.1/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.4.2/elevenlabslib/ElevenLabsVoice.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,14 @@
         """
         self._linkedUser = linkedUser
         # This is the name at the time the object was created. It won't be updated.
         # (Useful to iterate over all voices to find one with a specific name without spamming the API)
         self.initialName = voiceData["name"]
         self._voiceID = voiceData["voice_id"]
         self._category = voiceData["category"]
-        self._labels = voiceData["labels"]
 
     def _generate_payload(self, prompt:str, stability:Optional[float]=None, similarity_boost:Optional[float]=None) -> dict:
         """
         Generates the payload for the text-to-speech API call.
 
         Args:
             prompt (str): The prompt to generate speech for.
@@ -216,34 +215,50 @@
 
         Returns:
             str: The name of the voice.
         """
         # We don't store the name OR the settings, as they can be changed externally.
         response = _api_get("/voices/" + self._voiceID + "/settings", self._linkedUser.headers)
         return response.json()
+    def get_info(self) -> dict:
+        """
+        Get the raw metadata for the voice.
+        Returns:
+            dict: A dict containing all the metadata
+        """
+        response = _api_get("/voices/" + self._voiceID, self._linkedUser.headers)
+        return response.json()
 
+    #I've settled on only providing dedicated getters for the (imo) most common fields, name, description and labels. For everything else, there's the get_info method.
     def get_name(self) -> str:
         """
         Get the name of the current voice.
 
         Returns:
             str: The name of the voice.
         """
-        response = _api_get("/voices/" + self._voiceID, self._linkedUser.headers)
-        return response.json()["name"]
+        return self.get_info()["name"]
+
+    def get_description(self) -> str|None:
+        """
+        Get the description.
+
+        Returns:
+            str: The description for the voice.
+        """
+        return self.get_info()["description"]
 
     def get_preview_url(self) -> str|None:
         """
         Get the preview URL of the current voice.
 
         Returns:
             str|None: The preview URL of the voice, or None if it doesn't exist.
         """
-        response = _api_get("/voices/" + self._voiceID, self._linkedUser.headers)
-        return response.json()["preview_url"]
+        return self.get_info()["preview_url"]
 
     def edit_settings(self, stability:float=None, similarity_boost:float=None):
         """
         Edit the settings of the current voice.
 
         Args:
             stability (float, optional): The stability of the voice. If None, the current stability setting will be used. Defaults to None.
@@ -261,18 +276,14 @@
             raise ValueError("Please provide a value between 0 and 1.")
         payload = {"stability": stability, "similarity_boost": similarity_boost}
         _api_json("/voices/" + self._voiceID + "/settings/edit", self._linkedUser.headers, jsonData=payload)
 
     @property
     def category(self):
         return self._category
-    @property
-    def labels(self):
-        return self._labels
-
     # Since the same voice can be available for multiple users, we allow the user to change which API key is used.
     @property
     def linkedUser(self):
         """
         Returns the user currently linked to the voice, whose API key will be used.
 
         Returns:
@@ -542,30 +553,37 @@
         return readData
 
 
 class ElevenLabsDesignedVoice(ElevenLabsVoice):
     def __init__(self, voiceData, linkedUser: ElevenLabsUser):
         super().__init__(voiceData, linkedUser)
 
-    def edit_voice(self, newName:str = None, newLabels:dict[str, str] = None):
+    def edit_voice(self, newName:str = None, newLabels:dict[str, str] = None, description:str = None):
         """
         Edit the name/labels of the voice.
 
         Args:
-            newName (str): The new name for the voice.
-            newLabels (str): The new labels for the voice.
-        """
-        if newName is None:
-            newName = self.get_name()
-        payload = {"name": newName}
-
+            newName (str): The new name
+            newLabels (str): The new labels
+            description (str): The new description
+        """
+        currentInfo = self.get_info()
+        payload = {
+            "name": currentInfo["name"],
+            "labels": currentInfo["labels"],
+            "description": currentInfo["description"]
+        }
+        if newName is not None:
+            payload["name"] = newName
         if newLabels is not None:
             if len(newLabels.keys()) > 5:
                 raise ValueError("Too many labels! The maximum amount is 5.")
             payload["labels"] = newLabels
+        if description is not None:
+            payload["description"] = description
         _api_multipart("/voices/" + self._voiceID + "/edit", self._linkedUser.headers, data=payload)
     def delete_voice(self):
         """
         This function deletes the current voice.
 
         Returns:
             None
@@ -576,46 +594,26 @@
         """
         if self._category == "premade":
             raise RuntimeError("Cannot delete premade voices!")
         response = _api_del("/voices/" + self._voiceID, self._linkedUser.headers)
         self._voiceID = ""
 
 
-class ElevenLabsClonedVoice(ElevenLabsVoice):
+class ElevenLabsClonedVoice(ElevenLabsDesignedVoice):
     def __init__(self, voiceData, linkedUser: ElevenLabsUser):
         super().__init__(voiceData, linkedUser)
 
-
     def get_samples(self) -> list[ElevenLabsSample]:
-        response = _api_get("/voices/" + self._voiceID, self._linkedUser.headers)
         outputList = list()
-        samplesData = response.json()["samples"]
+        samplesData = self.get_info()["samples"]
         from elevenlabslib.ElevenLabsSample import ElevenLabsSample
         for sampleData in samplesData:
             outputList.append(ElevenLabsSample(sampleData, self))
         return outputList
 
-    def edit_voice(self, newName:str = None, newLabels:dict[str, str] = None):
-        """
-        Edit the name/labels of the voice.
-
-        Args:
-            newName (str): The new name for the voice.
-            newLabels (str): The new labels for the voice.
-        """
-        if newName is None:
-            newName = self.get_name()
-        payload = {"name": newName}
-
-        if newLabels is not None:
-            if len(newLabels.keys()) > 5:
-                raise ValueError("Too many labels! The maximum amount is 5.")
-            payload["labels"] = newLabels
-        _api_multipart("/voices/" + self._voiceID + "/edit", self._linkedUser.headers, data=payload)
-
     def add_samples_by_path(self, samples:list[str]):
         """
         This function adds samples to the current voice by their file paths.
 
         Args:
             samples (list[str]): A list of file paths to the sample audio files.
 
@@ -654,24 +652,8 @@
             raise ValueError("Please add at least one sample!")
 
         payload = {"name":self.get_name()}
         files = list()
         for fileName, fileBytes in samples.items():
             files.append(("files", (fileName, io.BytesIO(fileBytes))))
 
-        _api_multipart("/voices/" + self._voiceID + "/edit", self._linkedUser.headers, data=payload, filesData=files)
-
-    def delete_voice(self):
-        """
-        This function deletes the current voice.
-
-        Returns:
-            None
-
-        Raises:
-            RuntimeError: If the voice is a premade voice.
-
-        """
-        if self._category == "premade":
-            raise RuntimeError("Cannot delete premade voices!")
-        response = _api_del("/voices/" + self._voiceID, self._linkedUser.headers)
-        self._voiceID = ""
+        _api_multipart("/voices/" + self._voiceID + "/edit", self._linkedUser.headers, data=payload, filesData=files)
```

### Comparing `elevenlabslib-0.4.1/elevenlabslib/helpers.py` & `elevenlabslib-0.4.2/elevenlabslib/helpers.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.4.1/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.4.2/elevenlabslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.4.1
+Version: 0.4.2
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `elevenlabslib-0.4.1/pyproject.toml` & `elevenlabslib-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```

