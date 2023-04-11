# Comparing `tmp/citric-0.7.0.tar.gz` & `tmp/citric-0.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citric-0.7.0.tar", max compression
+gzip compressed data, was "citric-0.7.1b1.tar", max compression
```

## Comparing `citric-0.7.0.tar` & `citric-0.7.1b1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2023-03-31 20:54:36.007234 citric-0.7.0/LICENSE
--rw-r--r--   0        0        0     4491 2023-03-31 20:54:36.007234 citric-0.7.0/README.md
--rw-r--r--   0        0        0     4221 2023-03-31 20:54:36.011234 citric-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      399 2023-03-31 20:54:36.011234 citric-0.7.0/src/citric/__init__.py
--rw-r--r--   0        0        0     1511 2023-03-31 20:54:36.011234 citric-0.7.0/src/citric/_compat.py
--rw-r--r--   0        0        0    42865 2023-03-31 20:54:36.011234 citric-0.7.0/src/citric/client.py
--rw-r--r--   0        0        0     1739 2023-03-31 20:54:36.011234 citric-0.7.0/src/citric/enums.py
--rw-r--r--   0        0        0     1345 2023-03-31 20:54:36.011234 citric-0.7.0/src/citric/exceptions.py
--rw-r--r--   0        0        0     1135 2023-03-31 20:54:36.011234 citric-0.7.0/src/citric/method.py
--rw-r--r--   0        0        0     1171 2023-03-31 20:54:36.011234 citric-0.7.0/src/citric/objects.py
--rw-r--r--   0        0        0        0 2023-03-31 20:54:36.011234 citric-0.7.0/src/citric/py.typed
--rw-r--r--   0        0        0     6705 2023-03-31 20:54:36.011234 citric-0.7.0/src/citric/session.py
--rw-r--r--   0        0        0    13839 2023-03-31 20:54:36.011234 citric-0.7.0/src/citric/types.py
--rw-r--r--   0        0        0     6804 1970-01-01 00:00:00.000000 citric-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-11 05:24:40.664486 citric-0.7.1b1/LICENSE
+-rw-r--r--   0        0        0     4491 2023-04-11 05:24:40.664486 citric-0.7.1b1/README.md
+-rw-r--r--   0        0        0     4224 2023-04-11 05:24:40.668486 citric-0.7.1b1/pyproject.toml
+-rw-r--r--   0        0        0      399 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/__init__.py
+-rw-r--r--   0        0        0     1511 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/_compat.py
+-rw-r--r--   0        0        0    44877 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/client.py
+-rw-r--r--   0        0        0     1739 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/enums.py
+-rw-r--r--   0        0        0     1345 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/exceptions.py
+-rw-r--r--   0        0        0     1135 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/method.py
+-rw-r--r--   0        0        0     1171 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/objects.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/py.typed
+-rw-r--r--   0        0        0     6984 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/session.py
+-rw-r--r--   0        0        0    13839 2023-04-11 05:24:40.668486 citric-0.7.1b1/src/citric/types.py
+-rw-r--r--   0        0        0     6806 1970-01-01 00:00:00.000000 citric-0.7.1b1/PKG-INFO
```

### Comparing `citric-0.7.0/LICENSE` & `citric-0.7.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `citric-0.7.0/README.md` & `citric-0.7.1b1/README.md`

 * *Files identical despite different names*

### Comparing `citric-0.7.0/pyproject.toml` & `citric-0.7.1b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 homepage = 'https://github.com/edgarrmondragon/citric'
 keywords = ["limesurvey", "json-rpc"]
 license = "MIT"
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 name = "citric"
 readme = "README.md"
 repository = 'https://github.com/edgarrmondragon/citric'
-version = "0.7.0"
+version = "0.7.1-b1"
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/edgarrmondragon/citric/issues"
 
 [tool.poetry.dependencies]
 importlib_metadata = {version = ">=1.6", python = "<3.8"}
 python = "^3.7.0"
```

### Comparing `citric-0.7.0/src/citric/_compat.py` & `citric-0.7.1b1/src/citric/_compat.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.0/src/citric/client.py` & `citric-0.7.1b1/src/citric/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING, TypeVar
 
 import requests
 
 from citric import enums
-from citric._compat import future
 from citric.session import Session
 
 if TYPE_CHECKING:
     import sys
     from os import PathLike
     from types import TracebackType
     from typing import Any, BinaryIO, Generator, Iterable, Mapping, Sequence
@@ -102,14 +101,17 @@
         requests_session: A `requests.Session`_ object.
         auth_plugin: Name of the :ls_manual:`plugin <Authentication_plugins>` to use for
             authentication. For example,
             :ls_manual:`AuthLDAP <Authentication_plugins#LDAP>`. Defaults to using the
             :ls_manual:`internal database <Authentication_plugins#Internal_database>`
             (``"Authdb"``).
 
+    .. versionadded:: 0.0.6
+       Support Auth plugins with the ``auth_plugin`` parameter.
+
     .. _requests.Session:
         https://requests.readthedocs.io/en/latest/api/#request-sessions
     """
 
     session_class = Session
 
     def __init__(
@@ -156,25 +158,29 @@
         """Get fieldmap for a survey.
 
         Args:
             survey_id: ID of survey to get fieldmap for.
 
         Returns:
             Dictionary mapping response keys to LimeSurvey internal representation.
+
+        .. versionadded:: 0.3.0
         """
         return self.__session.get_fieldmap(survey_id)
 
     def activate_survey(self, survey_id: int) -> types.OperationStatus:
         """Activate a survey.
 
         Args:
             survey_id: ID of survey to be activated.
 
         Returns:
             Status and plugin feedback.
+
+        .. versionadded:: 0.0.1
         """
         return self.__session.activate_survey(survey_id)
 
     def activate_tokens(
         self,
         survey_id: int,
         attributes: list[int] | None = None,
@@ -185,27 +191,31 @@
 
         Args:
             survey_id: ID of survey to be activated.
             attributes: Optional list of participant attributes numbers to be activated.
 
         Returns:
             Status message.
+
+        .. versionadded:: 0.0.1
         """
         return self.__session.activate_tokens(survey_id, attributes or [])
 
     def add_language(self, survey_id: int, language: str) -> types.OperationStatus:
         """Add a survey language.
 
         Args:
             survey_id: ID of the Survey for which a language will be added.
             language: A valid language shortcut to add to the current Survey. If the
                 language already exists no error will be given.
 
         Returns:
             Status message.
+
+        .. versionadded:: 0.0.10
         """
         return self.__session.add_language(survey_id, language)
 
     def add_participants(
         self,
         survey_id: int,
         *,
@@ -217,22 +227,25 @@
         Args:
             survey_id: Survey to add participants to.
             participant_data: Information to create participants with.
             create_tokens: Whether to create the participants with tokens.
 
         Returns:
             Information of newly created participants.
+
+        .. versionadded:: 0.0.1
+        .. versionchanged:: 0.4.0
+           Use keyword-only arguments.
         """
         return self.__session.add_participants(
             survey_id,
             participant_data,
             create_tokens,
         )
 
-    @future("6.0")
     def add_quota(
         self,
         survey_id: int,
         name: str,
         limit: int,
         *,
         active: bool = True,
@@ -255,15 +268,15 @@
             url: URL to redirect the respondent to when the limit is reached.
             url_description: Description of the URL.
 
         Returns:
             ID of the newly created quota.
 
         .. versionadded:: 0.6.0
-        .. future:: 6.0
+        .. minlimesurvey:: 6.0.0
         """
         return self.session.add_quota(
             survey_id,
             name,
             limit,
             active,
             enums.QuotaAction(action),
@@ -287,14 +300,16 @@
             title: Title of the new Survey.
             language: Default language of the Survey.
             survey_format: Question appearance format (A, G or S) for "All on one page",
                 "Group by Group", "Single questions", default to group by group (G).
 
         Returns:
             The new survey ID.
+
+        .. versionadded:: 0.0.10
         """
         return self.__session.add_survey(
             survey_id,
             title,
             language,
             enums.NewSurveyType(survey_format),
         )
@@ -308,14 +323,16 @@
 
         Args:
             survey_id: Survey to delete participants to.
             participant_ids: Participant IDs to be deleted.
 
         Returns:
             Information of removed participants.
+
+        .. versionadded:: 0.0.1
         """
         return self.__session.delete_participants(
             survey_id,
             participant_ids,
         )
 
     def _get_question_mapping(
@@ -381,14 +398,16 @@
         Args:
             survey_id: ID of the Survey to add the group.
             title: Name of the group.
             description: Optional description of the group.
 
         Returns:
             The id of the new group.
+
+        .. versionadded:: 0.0.8
         """
         return self.__session.add_group(survey_id, title, description)
 
     def _add_response(self, survey_id: int, response_data: Mapping[str, Any]) -> int:
         """Add a single response to a survey.
 
         Args:
@@ -406,14 +425,16 @@
 
         Args:
             survey_id: Survey to add the response to.
             response_data: Single response as a mapping.
 
         Returns:
             ID of the new response.
+
+        .. versionadded:: 0.0.1
         """
         # Transform question codes to the format LimeSurvey expects
         questions = self._get_question_mapping(survey_id)
         data = self._map_response_keys(response_data, questions)
         return self._add_response(survey_id, data)
 
     def add_responses(
@@ -425,14 +446,16 @@
 
         Args:
             survey_id: Survey to add the response to.
             responses: Iterable of survey responses.
 
         Returns:
             IDs of the new responses.
+
+        .. versionadded:: 0.0.1
         """
         ids = []
         questions = self._get_question_mapping(survey_id)
         for response in responses:
             data = self._map_response_keys(response, questions)
             response_id = self._add_response(survey_id, data)
             ids.append(response_id)
@@ -443,28 +466,32 @@
 
         Args:
             survey_id: Survey to update the response in.
             response_data: Response data to update.
 
         Returns:
             True if the response was updated, False otherwise.
+
+        .. versionadded:: 0.2.0
         """
         questions = self._get_question_mapping(survey_id)
         data = self._map_response_keys(response_data, questions)
         return self.__session.update_response(survey_id, data)
 
     def copy_survey(self, survey_id: int, name: str) -> dict[str, Any]:
         """Copy a survey.
 
         Args:
             survey_id: ID of the source survey.
             name: Name of the new survey.
 
         Returns:
             Dictionary of status message and the new survey ID.
+
+        .. versionadded:: 0.0.10
         """
         return self.__session.copy_survey(survey_id, name)
 
     def import_cpdb_participants(
         self,
         participants: Sequence[Participant],
         *,
@@ -491,43 +518,45 @@
 
         Args:
             survey_id: ID of the Survey that the group belongs to.
             group_id: ID of the group to delete.
 
         Returns:
             ID of the deleted group.
+
+        .. versionadded:: 0.0.10
         """
         return self.__session.delete_group(survey_id, group_id)
 
     def delete_language(self, survey_id: int, language: str) -> types.OperationStatus:
         """Delete a language from a survey.
 
-        Requires at LimeSurvey >= 5.3.4.
-
         Args:
             survey_id: ID of the Survey for which a language will be deleted from.
             language: Language to delete.
 
         Returns:
             Status message.
+
+        .. versionadded:: 0.0.12
+        .. minlimesurvey:: 5.3.4
         """
         return self.__session.delete_language(survey_id, language)
 
-    @future("6.0")
     def delete_quota(self, quota_id: int) -> types.OperationStatus:
         """Delete a LimeSurvey quota.
 
         Args:
             quota_id: ID of the quota to delete.
 
         Returns:
             True if the quota was deleted.
 
         .. versionadded:: 0.6.0
-        .. future:: 6.0
+        .. minlimesurvey:: 6.0.0
         """
         return self.session.delete_quota(quota_id)
 
     def delete_response(
         self,
         survey_id: int,
         response_id: int,
@@ -536,40 +565,43 @@
 
         Args:
             survey_id: ID of the survey the response belongs to.
             response_id: ID of the response to delete.
 
         Returns:
             Status message.
+
+        .. versionadded:: 0.0.2
         """
         return self.__session.delete_response(survey_id, response_id)
 
     def delete_question(self, question_id: int) -> int:
         """Delete a survey.
 
-        Requires at least LimeSurvey 5.3.19+220607.
-
-        TODO: Add links to issue, PR, etc.
-
         Args:
             question_id: ID of Question to delete.
 
         Returns:
             ID of the deleted question.
+
+        .. versionadded:: 0.1.0
+        .. minlimesurvey:: 5.3.19
         """
         return self.__session.delete_question(question_id)
 
     def delete_survey(self, survey_id: int) -> types.OperationStatus:
         """Delete a survey.
 
         Args:
             survey_id: Survey to delete.
 
         Returns:
             Status message.
+
+        .. versionadded:: 0.0.1
         """
         return self.__session.delete_survey(survey_id)
 
     def export_responses(
         self,
         survey_id: int,
         *,
@@ -595,14 +627,19 @@
             response_type: Export long or short text responses.
             from_response_id: First response to export.
             to_response_id: Last response to export.
             fields: Which response fields to export. If none, exports all fields.
 
         Returns:
             Content bytes of exported to file.
+
+        .. versionadded:: 0.0.1
+
+        .. versionchanged:: 0.0.2
+           Return raw bytes instead of number of bytes written.
         """
         if token is None:
             return base64.b64decode(
                 self.__session.export_responses(
                     survey_id,
                     enums.ResponsesExportFormat(file_format),
                     language,
@@ -658,14 +695,16 @@
             response_type: Export long or short text responses.
             from_response_id: First response to export.
             to_response_id: Last response to export.
             fields: Which response fields to export. If none, exports all fields.
 
         Returns:
             Bytes length written to file.
+
+        .. versionadded:: 0.0.10
         """
         with Path(filename).open("wb") as f:
             return f.write(
                 self.export_responses(
                     survey_id,
                     token=token,
                     file_format=file_format,
@@ -697,14 +736,16 @@
             language: Language of the survey to use (default from Survey).
                 Defaults to None.
             graph: Export graphs. Defaults to False.
             group_ids: Question groups to generate statistics from. Defaults to None.
 
         Returns:
             File contents.
+
+        .. versionadded:: 0.0.10
         """
         return base64.b64decode(
             self.session.export_statistics(
                 survey_id,
                 enums.StatisticsExportFormat(file_format),
                 language,
                 "yes" if graph else "no",
@@ -761,14 +802,16 @@
             survey_id: ID of the Survey.
             period: Granularity level for aggregation submission counts.
             start: Start datetime.
             end: End datetime.
 
         Returns:
             Mapping of days/hours to submission counts.
+
+        .. versionadded:: 0.0.10
         """
         return self.session.export_timeline(
             survey_id,
             enums.TimelineAggregationPeriod(period),
             start.isoformat(),
             end.isoformat()
             if end
@@ -787,14 +830,16 @@
         Args:
             group_id: ID of the group to get properties of.
             settings: Properties to get, default to all.
             language: Parameter language for multilingual groups.
 
         Returns:
             Dictionary of group properties.
+
+        .. versionadded:: 0.0.10
         """
         return self.__session.get_group_properties(group_id, settings, language)
 
     def get_language_properties(
         self,
         survey_id: int,
         *,
@@ -806,14 +851,16 @@
         Args:
             survey_id: ID of the survey.
             settings: Properties to get, default to all.
             language: Parameter language for multilingual questions.
 
         Returns:
             Dictionary of survey language properties.
+
+        .. versionadded:: 0.0.10
         """
         return self.__session.get_language_properties(survey_id, settings, language)
 
     def get_participant_properties(
         self,
         survey_id: int,
         query: dict[str, Any] | int,
@@ -825,14 +872,16 @@
             survey_id: Survey to get participants properties.
             query: Mapping of properties to query participants, or the token id
                 as an integer.
             properties: Which participant properties to retrieve.
 
         Returns:
             List of participants properties.
+
+        .. versionadded:: 0.0.1
         """
         return self.__session.get_participant_properties(survey_id, query, properties)
 
     def get_question_properties(
         self,
         question_id: int,
         *,
@@ -844,18 +893,19 @@
         Args:
             question_id: ID of the question to get properties.
             settings: Properties to get, default to all.
             language: Parameter language for multilingual questions.
 
         Returns:
             Dictionary of question properties.
+
+        .. versionadded:: 0.0.10
         """
         return self.__session.get_question_properties(question_id, settings, language)
 
-    @future("6.0")
     def get_quota_properties(
         self,
         quota_id: int,
         settings: list[str] | None = None,
         language: str | None = None,
     ) -> types.QuotaProperties:
         """Get properties of a LimeSurvey quota.
@@ -865,15 +915,15 @@
             settings: Properties to get, default to all.
             language: Parameter language for multilingual quotas.
 
         Returns:
             Quota properties.
 
         .. versionadded:: 0.6.0
-        .. future:: 6.0
+        .. minlimesurvey:: 6.0.0
         """
         return self.session.get_quota_properties(quota_id, settings, language)
 
     def get_response_ids(
         self,
         survey_id: int,
         token: str,
@@ -882,94 +932,107 @@
 
         Args:
             survey_id: Survey to get responses from.
             token: Participant for which to get response IDs.
 
         Returns:
             A list of response IDs.
+
+        .. versionadded:: 0.0.1
         """
         return self.__session.get_response_ids(survey_id, token)
 
-    @future("6.0")
     def get_available_site_settings(self) -> list[str]:
         """Get all available site settings.
 
         Returns:
             A list of all the available site settings.
 
         .. versionadded:: 0.6.0
-        .. future:: 6.0
+        .. minlimesurvey:: 6.0.0
         """
         return self.session.get_available_site_settings()
 
     def _get_site_setting(self, setting_name: str) -> types.Result:
         """Get a global setting.
 
         Function to query site settings. Can only be used by super administrators.
 
         Args:
             setting_name: Name of the setting to get.
 
         Returns:
             The requested setting value.
+
+        .. versionadded:: 0.0.1
         """
         return self.__session.get_site_settings(setting_name)
 
     def get_default_theme(self) -> str:
         """Get the global default theme.
 
         Calls :rpc_method:`get_site_settings("defaulttheme") <get_site_settings>`.
 
         Returns:
             The name of the theme.
+
+        .. versionadded:: 0.0.1
         """
         return self._get_site_setting("defaulttheme")
 
     def get_site_name(self) -> str:
         """Get the site name.
 
         Calls :rpc_method:`get_site_settings("sitename") <get_site_settings>`.
 
         Returns:
             The name of the site.
+
+        .. versionadded:: 0.0.1
         """
         return self._get_site_setting("sitename")
 
     def get_default_language(self) -> str:
         """Get the default site language.
 
         Calls :rpc_method:`get_site_settings("defaultlang") <get_site_settings>`.
 
         Returns:
             A string representing the language.
+
+        .. versionadded:: 0.0.1
         """
         return self._get_site_setting("defaultlang")
 
     def get_available_languages(self) -> list[str] | None:
         """Get the list of available languages.
 
         Calls
         :rpc_method:`get_site_settings("restrictToLanguages") <get_site_settings>`.
 
         Returns:
             Either a list of strings for the available languages or None if there are
             no restrictions.
+
+        .. versionadded:: 0.0.1
         """
         langs: str = self._get_site_setting("restrictToLanguages")
 
         return langs.split(" ") if langs else None
 
     def get_summary(self, survey_id: int) -> dict[str, int]:
         """Get survey summary.
 
         Args:
             survey_id: ID of the survey to get summary of.
 
         Returns:
             Mapping of survey statistics.
+
+        .. versionadded:: 0.0.10
         """
         return self.session.get_summary(survey_id)
 
     def get_survey_properties(
         self,
         survey_id: int,
         properties: Sequence[str] | None = None,
@@ -978,14 +1041,16 @@
 
         Args:
             survey_id: Survey to get properties.
             properties: Which survey properties to retrieve. If none, gets all fields.
 
         Returns:
             Dictionary of survey properties.
+
+        .. versionadded:: 0.0.1
         """
         return self.__session.get_survey_properties(survey_id, properties)
 
     def get_uploaded_files(
         self,
         survey_id: int,
         token: str | None = None,
@@ -994,14 +1059,16 @@
 
         Args:
             survey_id: Survey for which to download files.
             token: Optional participant token to filter uploaded files.
 
         Returns:
             Dictionary with uploaded files metadata.
+
+        .. versionadded:: 0.0.5
         """
         return self.__session.get_uploaded_files(survey_id, token)
 
     def get_uploaded_file_objects(
         self,
         survey_id: int,
         token: str | None = None,
@@ -1010,14 +1077,16 @@
 
         Args:
             survey_id: Survey for which to download files.
             token: Optional participant token to filter uploaded files.
 
         Yields:
             :class:`~citric.client.UploadedFile` objects.
+
+        .. versionadded:: 0.0.13
         """
         files_data = self.get_uploaded_files(survey_id, token)
         for file in files_data:
             metadata: dict = files_data[file]["meta"]
             question: dict = metadata.pop("question")
             content = base64.b64decode(files_data[file]["content"])
 
@@ -1040,14 +1109,16 @@
         Args:
             directory: Where to store the files.
             survey_id: Survey for which to download files.
             token: Optional participant token to filter uploaded files.
 
         Returns:
             List with the paths of downloaded files.
+
+        .. versionadded:: 0.0.1
         """
         dirpath = Path(directory)
 
         filepaths = []
         uploaded_files = self.get_uploaded_file_objects(survey_id, token=token)
 
         for file in uploaded_files:
@@ -1073,14 +1144,16 @@
         Args:
             file: File object.
             survey_id: The ID of the Survey that the question will belong to.
             file_type: Type of file. One of LSS, CSV, TXT and LSA.
 
         Returns:
             The ID of the new group.
+
+        .. versionadded:: 0.0.10
         """
         contents = base64.b64encode(file.read()).decode()
         return self.__session.import_group(
             survey_id,
             contents,
             enums.ImportGroupType(file_type),
         )
@@ -1100,14 +1173,16 @@
         Args:
             file: File object.
             survey_id: The ID of the Survey that the question will belong to.
             group_id: The ID of the Group that the question will belong to.
 
         Returns:
             The ID of the new question.
+
+        .. versionadded:: 0.0.8
         """
         contents = base64.b64encode(file.read()).decode()
         return self.__session.import_question(
             survey_id,
             group_id,
             contents,
             "lsq",
@@ -1129,14 +1204,18 @@
             file_type: Type of file. One of LSS, CSV, TXT and LSA.
             survey_name: Override the new survey name.
             survey_id: Desired ID of the new survey. A different ID will be used if
                 there is already a survey with this ID.
 
         Returns:
             The ID of the new survey.
+
+        .. versionadded:: 0.0.1
+        .. versionchanged:: 0.0.5
+           Accept a binary file object instead of a path.
         """
         contents = base64.b64encode(file.read()).decode()
         return self.__session.import_survey(
             contents,
             enums.ImportSurveyType(file_type),
             survey_name,
             survey_id,
@@ -1160,14 +1239,18 @@
             limit: Maximum number of participants to retrieve.
             unused: Retrieve partipants with unused tokens.
             attributes: Extra participant attributes to include in the result.
             conditions: Dictionary of conditions to limit the list.
 
         Returns:
             List of participants with basic information.
+
+        .. versionadded:: 0.0.1
+        .. versionchanged:: 0.4.0
+           Use keyword-only arguments.
         """
         return self.__session.list_participants(
             survey_id,
             start,
             limit,
             unused,
             attributes,
@@ -1175,14 +1258,16 @@
         )
 
     def list_users(self) -> list[dict[str, Any]]:
         """Get LimeSurvey users.
 
         Returns:
             List of users.
+
+        .. versionadded:: 0.0.3
         """
         return self.__session.list_users()
 
     def list_groups(
         self,
         survey_id: int,
         language: str | None = None,
@@ -1191,14 +1276,16 @@
 
         Args:
             survey_id: ID of the Survey containing the groups.
             language: Optional parameter language for multilingual groups.
 
         Returns:
             List of question groups.
+
+        .. versionadded:: 0.0.10
         """
         return self.__session.list_groups(survey_id, language)
 
     def list_questions(
         self,
         survey_id: int,
         group_id: int | None = None,
@@ -1209,54 +1296,59 @@
         Args:
             survey_id: Survey.
             group_id: Question group.
             language: Retrieve question text, description, etc. in this language.
 
         Returns:
             List of questions with basic information.
+
+        .. versionadded:: 0.0.1
         """
         return self.__session.list_questions(survey_id, group_id, language)
 
-    @future("6.0")
     def list_quotas(self, survey_id: int) -> list[types.QuotaListElement]:
         """Get all quotas for a LimeSurvey survey.
 
         Args:
             survey_id: ID of the survey to get quotas for.
 
         Returns:
             List of quotas.
 
         .. versionadded:: 0.6.0
-        .. future:: 6.0
+        .. minlimesurvey:: 6.0.0
         """
         return self.session.list_quotas(survey_id)
 
     def list_surveys(self, username: str | None = None) -> list[dict[str, Any]]:
         """Get all surveys or only those owned by a user.
 
         Args:
             username: Owner of the surveys to retrieve.
 
         Returns:
             List of surveys with basic information.
+
+        .. versionadded:: 0.0.1
         """
         return self.__session.list_surveys(username)
 
     def list_survey_groups(
         self,
         username: str | None = None,
     ) -> list[dict[str, Any]]:
         """Get all survey groups or only those owned by a user.
 
         Args:
             username: Owner of the survey groups to retrieve.
 
         Returns:
             List of survey groups with basic information.
+
+        .. versionadded:: 0.0.2
         """
         return self.__session.list_survey_groups(username)
 
     def set_group_properties(
         self,
         group_id: int,
         **properties: Unpack[types.GroupProperties],
@@ -1265,14 +1357,16 @@
 
         Args:
             group_id: ID of the group.
             properties: Properties to set.
 
         Returns:
             Mapping of property names to whether they were set successfully.
+
+        .. versionadded:: 0.0.11
         """
         return self.session.set_group_properties(group_id, properties)
 
     def set_language_properties(
         self,
         survey_id: int,
         language: str | None = None,
@@ -1283,14 +1377,16 @@
         Args:
             survey_id: ID of the survey for which to set the language properties.
             language: Language code.
             properties: Properties to set.
 
         Returns:
             Mapping with status and updated properties.
+
+        .. versionadded:: 0.0.11
         """
         return self.session.set_language_properties(survey_id, properties, language)
 
     def set_participant_properties(
         self,
         survey_id: int,
         token_query_properties: Mapping[str, Any] | int,
@@ -1302,14 +1398,16 @@
             survey_id: ID of the survey to which the participant belongs.
             token_query_properties: Dictionary of properties to match the participant
                 or token ID.
             token_data: Properties to set.
 
         Returns:
             New participant properties.
+
+        .. versionadded:: 0.0.11
         """
         return self.session.set_participant_properties(
             survey_id,
             token_query_properties,
             token_data,
         )
 
@@ -1324,14 +1422,16 @@
         Args:
             question_id: ID of the question to set the properties of.
             language: Language code.
             properties: Properties to set.
 
         Returns:
             Mapping of property names to whether they were set successfully.
+
+        .. versionadded:: 0.0.11
         """
         return self.session.set_question_properties(question_id, properties, language)
 
     def set_quota_properties(
         self,
         quota_id: int,
         **properties: Unpack[types.QuotaProperties],
@@ -1360,14 +1460,16 @@
 
         Args:
             survey_id: ID of the survey to set the properties of.
             properties: Properties to set.
 
         Returns:
             Mapping of property names to whether they were set successfully.
+
+        .. versionadded:: 0.0.11
         """
         return self.session.set_survey_properties(survey_id, properties)
 
     def upload_file_object(
         self,
         survey_id: int,
         field: str,
@@ -1380,14 +1482,16 @@
             survey_id: ID of the survey to upload the file to.
             field: Field name to upload the file to.
             filename: Name of the file to upload.
             file: File-like object to upload.
 
         Returns:
             File metadata with final upload path.
+
+        .. versionadded:: 0.0.14
         """
         contents = base64.b64encode(file.read()).decode()
         return self.session.upload_file(survey_id, field, filename, contents)
 
     def upload_file(
         self,
         survey_id: int,
@@ -1402,14 +1506,16 @@
             survey_id: ID of the survey to which the file belongs.
             field: Field to upload the file to.
             path: Path to the file to upload.
             filename: Optional filename override to use in LimeSurvey.
 
         Returns:
             File metadata with final upload path.
+
+        .. versionadded:: 0.0.14
         """
         path = Path(path)
         if filename is None:
             filename = path.name
 
         with Path(path).open("rb") as file:
             return self.upload_file_object(survey_id, field, filename, file)
```

### Comparing `citric-0.7.0/src/citric/enums.py` & `citric-0.7.1b1/src/citric/enums.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.0/src/citric/exceptions.py` & `citric-0.7.1b1/src/citric/exceptions.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.0/src/citric/method.py` & `citric-0.7.1b1/src/citric/method.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.0/src/citric/objects.py` & `citric-0.7.1b1/src/citric/objects.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.0/src/citric/session.py` & `citric-0.7.1b1/src/citric/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,24 @@
             authentication. For example,
             :ls_manual:`AuthLDAP <Authentication_plugins#LDAP>`. Defaults to using the
             :ls_manual:`internal database <Authentication_plugins#Internal_database>`
             (``"Authdb"``).
         json_encoder: A `JSON encoder class <JSONEncoder>` to use for encoding RPC
             parameters.
 
+    .. versionchanged:: 0.0.4
+       Replaced the ``requests_session_factory`` parameter with ``requests_session``.
+
+    .. versionadded:: 0.0.6
+       Support Auth plugins with the ``auth_plugin`` parameter.
+
+    .. versionadded:: 0.5.0
+       The ``json_encoder`` parameter.
+
+
     .. _requests.Session:
         https://requests.readthedocs.io/en/latest/api/#request-sessions
     .. _key: #citric.session.Session.key
     .. _closure: #citric.session.Session.close
     .. _JSONEncoder: https://docs.python.org/3/library/json.html#json.JSONEncoder
     """
```

### Comparing `citric-0.7.0/src/citric/types.py` & `citric-0.7.1b1/src/citric/types.py`

 * *Files identical despite different names*

### Comparing `citric-0.7.0/PKG-INFO` & `citric-0.7.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citric
-Version: 0.7.0
+Version: 0.7.1b1
 Summary: A client to the LimeSurvey Remote Control API 2, written in modern Python.
 Home-page: https://github.com/edgarrmondragon/citric
 License: MIT
 Keywords: limesurvey,json-rpc
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Maintainer: Edgar Ramírez-Mondragón
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: citric Version: 0.7.0 Summary: A client to the
+Metadata-Version: 2.1 Name: citric Version: 0.7.1b1 Summary: A client to the
 LimeSurvey Remote Control API 2, written in modern Python. Home-page: https://
 github.com/edgarrmondragon/citric License: MIT Keywords: limesurvey,json-rpc
 Author: Edgar RamÃ­rez-MondragÃ³n Author-email: edgarrm358@gmail.com
 Maintainer: Edgar RamÃ­rez-MondragÃ³n Maintainer-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.0,<4.0.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
```

