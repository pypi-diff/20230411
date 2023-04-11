# Comparing `tmp/nbdefense-1.0.3.tar.gz` & `tmp/nbdefense-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbdefense-1.0.3.tar", max compression
+gzip compressed data, was "nbdefense-1.0.4.tar", max compression
```

## Comparing `nbdefense-1.0.3.tar` & `nbdefense-1.0.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    10755 2023-03-31 20:29:44.913862 nbdefense-1.0.3/LICENSE
--rw-r--r--   0        0        0     3078 2023-03-31 20:29:44.913862 nbdefense-1.0.3/README.md
--rw-r--r--   0        0        0       68 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/__init__.py
--rw-r--r--   0        0        0       22 2023-03-31 20:30:08.922577 nbdefense-1.0.3/nbdefense/_version.py
--rw-r--r--   0        0        0     5566 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/cli.py
--rw-r--r--   0        0        0     9504 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/codebase.py
--rw-r--r--   0        0        0     4282 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/constants.py
--rw-r--r--   0        0        0     3452 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/dependencies.py
--rw-r--r--   0        0        0     1043 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/errors.py
--rw-r--r--   0        0        0    10085 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/issues.py
--rw-r--r--   0        0        0     8290 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/nbdefense.py
--rw-r--r--   0        0        0     9227 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/notebook.py
--rw-r--r--   0        0        0      467 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/plugins/__init__.py
--rw-r--r--   0        0        0     2916 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/plugins/cve/cve_dependency_file_plugin.py
--rw-r--r--   0        0        0     7465 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/plugins/cve/cve_notebooks_plugin.py
--rw-r--r--   0        0        0     2692 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/plugins/cve/cve_plugin.py
--rw-r--r--   0        0        0    11235 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/plugins/licenses/license_plugin.py
--rw-r--r--   0        0        0     1471 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/plugins/licenses/license_plugin_settings.py
--rw-r--r--   0        0        0     4197 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/plugins/licenses/licenses_dependency_file_plugin.py
--rw-r--r--   0        0        0     5915 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/plugins/licenses/licenses_notebooks_plugin.py
--rw-r--r--   0        0        0    16845 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/plugins/pii.py
--rw-r--r--   0        0        0     2896 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/plugins/plugin.py
--rw-r--r--   0        0        0     8682 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/plugins/secrets.py
--rw-r--r--   0        0        0     5896 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/reports.py
--rw-r--r--   0        0        0     3011 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/settings.py
--rw-r--r--   0        0        0      575 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/errors.html
--rw-r--r--   0        0        0      788 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/files-scanned-dialog.html
--rw-r--r--   0        0        0      237 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/footer.html
--rw-r--r--   0        0        0     1288 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/header.html
--rw-r--r--   0        0        0      619 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/icons/alert-icon-critical.svg
--rw-r--r--   0        0        0      619 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/icons/alert-icon-high.svg
--rw-r--r--   0        0        0      619 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/icons/alert-icon-low.svg
--rw-r--r--   0        0        0      639 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/icons/alert-icon-medium.svg
--rw-r--r--   0        0        0     1038 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/icons/header-github.svg
--rw-r--r--   0        0        0      237 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/icons/x.svg
--rw-r--r--   0        0        0      309 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/issue-codes/dependency-file.html
--rw-r--r--   0        0        0      429 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/issue-codes/license-not-found-dep-file.html
--rw-r--r--   0        0        0      805 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/issue-codes/pii-found.html
--rw-r--r--   0        0        0      718 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/issue-codes/secrets.html
--rw-r--r--   0        0        0      502 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/issue-codes/unapproved-license-dep-file.html
--rw-r--r--   0        0        0      895 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/issue-codes/vulnerable-dependency-dep-file.html
--rw-r--r--   0        0        0      319 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/issue.html
--rw-r--r--   0        0        0      711 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/issues.html
--rw-r--r--   0        0        0      368 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/navbar.html
--rw-r--r--   0        0        0      178 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/no-issues.html
--rw-r--r--   0        0        0      948 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/report.html
--rw-r--r--   0        0        0      804 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/scripts.html
--rw-r--r--   0        0        0      711 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templates/summary-card.html
--rw-r--r--   0        0        0     1260 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/templating.py
--rw-r--r--   0        0        0     2879 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/tools.py
--rw-r--r--   0        0        0     3527 2023-03-31 20:29:44.913862 nbdefense-1.0.3/nbdefense/utils.py
--rw-r--r--   0        0        0     1376 2023-03-31 20:30:09.350588 nbdefense-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4012 1970-01-01 00:00:00.000000 nbdefense-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    10755 2023-04-11 18:09:11.979092 nbdefense-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2529 2023-04-11 18:09:11.979092 nbdefense-1.0.4/README.md
+-rw-r--r--   0        0        0       68 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-11 18:09:35.803308 nbdefense-1.0.4/nbdefense/_version.py
+-rw-r--r--   0        0        0     5566 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/cli.py
+-rw-r--r--   0        0        0     9504 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/codebase.py
+-rw-r--r--   0        0        0     4282 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/constants.py
+-rw-r--r--   0        0        0     3452 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/dependencies.py
+-rw-r--r--   0        0        0     1043 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/errors.py
+-rw-r--r--   0        0        0    10085 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/issues.py
+-rw-r--r--   0        0        0     8290 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/nbdefense.py
+-rw-r--r--   0        0        0     9227 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/notebook.py
+-rw-r--r--   0        0        0      467 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/plugins/__init__.py
+-rw-r--r--   0        0        0     2916 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/plugins/cve/cve_dependency_file_plugin.py
+-rw-r--r--   0        0        0     7465 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/plugins/cve/cve_notebooks_plugin.py
+-rw-r--r--   0        0        0     2692 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/plugins/cve/cve_plugin.py
+-rw-r--r--   0        0        0    11235 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/plugins/licenses/license_plugin.py
+-rw-r--r--   0        0        0     1471 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/plugins/licenses/license_plugin_settings.py
+-rw-r--r--   0        0        0     4197 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/plugins/licenses/licenses_dependency_file_plugin.py
+-rw-r--r--   0        0        0     5915 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/plugins/licenses/licenses_notebooks_plugin.py
+-rw-r--r--   0        0        0    16845 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/plugins/pii.py
+-rw-r--r--   0        0        0     2896 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/plugins/plugin.py
+-rw-r--r--   0        0        0     8682 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/plugins/secrets.py
+-rw-r--r--   0        0        0     5896 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/reports.py
+-rw-r--r--   0        0        0     3011 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/settings.py
+-rw-r--r--   0        0        0      575 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/errors.html
+-rw-r--r--   0        0        0      788 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/files-scanned-dialog.html
+-rw-r--r--   0        0        0      237 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/footer.html
+-rw-r--r--   0        0        0     1288 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/header.html
+-rw-r--r--   0        0        0      619 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/icons/alert-icon-critical.svg
+-rw-r--r--   0        0        0      619 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/icons/alert-icon-high.svg
+-rw-r--r--   0        0        0      619 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/icons/alert-icon-low.svg
+-rw-r--r--   0        0        0      639 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/icons/alert-icon-medium.svg
+-rw-r--r--   0        0        0     1038 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/icons/header-github.svg
+-rw-r--r--   0        0        0      237 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/icons/x.svg
+-rw-r--r--   0        0        0      309 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/issue-codes/dependency-file.html
+-rw-r--r--   0        0        0      429 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/issue-codes/license-not-found-dep-file.html
+-rw-r--r--   0        0        0      812 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/issue-codes/pii-found.html
+-rw-r--r--   0        0        0      718 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/issue-codes/secrets.html
+-rw-r--r--   0        0        0      502 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/issue-codes/unapproved-license-dep-file.html
+-rw-r--r--   0        0        0      895 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/issue-codes/vulnerable-dependency-dep-file.html
+-rw-r--r--   0        0        0      319 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/issue.html
+-rw-r--r--   0        0        0      711 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/issues.html
+-rw-r--r--   0        0        0      368 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/navbar.html
+-rw-r--r--   0        0        0      178 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/no-issues.html
+-rw-r--r--   0        0        0      948 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/report.html
+-rw-r--r--   0        0        0      804 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/scripts.html
+-rw-r--r--   0        0        0      711 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templates/summary-card.html
+-rw-r--r--   0        0        0     1260 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/templating.py
+-rw-r--r--   0        0        0     2879 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/tools.py
+-rw-r--r--   0        0        0     3527 2023-04-11 18:09:12.091098 nbdefense-1.0.4/nbdefense/utils.py
+-rw-r--r--   0        0        0     1383 2023-04-11 18:09:36.307315 nbdefense-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 nbdefense-1.0.4/PKG-INFO
```

### Comparing `nbdefense-1.0.3/LICENSE` & `nbdefense-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/cli.py` & `nbdefense-1.0.4/nbdefense/cli.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/codebase.py` & `nbdefense-1.0.4/nbdefense/codebase.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/constants.py` & `nbdefense-1.0.4/nbdefense/constants.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/dependencies.py` & `nbdefense-1.0.4/nbdefense/dependencies.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/errors.py` & `nbdefense-1.0.4/nbdefense/errors.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/issues.py` & `nbdefense-1.0.4/nbdefense/issues.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/nbdefense.py` & `nbdefense-1.0.4/nbdefense/nbdefense.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/notebook.py` & `nbdefense-1.0.4/nbdefense/notebook.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/plugins/cve/cve_dependency_file_plugin.py` & `nbdefense-1.0.4/nbdefense/plugins/cve/cve_dependency_file_plugin.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/plugins/cve/cve_notebooks_plugin.py` & `nbdefense-1.0.4/nbdefense/plugins/cve/cve_notebooks_plugin.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/plugins/cve/cve_plugin.py` & `nbdefense-1.0.4/nbdefense/plugins/cve/cve_plugin.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/plugins/licenses/license_plugin.py` & `nbdefense-1.0.4/nbdefense/plugins/licenses/license_plugin.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/plugins/licenses/license_plugin_settings.py` & `nbdefense-1.0.4/nbdefense/plugins/licenses/license_plugin_settings.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/plugins/licenses/licenses_dependency_file_plugin.py` & `nbdefense-1.0.4/nbdefense/plugins/licenses/licenses_dependency_file_plugin.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/plugins/licenses/licenses_notebooks_plugin.py` & `nbdefense-1.0.4/nbdefense/plugins/licenses/licenses_notebooks_plugin.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/plugins/pii.py` & `nbdefense-1.0.4/nbdefense/plugins/pii.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/plugins/plugin.py` & `nbdefense-1.0.4/nbdefense/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/plugins/secrets.py` & `nbdefense-1.0.4/nbdefense/plugins/secrets.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/reports.py` & `nbdefense-1.0.4/nbdefense/reports.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/settings.py` & `nbdefense-1.0.4/nbdefense/settings.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templates/errors.html` & `nbdefense-1.0.4/nbdefense/templates/errors.html`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templates/files-scanned-dialog.html` & `nbdefense-1.0.4/nbdefense/templates/files-scanned-dialog.html`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templates/header.html` & `nbdefense-1.0.4/nbdefense/templates/header.html`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templates/icons/alert-icon-critical.svg` & `nbdefense-1.0.4/nbdefense/templates/icons/alert-icon-critical.svg`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templates/icons/alert-icon-high.svg` & `nbdefense-1.0.4/nbdefense/templates/icons/alert-icon-high.svg`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templates/icons/alert-icon-low.svg` & `nbdefense-1.0.4/nbdefense/templates/icons/alert-icon-low.svg`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templates/icons/alert-icon-medium.svg` & `nbdefense-1.0.4/nbdefense/templates/icons/alert-icon-medium.svg`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templates/icons/header-github.svg` & `nbdefense-1.0.4/nbdefense/templates/icons/header-github.svg`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templates/issue-codes/pii-found.html` & `nbdefense-1.0.4/nbdefense/templates/issue-codes/vulnerable-dependency-dep-file.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 <div class="w-full">
-  <h3 class="font-bold">{{ issue_code | replace("_", " ") | title | replace("Pii", "PII") }}</h3>
-  <p class="mt-4">Path: {{ issue.details.file_path }}</p>
-  <p class="mt-4"><b>Description</b>:</p>
-  <p>{{ issue.details.description }} with the following tag(s):</p>
+  {% set issue_details = issue.details %}
+  <h3 class="font-bold">CVE</h3>
+  <p class="mt-4">Path: {{ issue_details.file_path }}</p>
   <p>
-  <pre>{{ issue.details.summary_field | to_pretty_json | safe }}</pre>
-  </p>
-  <p class="mt-4">
-    <b>Location</b>: cell {{ issue.location.value }}
-  </p>
-  <div class="flex flex-row w-100 mt-4">
-    <div class="pr-4">
-      <p class="font-bold">Cell #{{ issue.cell.cell_index }}</p>
-    </div>   
-    <div
-      class="bg-white border-solid border border-none-border rounded-md overflow-x-auto w-[42rem]"
+    Vulnerability:
+    <a
+      class="underline text-blue-600 hover:text-blue-800"
+      href="{{ issue_details.vulnerability['PrimaryURL'] }}"
+      target="_blank"
+      rel="noreferrer"
+      >{{ issue_details.vulnerability['VulnerabilityID'] }}</a
     >
-      <span class="pl-4">{{ issue.cell | string() | safe }}</span>
-    </div>     
+  </p>
+  <div class="grid grid-cols-3 background-black w-full mt-4">
+    <div>
+      <h3 class="font-bold">Package</h3>
+      <p>{{ issue_details.vulnerability['PkgName'] }}</p>
+    </div>
+    <div>
+      <h3 class="font-bold">Affected versions</h3>
+      <p>{{ issue_details.vulnerability['InstalledVersion'] }}</p>
+    </div>
+    <div>
+      <h3 class="font-bold">Fixed versions</h3>
+      <p>{{ issue_details.vulnerability['FixedVersion'] }}</p>
+    </div>
   </div>
-</div>
+</div>
```

### Comparing `nbdefense-1.0.3/nbdefense/templates/issue-codes/secrets.html` & `nbdefense-1.0.4/nbdefense/templates/issue-codes/secrets.html`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templates/issues.html` & `nbdefense-1.0.4/nbdefense/templates/issues.html`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templates/report.html` & `nbdefense-1.0.4/nbdefense/templates/report.html`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templates/scripts.html` & `nbdefense-1.0.4/nbdefense/templates/scripts.html`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templates/summary-card.html` & `nbdefense-1.0.4/nbdefense/templates/summary-card.html`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/templating.py` & `nbdefense-1.0.4/nbdefense/templating.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/tools.py` & `nbdefense-1.0.4/nbdefense/tools.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/nbdefense/utils.py` & `nbdefense-1.0.4/nbdefense/utils.py`

 * *Files identical despite different names*

### Comparing `nbdefense-1.0.3/pyproject.toml` & `nbdefense-1.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "nbdefense"
-description = "NB Defense CLI."
-version = "1.0.3"
+description = "NB Defense CLI and SDK"
+version = "1.0.4"
 authors = ["ProtectAI <community@protectai.com>"]
 readme = "README.md"
 packages = [{ include = "nbdefense" }]
 license = "Apache License 2.0"
 exclude = ["tests/*", "Makefile"]
 
 [tool.poetry.scripts]
```

