# Comparing `tmp/odoo-fast-report-mapper-equitania-0.1.5.tar.gz` & `tmp/odoo-fast-report-mapper-equitania-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo-fast-report-mapper-equitania-0.1.5.tar", last modified: Fri Feb 11 07:07:25 2022, max compression
+gzip compressed data, was "odoo-fast-report-mapper-equitania-0.1.8.tar", last modified: Fri Feb 18 10:32:30 2022, max compression
```

## Comparing `odoo-fast-report-mapper-equitania-0.1.5.tar` & `odoo-fast-report-mapper-equitania-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2022-02-11 07:07:25.135784 odoo-fast-report-mapper-equitania-0.1.5/
--rw-r--r--   0 picard     (501) staff       (20)    33892 2021-01-21 10:02:56.000000 odoo-fast-report-mapper-equitania-0.1.5/LICENSE.txt
--rw-r--r--   0 picard     (501) staff       (20)     2383 2022-02-11 07:07:25.135645 odoo-fast-report-mapper-equitania-0.1.5/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)     1824 2021-11-25 09:18:48.000000 odoo-fast-report-mapper-equitania-0.1.5/README.md
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2022-02-11 07:07:25.133696 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper/
--rw-r--r--   0 picard     (501) staff       (20)      218 2021-10-14 07:57:03.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper/MyDumper.py
--rw-r--r--   0 picard     (501) staff       (20)      127 2021-10-14 07:57:03.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper/__init__.py
--rw-r--r--   0 picard     (501) staff       (20)    14877 2022-02-11 07:05:21.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper/eq_odoo_connection.py
--rw-r--r--   0 picard     (501) staff       (20)     3725 2022-02-11 07:05:21.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper/eq_report.py
--rw-r--r--   0 picard     (501) staff       (20)     3772 2021-10-14 07:57:03.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper/eq_utils.py
--rw-r--r--   0 picard     (501) staff       (20)     2210 2021-11-25 12:48:50.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper/odoo_fast_report_mapper.py
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2022-02-11 07:07:25.134501 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper_equitania.egg-info/
--rw-r--r--   0 picard     (501) staff       (20)     2383 2022-02-11 07:07:25.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper_equitania.egg-info/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)      775 2022-02-11 07:07:25.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper_equitania.egg-info/SOURCES.txt
--rw-r--r--   0 picard     (501) staff       (20)        1 2022-02-11 07:07:25.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper_equitania.egg-info/dependency_links.txt
--rw-r--r--   0 picard     (501) staff       (20)      124 2022-02-11 07:07:25.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper_equitania.egg-info/entry_points.txt
--rw-r--r--   0 picard     (501) staff       (20)       41 2022-02-11 07:07:25.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper_equitania.egg-info/requires.txt
--rw-r--r--   0 picard     (501) staff       (20)       43 2022-02-11 07:07:25.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper_equitania.egg-info/top_level.txt
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2022-02-11 07:07:25.135326 odoo-fast-report-mapper-equitania-0.1.5/odoo_report_helper/
--rw-r--r--   0 picard     (501) staff       (20)       96 2021-01-21 10:02:56.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_report_helper/__init__.py
--rw-r--r--   0 picard     (501) staff       (20)      254 2021-01-21 10:02:56.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_report_helper/exceptions.py
--rw-r--r--   0 picard     (501) staff       (20)     9153 2021-10-14 07:57:03.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_report_helper/odoo_connection.py
--rw-r--r--   0 picard     (501) staff       (20)     2816 2021-10-14 07:57:03.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_report_helper/report.py
--rw-r--r--   0 picard     (501) staff       (20)     2226 2021-01-21 10:02:56.000000 odoo-fast-report-mapper-equitania-0.1.5/odoo_report_helper/utils.py
--rw-r--r--   0 picard     (501) staff       (20)       38 2022-02-11 07:07:25.135828 odoo-fast-report-mapper-equitania-0.1.5/setup.cfg
--rw-r--r--   0 picard     (501) staff       (20)     1008 2022-02-11 07:05:21.000000 odoo-fast-report-mapper-equitania-0.1.5/setup.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2022-02-18 10:32:30.414129 odoo-fast-report-mapper-equitania-0.1.8/
+-rw-r--r--   0 picard     (501) staff       (20)    33892 2021-01-21 10:02:56.000000 odoo-fast-report-mapper-equitania-0.1.8/LICENSE.txt
+-rw-r--r--   0 picard     (501) staff       (20)     2383 2022-02-18 10:32:30.414008 odoo-fast-report-mapper-equitania-0.1.8/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)     1824 2021-11-25 09:18:48.000000 odoo-fast-report-mapper-equitania-0.1.8/README.md
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2022-02-18 10:32:30.412357 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper/
+-rw-r--r--   0 picard     (501) staff       (20)      218 2021-10-14 07:57:03.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper/MyDumper.py
+-rw-r--r--   0 picard     (501) staff       (20)      127 2021-10-14 07:57:03.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper/__init__.py
+-rw-r--r--   0 picard     (501) staff       (20)    20667 2022-02-18 10:31:34.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper/eq_odoo_connection.py
+-rw-r--r--   0 picard     (501) staff       (20)     3326 2022-02-18 10:31:34.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper/eq_report.py
+-rw-r--r--   0 picard     (501) staff       (20)     4304 2022-02-18 10:31:34.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper/eq_utils.py
+-rw-r--r--   0 picard     (501) staff       (20)     2298 2022-02-18 10:31:34.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper/odoo_fast_report_mapper.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2022-02-18 10:32:30.412981 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper_equitania.egg-info/
+-rw-r--r--   0 picard     (501) staff       (20)     2383 2022-02-18 10:32:30.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper_equitania.egg-info/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)      775 2022-02-18 10:32:30.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper_equitania.egg-info/SOURCES.txt
+-rw-r--r--   0 picard     (501) staff       (20)        1 2022-02-18 10:32:30.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper_equitania.egg-info/dependency_links.txt
+-rw-r--r--   0 picard     (501) staff       (20)      124 2022-02-18 10:32:30.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper_equitania.egg-info/entry_points.txt
+-rw-r--r--   0 picard     (501) staff       (20)       41 2022-02-18 10:32:30.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper_equitania.egg-info/requires.txt
+-rw-r--r--   0 picard     (501) staff       (20)       43 2022-02-18 10:32:30.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper_equitania.egg-info/top_level.txt
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2022-02-18 10:32:30.413802 odoo-fast-report-mapper-equitania-0.1.8/odoo_report_helper/
+-rw-r--r--   0 picard     (501) staff       (20)       96 2021-01-21 10:02:56.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_report_helper/__init__.py
+-rw-r--r--   0 picard     (501) staff       (20)      254 2021-01-21 10:02:56.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_report_helper/exceptions.py
+-rw-r--r--   0 picard     (501) staff       (20)     9153 2021-10-14 07:57:03.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_report_helper/odoo_connection.py
+-rw-r--r--   0 picard     (501) staff       (20)     2816 2021-10-14 07:57:03.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_report_helper/report.py
+-rw-r--r--   0 picard     (501) staff       (20)     2226 2021-01-21 10:02:56.000000 odoo-fast-report-mapper-equitania-0.1.8/odoo_report_helper/utils.py
+-rw-r--r--   0 picard     (501) staff       (20)       38 2022-02-18 10:32:30.414166 odoo-fast-report-mapper-equitania-0.1.8/setup.cfg
+-rw-r--r--   0 picard     (501) staff       (20)     1008 2022-02-18 10:31:34.000000 odoo-fast-report-mapper-equitania-0.1.8/setup.py
```

### Comparing `odoo-fast-report-mapper-equitania-0.1.5/LICENSE.txt` & `odoo-fast-report-mapper-equitania-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `odoo-fast-report-mapper-equitania-0.1.5/PKG-INFO` & `odoo-fast-report-mapper-equitania-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-fast-report-mapper-equitania
-Version: 0.1.5
+Version: 0.1.8
 Summary: A package to create FastReport entries in Odoo
 Home-page: https://github.com/equitania/odoo-fast-report-mapper
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `odoo-fast-report-mapper-equitania-0.1.5/README.md` & `odoo-fast-report-mapper-equitania-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper/eq_odoo_connection.py` & `odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper/eq_odoo_connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,20 +16,39 @@
 
 class EqOdooConnection(OdooConnection):
     def __init__(self, clean_old_reports, language, *args, **kwargs):
         super(EqOdooConnection, self).__init__(*args, **kwargs)
         self.do_clean_reports = clean_old_reports
         self.language = language
 
-    def _search_report(self, model_name, report_name: dict):
+    def _search_report_v13(self, model_name, report_name: dict, IR_ACTIONS_REPORT=False, company_id=False):
         """
             If parameter "do_clean_reports" (delete_old_reports in connection yaml) is set, delete all report with
             report_type = fast_report
         """
-        IR_ACTIONS_REPORT = self.connection.env['ir.actions.report']
+        if not IR_ACTIONS_REPORT:
+            IR_ACTIONS_REPORT = self.connection.env['ir.actions.report']
+        report_ids = IR_ACTIONS_REPORT.search(
+            [('model', '=ilike', model_name), '|', ('name', '=ilike', report_name['ger']),
+             ('name', '=ilike', report_name['ger'] + " " + "(PDF)"),'|', ('company_id', '=', company_id), ('company_id', '=', False)])
+        if len(report_ids) == 0 and 'eng' in report_name:
+            report_ids = IR_ACTIONS_REPORT.search([('model', '=', model_name), '|', ('name', '=', report_name['eng']),
+                                                   ('name', '=', report_name['eng'] + " " + "(PDF)"), '|', ('company_id', '=', company_id), ('company_id', '=', False)])
+        if len(report_ids) == 0:
+            return False
+        else:
+            return report_ids[0]
+
+    def _search_report(self, model_name, report_name: dict, IR_ACTIONS_REPORT=False):
+        """
+            If parameter "do_clean_reports" (delete_old_reports in connection yaml) is set, delete all report with
+            report_type = fast_report
+        """
+        if not IR_ACTIONS_REPORT:
+            IR_ACTIONS_REPORT = self.connection.env['ir.actions.report']
         report_ids = IR_ACTIONS_REPORT.search(
             [('model', '=ilike', model_name), '|', ('name', '=ilike', report_name['ger']),
              ('name', '=ilike', report_name['ger'] + " " + "(PDF)")])
         if len(report_ids) == 0 and 'eng' in report_name:
             report_ids = IR_ACTIONS_REPORT.search([('model', '=', model_name), '|', ('name', '=', report_name['eng']),
                                                    ('name', '=', report_name['eng'] + " " + "(PDF)")])
         if len(report_ids) == 0:
@@ -38,44 +57,75 @@
             return report_ids[0]
 
     def clean_reports(self):
         """
             If parameter "do_clean_reports" (delete_old_reports in connection yaml) is set, delete all report with
             report_type = fast_report
         """
-        if self.do_clean_reports:
-            report_ids = self._get_fast_report_ids()
-            for report_id in report_ids:
-                self._delete_report(report_id)
+        original_company_yaml_user = self.connection.env.user.company_id.id
+        company_ids = self.connection.env.user.company_ids.ids if self.connection.env.user.company_ids else self.connection.env.user.company_id.ids
+        for company_id in company_ids:
+            self.connection.env.user.company_id = company_id
+            if self.do_clean_reports:
+                report_ids = self._get_fast_report_ids()
+                for report_id in report_ids:
+                    self._delete_report(report_id)
+        self.connection.env.user.company_id = original_company_yaml_user
+
+    def check_dependencies(self, dependencies):
+        """
+            Check if all dependencies (modules) are installed, if one isn't, return False
+            :param: dependencies: List of names of modules
+        """
+        not_installed_modules = []
+        if dependencies:
+            for dependency in dependencies:
+                dependency_installed = self.check_module(dependency)
+                if not dependency_installed:
+                    not_installed_modules.append(dependency)
+            if not_installed_modules:
+                return False, not_installed_modules
+        return True, not_installed_modules
 
     def map_reports(self, report_list: list):
         """
             Create/Write reports into the Odoo system with their fields and properties
             :param: report_list: List of report objects
         """
         IR_MODEL = self.connection.env['ir.model']
         IR_MODEL_FIELDS = self.connection.env['ir.model.fields']
         IR_ACTIONS_REPORT = self.connection.env['ir.actions.report']
+        original_company_yaml_user = IR_ACTIONS_REPORT.env.user.company_id
         for report in report_list:
             report.self_ensure()
             report._data_dictionary['name'] = report.entry_name[self.language]
-            dependencies_installed = self.check_dependencies(report._dependencies)
-            if not dependencies_installed:
+            dependencies_installed, not_installed_modules = self.check_dependencies(report._dependencies)
+            if not dependencies_installed and not_installed_modules:
                 print(f"!!! ******** DEPENDENCIES FOR {report.report_name} NOT INSTALLED ******** !!!")
+                for not_installed_module in not_installed_modules:
+                    print(f"!!! ******** MODULE - {not_installed_module} - NOT INSTALLED ******** !!!")
                 continue
-            report_id = self._search_report(report.model_name, report.entry_name)
+            if report.company_id:
+                IR_ACTIONS_REPORT.env.user.company_id = report.company_id[0]
+                if self.version == '13':
+                    report_id = self._search_report_v13(report.model_name, report.entry_name, IR_ACTIONS_REPORT, report.company_id[0])
+                else:
+                    report_id = self._search_report(report.model_name, report.entry_name, IR_ACTIONS_REPORT)
+            else:
+                report_id = self._search_report(report.model_name, report.entry_name, IR_ACTIONS_REPORT)
             if not report_id:
                 report_id = IR_ACTIONS_REPORT.create(report._data_dictionary)
                 report_object = IR_ACTIONS_REPORT.browse(report_id)
             else:
                 report_object = IR_ACTIONS_REPORT.browse(report_id)
                 report_object.write(report._data_dictionary)
             # Add report to print menu
             report_object.create_action()
             print(f"!!! ******** START {report.report_name} ******** !!!")
+            IR_ACTIONS_REPORT.env.user.company_id = original_company_yaml_user
             try:
                 # Loop over all models in report fields dictionary
                 for model_name in report._fields:
                     # Get model object in Odoo
                     model_id = IR_MODEL.search([('model', '=', model_name)])
                     model_object = IR_MODEL.browse(model_id)
                     # Loop over all fields in the list of the current model
@@ -83,64 +133,88 @@
                         # Get the field from in Odoo
                         field_id = IR_MODEL_FIELDS.search(
                             [('model_id', '=', model_object.id), ('name', '=', field_name)])
                         if field_id:
                             field = IR_MODEL_FIELDS.browse(field_id)
                             # Insert the report_id
                             if report_object.id not in field.eq_report_ids.ids:
-                                report_ids = field.eq_report_ids.ids
-                                report_ids.append(report_object.id)
+                                report_ids = field.eq_report_ids.ids + [report_object.id]
                                 field.write({'eq_report_ids': [(6, 0, report_ids)]})
+                                # field.update({'eq_report_ids': [(6, 0, report_ids)]})
+                                # field.update({'eq_report_ids': [(4, report_object.id)]})
                 if report._calculated_fields:
                     for field, content in report._calculated_fields.items():
                         for function_name, parameter in content.items():
                             self.set_calculated_fields(field, function_name, parameter, report.entry_name,
                                                        report.model_name)
                 print(f"!!! ******** END {report.report_name} ******** !!!")
             except Exception as ex:
                 print("!!! ******** EXCEPTION ******** !!!")
                 print(ex)
 
     def collect_all_report_entries(self, output_path):
-        IR_MODEL_FIELDS = self.connection.env['ir.model.fields']
-        all_report_field_ids = IR_MODEL_FIELDS.search([('eq_report_ids', '!=', False)])
+        company_ids = self.connection.env.user.company_ids.ids if self.connection.env.user.company_ids else self.connection.env.user.company_id.ids
+        report_name_id_combination = dict()
         data_dictionary = {}
-        print('Collect fields...')
-        # Progressbar...
-        with click.progressbar(range(len(all_report_field_ids))) as bar:
-            for field_id in all_report_field_ids:
-                # Get object
-                field_object = IR_MODEL_FIELDS.browse(field_id)
-                # Get attributes
-                report_action_ids = field_object.eq_report_ids.ids
-                model_id = field_object.model_id
-                model_name = model_id.model
-                field_name = field_object.name
-                # Add field to dictionary
-                for report_action_id in report_action_ids:
-                    data_dictionary = self.add_field_to_dictionary(data_dictionary, report_action_id, model_name,
-                                                                   field_name)
+        for company_id in company_ids:
+            self.connection.env.user.company_id = company_id
+            IR_MODEL_FIELDS = self.connection.env['ir.model.fields']
+            all_report_field_ids = IR_MODEL_FIELDS.search([('eq_report_ids', '!=', False)])
+            print('Collect fields...')
+            # Progressbar...
+            with click.progressbar(range(len(all_report_field_ids))) as bar:
+                for field_id in all_report_field_ids:
+                    # Get object
+                    field_object = IR_MODEL_FIELDS.browse(field_id)
+                    # Get attributes
+                    report_action_ids = field_object.eq_report_ids.ids
+                    model_id = field_object.model_id
+                    model_name = model_id.model
+                    field_name = field_object.name
+                    if self.version == "10":
+                        IR_ACTIONS_REPORT = self.connection.env['ir.actions.report.xml']
+                    else:
+                        IR_ACTIONS_REPORT = self.connection.env['ir.actions.report']
+                    # Add field to dictionary
+                    for report_action_id in report_action_ids:
+                        report_action_object = IR_ACTIONS_REPORT.browse(report_action_id)
+                        company_id = report_action_object.company_id.id if report_action_object.company_id else False
+                        if company_id:
+                            if report_action_object.report_name in report_name_id_combination and report_action_id != report_name_id_combination[report_action_object.report_name]:
+                                if 'company_id' in data_dictionary[report_name_id_combination[report_action_object.report_name]] and company_id not in data_dictionary[report_name_id_combination[report_action_object.report_name]]['company_id']:
+                                    data_dictionary[report_name_id_combination[report_action_object.report_name]]['company_id'].append(company_id)
+                                continue
+                            else:
+                                report_name_id_combination[report_action_object.report_name] = report_action_id
+                        data_dictionary = self.add_field_to_dictionary(data_dictionary, report_action_id, model_name,
+                                                                    field_name, company_id)
         for report_action_id, fields in data_dictionary.items():
             # Create report object
             eq_report_object = self.create_eq_report_object(report_action_id, fields)
             eq_yaml_data = eq_report_object.ensure_data_for_yaml()
+
             # Get timestamp
             now = datetime.now()
             date_now = now.strftime("%m_%d_%Y_%H_%M_%S")
             # Set output name
             output_name = output_path + '/' + eq_report_object.report_name + '_' + date_now + '.yaml'
             self.write_yaml(output_name, eq_yaml_data)
 
-    def add_field_to_dictionary(self, data_dictionary, report_id, model_name, field_name):
+    def add_field_to_dictionary(self, data_dictionary, report_id, model_name, field_name, company_id):
         if report_id not in data_dictionary:
             data_dictionary[report_id] = {}
         if model_name not in data_dictionary[report_id]:
             data_dictionary[report_id][model_name] = [field_name]
-        else:
+        if field_name not in data_dictionary[report_id][model_name]:
             data_dictionary[report_id][model_name].append(field_name)
+        if company_id:
+            if 'company_id' in data_dictionary[report_id] and company_id not in data_dictionary[report_id]['company_id']:
+                data_dictionary[report_id]['company_id'].append(company_id)
+            else:
+                data_dictionary[report_id]['company_id'] = [company_id]
         return data_dictionary
 
     def _collect_calculated_fields(self, eq_calculated_field_objects):
         """
             Get calculated fields from eq_calculated_field model objects:
             Example:
             {
@@ -159,51 +233,48 @@
         return eq_calculated_field_dict
 
     def create_eq_report_object(self, action_id, field_dictionary):
         if self.version == "10":
             IR_ACTIONS_REPORT = self.connection.env['ir.actions.report.xml']
         else:
             IR_ACTIONS_REPORT = self.connection.env['ir.actions.report']
+        if 'company_id' in field_dictionary:
+            self.connection.env.user.company_id = field_dictionary['company_id'][0]
         action_object = IR_ACTIONS_REPORT.browse(action_id)
         # Collect attributes
         name = {self.language: action_object.name}
         report_name = action_object.report_name
         report_type = action_object.report_type
         eq_export_type = action_object.eq_export_type
         print_report_name = action_object.print_report_name
         model_name = action_object.model
         eq_ignore_images = action_object.eq_ignore_images
-        eq_ignore_html = action_object.eq_ignore_html
-        eq_export_complete_html = action_object.eq_export_complete_html
-        multi_print = action_object.multi
+        eq_handling_html_fields = action_object.eq_handling_html_fields
+        multi = action_object.multi
         attachment_use = action_object.attachment_use
         attachment = action_object.attachment
         eq_calculated_field_ids = action_object.eq_calculated_field_ids
-        company_id = action_object.company_id
+        company_id = field_dictionary['company_id'] if 'company_id' in field_dictionary else False
+        if 'company_id' in field_dictionary:
+            del field_dictionary['company_id']
 
-        # Special cases => not in every version
-        eq_export_as_sql = action_object.eq_export_as_sql
-        if not self.is_boolean(eq_export_as_sql):
-            eq_export_as_sql = True
         calculated_fields_dict = self._collect_calculated_fields(eq_calculated_field_ids)
         if not self.is_dict(calculated_fields_dict):
             calculated_fields_dict = {}
         eq_print_button = action_object.eq_print_button
         if not self.is_boolean(eq_print_button):
             eq_print_button = False
-        eq_merge_data_from_multi = action_object.eq_merge_data_from_multi
-        if not self.is_boolean(eq_merge_data_from_multi):
-            eq_merge_data_from_multi = False
+        eq_multiprint = action_object.eq_multiprint
 
         eq_report_obj = eq_report.EqReport(name, report_name, report_type, model_name, company_id, eq_export_type,
                                            print_report_name, attachment,
-                                           eq_ignore_images, eq_ignore_html, eq_export_complete_html, eq_export_as_sql,
-                                           multi_print,
+                                           eq_ignore_images, eq_handling_html_fields,
+                                           multi,
                                            attachment_use, eq_print_button, [], field_dictionary,
-                                           calculated_fields_dict, eq_merge_data_from_multi)
+                                           calculated_fields_dict, eq_multiprint)
         return eq_report_obj
 
     def write_yaml(self, file_name, data):
         with io.open(file_name, 'w', encoding='utf8') as outfile:
             yaml.dump(data, outfile, Dumper=MyDumper.MyDumper, default_flow_style=False, allow_unicode=True,
                       sort_keys=False)
 
@@ -225,20 +296,29 @@
         """
 
         ### Uncomment/comment to display logging to extern log file or to console ###
         ## Log file
         #logging.basicConfig(format='%(asctime)s - %(message)s ',  datefmt='%H:%M:%S %d.%m.%Y', level=logging.INFO, filename=f"testing_fast_report_rendering_{self.connection._env._db}.log")
         ## Console
         logging.basicConfig(format='%(asctime)s - %(message)s ',  datefmt='%H:%M:%S %d.%m.%Y', level=logging.INFO)
-
-        IR_ACTIONS_REPORT = self.connection.env['ir.actions.report']
-        IR_MODEL = self.connection.env['ir.model']
+        original_company_yaml_user = self.connection.env.user.company_id
         for report in report_list:
+            if report.company_id:
+                self.connection.env.user.company_id = report.company_id[0]
+                IR_ACTIONS_REPORT = self.connection.env['ir.actions.report']
+                IR_MODEL = self.connection.env['ir.model']
+                if self.version == '13':
+                    report_id = self._search_report_v13(report.model_name, report.entry_name, IR_ACTIONS_REPORT, report.company_id[0])
+                else:
+                    report_id = self._search_report(report.model_name, report.entry_name, IR_ACTIONS_REPORT)
+            else:
+                IR_ACTIONS_REPORT = self.connection.env['ir.actions.report']
+                IR_MODEL = self.connection.env['ir.model']
+                report_id = self._search_report(report.model_name, report.entry_name, IR_ACTIONS_REPORT)
             # Get report action record
-            report_id = self._search_report(report.model_name, report.entry_name)
             report_object = IR_ACTIONS_REPORT.browse(report_id) if report_id else False
             # Check if the report has been created and is type Fast Report
             if not report_id or report_object.report_type != "fast_report": 
                 logging.info(f"!!! ******** REPORT {report.report_name} NOT CREATED OR IS NOT TYPE FAST REPORT ******** !!!")
                 continue
 
             logging.info(f"!!! ******** TESTING REPORT RENDERING {report.report_name} ******** !!!")
@@ -273,7 +353,8 @@
                 except Exception as ex:
                     if "No such file or directory" in str(ex):
                         logging.info(f"\033[0;33m!!! ******** NO DEMO DATA TO TEST REPORT {report.report_name} ******** !!!\033[0;37m ")
                     else:
                         logging.info(f"\033[0;31m!!! ******** REPORT \033[1;31m{report.report_name}\033[0;31m NOT RENDERING CORRECTLY ******** !!!\033[0;37m ")
                         logging.info(f"\033[0;31m!!! ******** EXCEPTION ******** !!!\033[0;37m")
                         logging.info("\033[0;31m" + str(ex) + "\033[0;37m")
+        self.connection.env.user.company_id = original_company_yaml_user
```

### Comparing `odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper/eq_report.py` & `odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper/eq_report.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,32 +3,29 @@
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 from odoo_report_helper.report import Report
 
 
 class EqReport(Report):
     def __init__(self, entry_name, report_name: str, report_type: str, model_name: str, company_id, eq_export_type="pdf",
-                 print_report_name="Report", attachment="Report.pdf", eq_ignore_images=True, eq_ignore_html=False,
-                 eq_export_complete_html=False, eq_export_as_sql=True, multi_print=False, attachment_use=False,
+                 print_report_name="Report", attachment="Report.pdf", eq_ignore_images=True, eq_handling_html_fields='standard', multi=False, attachment_use=False,
                  eq_print_button=False, dependencies=[], model_fields={}, calculated_fields={},
-                 eq_merge_data_from_multi=False):
+                 eq_multiprint='standard'):
         self.entry_name = entry_name
         self.report_name = report_name
         self.report_type = report_type
         self.model_name = model_name
         self.print_report_name = print_report_name
         self.eq_export_type = eq_export_type
         self.attachment = attachment
         self.eq_ignore_images = eq_ignore_images
-        self.eq_ignore_html = eq_ignore_html
-        self.eq_export_complete_html = eq_export_complete_html
-        self.eq_export_as_sql = eq_export_as_sql
-        self.multi_print = multi_print
+        self.eq_handling_html_fields = eq_handling_html_fields
+        self.multi = multi
         self.attachment_use = attachment_use
-        self.eq_merge_data_from_multi = eq_merge_data_from_multi
+        self.eq_multiprint = eq_multiprint
         self.eq_print_button = eq_print_button
         self._fields = model_fields
         self._calculated_fields = calculated_fields
         self._dependencies = dependencies
         self._data_dictionary = {}
         self.company_id = company_id
 
@@ -38,43 +35,40 @@
         """
         self._data_dictionary = {
             'name': self.entry_name['ger'],
             'report_name': self.report_name,
             'report_type': self.report_type,
             'print_report_name': self.print_report_name,
             'model': self.model_name,
+            'company_id': self.company_id[0] if self.company_id else False,
             'eq_export_type': self.eq_export_type,
             'eq_ignore_images': self.eq_ignore_images,
-            'eq_ignore_html': self.eq_ignore_html,
-            'eq_export_complete_html': self.eq_export_complete_html,
-            'eq_export_as_sql': self.eq_export_as_sql,
-            'eq_merge_data_from_multi': self.eq_merge_data_from_multi,
-            'multi': self.multi_print,
+            'eq_handling_html_fields': self.eq_handling_html_fields,
+            'eq_multiprint': self.eq_multiprint,
+            'multi': self.multi,
             'attachment': self.attachment,
             'attachment_use': self.attachment_use,
             'eq_print_button': self.eq_print_button
         }
 
     def ensure_data_for_yaml(self):
         yaml_data = {
             'name': self.entry_name,
             'report_name': self.report_name,
             'report_type': self.report_type,
             'print_report_name': self.print_report_name,
             'report_model': self.model_name,
             'eq_export_type': self.eq_export_type,
             'eq_ignore_images': self.eq_ignore_images,
-            'eq_ignore_html': self.eq_ignore_html,
-            'eq_export_complete_html': self.eq_export_complete_html,
-            'eq_export_as_sql': self.eq_export_as_sql,
-            'eq_merge_data_from_multi': self.eq_merge_data_from_multi,
-            'multiprint': self.multi_print,
+            'eq_handling_html_fields': self.eq_handling_html_fields,
+            'eq_multiprint': self.eq_multiprint,
+            'multi': self.multi,
             'attachment': self.attachment,
             'attachment_use': self.attachment_use,
             'eq_print_button': self.eq_print_button,
             'dependencies': [],
             'report_fields': self._fields,
             'calculated_fields': self._calculated_fields
         }
         if self.company_id:
-            yaml_data = {k: v for k, v in (list(yaml_data.items())[:5] + [('company_id', [self.company_id.id])] + list(yaml_data.items())[5:])}
+            yaml_data = {k: v for k, v in (list(yaml_data.items())[:5] + [('company_id', self.company_id)] + list(yaml_data.items())[5:])}
         return yaml_data
```

### Comparing `odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper/eq_utils.py` & `odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper/eq_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,46 +2,42 @@
 # Copyright 2014-now Equitania Software GmbH - Pforzheim - Germany
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 from . import eq_report
 from . import eq_odoo_connection
 import odoo_report_helper.utils as utils
 import odoo_report_helper.exceptions as exceptions
+import copy
 
 
 def create_report_object_from_yaml_object(yaml_object):
     """
         Create EqReport object from yaml_object
         :param: yaml_object
         :return: EqReport object
     """
     # Set this in a try block because not all yaml files are up2date
-    try:
-        eq_merge_data_from_multi = yaml_object['eq_merge_data_from_multi']
-    except KeyError:
-        eq_merge_data_from_multi = False
     report = eq_report.EqReport(
         yaml_object['name'],
         yaml_object['report_name'],
         yaml_object['report_type'],
         yaml_object['report_model'],
+        yaml_object.get('company_id', False),
         yaml_object['eq_export_type'],
         yaml_object['print_report_name'],
         yaml_object['attachment'],
         yaml_object['eq_ignore_images'],
-        yaml_object['eq_ignore_html'],
-        yaml_object['eq_export_complete_html'],
-        yaml_object['eq_export_as_sql'],
-        yaml_object['multiprint'],
+        yaml_object['eq_handling_html_fields'],
+        yaml_object['multi'],
         yaml_object['attachment_use'],
         yaml_object['eq_print_button'],
         yaml_object['dependencies'],
         yaml_object['report_fields'],
         yaml_object['calculated_fields'],
-        eq_merge_data_from_multi
+        yaml_object['eq_multiprint'],
     )
     return report
 
 
 def create_odoo_connection_from_yaml_object(yaml_object):
     """
         Create EqOdooConnection object from yaml_object
@@ -78,15 +74,26 @@
     """
         Get all yaml objects from path and convert them into report objects
         :param: path to yaml files
         :return: list of report objects
     """
     try:
         yaml_report_objects = utils.parse_yaml_folder(path)
-        eq_report_objects = convert_all_yaml_objects(yaml_report_objects, create_report_object_from_yaml_object)
+        filtered_yaml_report_objects = []
+        for yaml_report_object in yaml_report_objects:
+            if yaml_report_object.get('company_id') and len(yaml_report_object.get('company_id')) > 1:
+                company_ids = yaml_report_object.get('company_id')
+                del yaml_report_object['company_id']
+                for company_id in company_ids:
+                    temp_yaml_report_object = copy.deepcopy(yaml_report_object)
+                    temp_yaml_report_object['company_id'] = [company_id]
+                    filtered_yaml_report_objects.append(temp_yaml_report_object)
+            else:
+                filtered_yaml_report_objects.append(yaml_report_object)
+        eq_report_objects = convert_all_yaml_objects(filtered_yaml_report_objects, create_report_object_from_yaml_object)
         return eq_report_objects
     except FileNotFoundError as ex:
         raise exceptions.PathDoesNotExitError("ERROR: Please check your Path" + " " + str(ex))
         sys.exit(0)
 
 
 def collect_all_connections(path):
```

### Comparing `odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper/odoo_fast_report_mapper.py` & `odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper/odoo_fast_report_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 
 @click.command()
 @click.option('--server_path', help='Server configuration folder',
               prompt='Please enter the path to your configuration folder')
 @click.option('--report_path', help='Reports folder',
               prompt='Please enter the path to your report folder')
-@click.option('--collect_reports', help='Report collection - this will disable mapping of reports (y/n)')
+@click.option('--collect_reports', help='Report collection - this will disable mapping of reports (y/n)', 
+              prompt='Report collection - this will disable mapping of reports (y/n)')
 @click.option('--disable_qweb', help='Disable QWeb Reports (y/n)',
               prompt='Disable QWeb reports? (y/n)')
 @click.option('--testing_only', help='Testing only (y) or Mapping & Testing (n). Default:n',
               prompt='Testing FastReport only? (y/n)')
 def start_odoo_fast_report_mapper(server_path, report_path, collect_reports, disable_qweb, testing_only):
     # Collect yaml files and build objects
     connections = eq_utils.collect_all_connections(server_path)
```

### Comparing `odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper_equitania.egg-info/PKG-INFO` & `odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper_equitania.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-fast-report-mapper-equitania
-Version: 0.1.5
+Version: 0.1.8
 Summary: A package to create FastReport entries in Odoo
 Home-page: https://github.com/equitania/odoo-fast-report-mapper
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `odoo-fast-report-mapper-equitania-0.1.5/odoo_fast_report_mapper_equitania.egg-info/SOURCES.txt` & `odoo-fast-report-mapper-equitania-0.1.8/odoo_fast_report_mapper_equitania.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odoo-fast-report-mapper-equitania-0.1.5/odoo_report_helper/odoo_connection.py` & `odoo-fast-report-mapper-equitania-0.1.8/odoo_report_helper/odoo_connection.py`

 * *Files identical despite different names*

### Comparing `odoo-fast-report-mapper-equitania-0.1.5/odoo_report_helper/report.py` & `odoo-fast-report-mapper-equitania-0.1.8/odoo_report_helper/report.py`

 * *Files identical despite different names*

### Comparing `odoo-fast-report-mapper-equitania-0.1.5/odoo_report_helper/utils.py` & `odoo-fast-report-mapper-equitania-0.1.8/odoo_report_helper/utils.py`

 * *Files identical despite different names*

### Comparing `odoo-fast-report-mapper-equitania-0.1.5/setup.py` & `odoo-fast-report-mapper-equitania-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="odoo-fast-report-mapper-equitania",
-    version="0.1.5",
+    version="0.1.8",
     author="Equitania Software GmbH",
     author_email="info@equitania.de",
     description="A package to create FastReport entries in Odoo",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/equitania/odoo-fast-report-mapper",
     packages=['odoo_fast_report_mapper', 'odoo_report_helper'],
```

