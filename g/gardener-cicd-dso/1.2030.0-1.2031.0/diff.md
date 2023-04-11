# Comparing `tmp/gardener-cicd-dso-1.2030.0.tar.gz` & `tmp/gardener-cicd-dso-1.2031.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-dso-1.2030.0.tar", last modified: Fri Apr  7 16:33:10 2023, max compression
+gzip compressed data, was "gardener-cicd-dso-1.2031.0.tar", last modified: Tue Apr 11 14:25:22 2023, max compression
```

## Comparing `gardener-cicd-dso-1.2030.0.tar` & `gardener-cicd-dso-1.2031.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:33:10.044254 gardener-cicd-dso-1.2030.0/
--rw-r--r--   0 root         (0) root         (0)    16830 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-07 16:33:10.044254 gardener-cicd-dso-1.2030.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:33:10.040254 gardener-cicd-dso-1.2030.0/checkmarx/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/checkmarx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7623 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/checkmarx/client.py
--rw-r--r--   0 root         (0) root         (0)     3746 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/checkmarx/model.py
--rw-r--r--   0 root         (0) root         (0)     7006 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/checkmarx/project.py
--rw-r--r--   0 root         (0) root         (0)     5790 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/checkmarx/tablefmt.py
--rw-r--r--   0 root         (0) root         (0)    17856 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/checkmarx/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:33:10.044254 gardener-cicd-dso-1.2030.0/clamav/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/clamav/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5287 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/clamav/client.py
--rw-r--r--   0 root         (0) root         (0)     5266 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/clamav/cnudie.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/clamav/model.py
--rw-r--r--   0 root         (0) root         (0)     1339 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/clamav/report.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/clamav/routes.py
--rw-r--r--   0 root         (0) root         (0)     7689 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/clamav/scan.py
--rw-r--r--   0 root         (0) root         (0)     6135 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/clamav/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:33:10.044254 gardener-cicd-dso-1.2030.0/gardener_cicd_dso.egg-info/
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-07 16:33:09.000000 gardener-cicd-dso-1.2030.0/gardener_cicd_dso.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      688 2023-04-07 16:33:10.000000 gardener-cicd-dso-1.2030.0/gardener_cicd_dso.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 16:33:09.000000 gardener-cicd-dso-1.2030.0/gardener_cicd_dso.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-07 16:33:09.000000 gardener-cicd-dso-1.2030.0/gardener_cicd_dso.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-07 16:33:09.000000 gardener-cicd-dso-1.2030.0/gardener_cicd_dso.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 16:33:10.044254 gardener-cicd-dso-1.2030.0/protecode/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/protecode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5756 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/protecode/assessments.py
--rw-r--r--   0 root         (0) root         (0)    17050 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/protecode/client.py
--rw-r--r--   0 root         (0) root         (0)    11985 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/protecode/model.py
--rw-r--r--   0 root         (0) root         (0)     3645 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/protecode/report.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/protecode/rescore.py
--rw-r--r--   0 root         (0) root         (0)    24660 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/protecode/scanning.py
--rw-r--r--   0 root         (0) root         (0)     8437 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/protecode/util.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-04-07 16:33:10.044254 gardener-cicd-dso-1.2030.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      673 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/setup.dso.py
--rw-r--r--   0 root         (0) root         (0)     2096 2023-04-07 16:32:17.000000 gardener-cicd-dso-1.2030.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:25:22.595543 gardener-cicd-dso-1.2031.0/
+-rw-r--r--   0 root         (0) root         (0)    16830 2023-04-11 14:23:16.000000 gardener-cicd-dso-1.2031.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-11 14:23:16.000000 gardener-cicd-dso-1.2031.0/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)      171 2023-04-11 14:25:22.595543 gardener-cicd-dso-1.2031.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-04-11 14:23:16.000000 gardener-cicd-dso-1.2031.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:25:22.591543 gardener-cicd-dso-1.2031.0/checkmarx/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-11 14:23:16.000000 gardener-cicd-dso-1.2031.0/checkmarx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7623 2023-04-11 14:23:16.000000 gardener-cicd-dso-1.2031.0/checkmarx/client.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2023-04-11 14:23:16.000000 gardener-cicd-dso-1.2031.0/checkmarx/model.py
+-rw-r--r--   0 root         (0) root         (0)     7006 2023-04-11 14:23:16.000000 gardener-cicd-dso-1.2031.0/checkmarx/project.py
+-rw-r--r--   0 root         (0) root         (0)     5790 2023-04-11 14:23:16.000000 gardener-cicd-dso-1.2031.0/checkmarx/tablefmt.py
+-rw-r--r--   0 root         (0) root         (0)    17856 2023-04-11 14:23:16.000000 gardener-cicd-dso-1.2031.0/checkmarx/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:25:22.591543 gardener-cicd-dso-1.2031.0/clamav/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/clamav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5287 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/clamav/client.py
+-rw-r--r--   0 root         (0) root         (0)     5266 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/clamav/cnudie.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/clamav/model.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/clamav/report.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/clamav/routes.py
+-rw-r--r--   0 root         (0) root         (0)     7689 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/clamav/scan.py
+-rw-r--r--   0 root         (0) root         (0)     6135 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/clamav/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:25:22.591543 gardener-cicd-dso-1.2031.0/gardener_cicd_dso.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-04-11 14:25:22.000000 gardener-cicd-dso-1.2031.0/gardener_cicd_dso.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      688 2023-04-11 14:25:22.000000 gardener-cicd-dso-1.2031.0/gardener_cicd_dso.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 14:25:22.000000 gardener-cicd-dso-1.2031.0/gardener_cicd_dso.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-11 14:25:22.000000 gardener-cicd-dso-1.2031.0/gardener_cicd_dso.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-11 14:25:22.000000 gardener-cicd-dso-1.2031.0/gardener_cicd_dso.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:25:22.595543 gardener-cicd-dso-1.2031.0/protecode/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/protecode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5756 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/protecode/assessments.py
+-rw-r--r--   0 root         (0) root         (0)    17050 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/protecode/client.py
+-rw-r--r--   0 root         (0) root         (0)    11985 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/protecode/model.py
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/protecode/report.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/protecode/rescore.py
+-rw-r--r--   0 root         (0) root         (0)    24660 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/protecode/scanning.py
+-rw-r--r--   0 root         (0) root         (0)     8437 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/protecode/util.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-04-11 14:25:22.595543 gardener-cicd-dso-1.2031.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      673 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/setup.dso.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-04-11 14:23:17.000000 gardener-cicd-dso-1.2031.0/setup.py
```

### Comparing `gardener-cicd-dso-1.2030.0/LICENSE.md` & `gardener-cicd-dso-1.2031.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/README.md` & `gardener-cicd-dso-1.2031.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/checkmarx/__init__.py` & `gardener-cicd-dso-1.2031.0/checkmarx/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/checkmarx/client.py` & `gardener-cicd-dso-1.2031.0/checkmarx/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/checkmarx/model.py` & `gardener-cicd-dso-1.2031.0/checkmarx/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/checkmarx/project.py` & `gardener-cicd-dso-1.2031.0/checkmarx/project.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/checkmarx/tablefmt.py` & `gardener-cicd-dso-1.2031.0/checkmarx/tablefmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/checkmarx/util.py` & `gardener-cicd-dso-1.2031.0/checkmarx/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/clamav/__init__.py` & `gardener-cicd-dso-1.2031.0/clamav/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/clamav/client.py` & `gardener-cicd-dso-1.2031.0/clamav/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/clamav/cnudie.py` & `gardener-cicd-dso-1.2031.0/clamav/cnudie.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/clamav/model.py` & `gardener-cicd-dso-1.2031.0/clamav/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/clamav/report.py` & `gardener-cicd-dso-1.2031.0/clamav/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/clamav/routes.py` & `gardener-cicd-dso-1.2031.0/clamav/routes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/clamav/scan.py` & `gardener-cicd-dso-1.2031.0/clamav/scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/clamav/util.py` & `gardener-cicd-dso-1.2031.0/clamav/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/gardener_cicd_dso.egg-info/SOURCES.txt` & `gardener-cicd-dso-1.2031.0/gardener_cicd_dso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/protecode/__init__.py` & `gardener-cicd-dso-1.2031.0/protecode/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/protecode/assessments.py` & `gardener-cicd-dso-1.2031.0/protecode/assessments.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/protecode/client.py` & `gardener-cicd-dso-1.2031.0/protecode/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/protecode/model.py` & `gardener-cicd-dso-1.2031.0/protecode/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/protecode/report.py` & `gardener-cicd-dso-1.2031.0/protecode/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/protecode/rescore.py` & `gardener-cicd-dso-1.2031.0/protecode/rescore.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import logging
 import typing
 
 import cnudie.iter
 import dso.cvss
 import dso.labels
 import protecode.client
 import protecode.model
 
+logger = logging.getLogger(__name__)
+
 
 def cve_categorisation(
     resource_node: cnudie.iter.ResourceNode,
     absent_ok: bool=True,
 ) -> dso.cvss.CveCategorisation | None:
     label_name = dso.labels.CveCategorisationLabel.name
     label = resource_node.resource.find_label(name=label_name)
@@ -34,32 +37,31 @@
     rescores bdba-findings for the given resource-node. Rescoring is only possible if
     cve-categorisations are available from categoristion-label in either resource or component.
     '''
     if not (categorisation := cve_categorisation(resource_node=resource_node)):
         return scan_result
 
     product_id = scan_result.product_id()
+    component = resource_node.component
+    resource = resource_node.resource
+
+    logger.info(f'rescoring {component.name}:{resource.name} - {product_id=}')
 
     all_components = tuple(scan_result.components())
     components_with_vulnerabilities = [c for c in all_components if tuple(c.vulnerabilities())]
 
     components_with_vulnerabilities = sorted(
         components_with_vulnerabilities,
         key=lambda c: c.name()
     )
 
-    total_vulns = 0
-    total_rescored = 0
-
     for c in components_with_vulnerabilities:
         if not c.version():
             continue # do not inject dummy-versions in fully automated mode, yet
 
-        vulns_count = 0
-        rescored_count = 0
         vulns_to_assess = []
 
         for v in c.vulnerabilities():
             if v.historical():
                 continue
             if v.has_triage():
                 continue
@@ -67,46 +69,37 @@
             if not v.cvss:
                 continue # happens if only cvss-v2 is available - ignore for now
 
             orig_severity = dso.cvss.CVESeverity.from_cve_score(v.cve_severity())
             if orig_severity > max_rescore_severity:
                 continue
 
-            vulns_count += 1
-
             matching_rules = dso.cvss.matching_rescore_rules(
                 rescoring_rules=rescoring_rules,
                 categorisation=categorisation,
                 cvss=v.cvss,
             )
             rescored = dso.cvss.rescore(
                 rescoring_rules=tuple(matching_rules),
                 severity=orig_severity,
             )
 
-            if orig_severity is not rescored:
-                rescored_count += 1
-
-                if rescored is dso.cvss.CVESeverity.NONE:
-                    vulns_to_assess.append(v)
+            if rescored is dso.cvss.CVESeverity.NONE:
+                vulns_to_assess.append(v)
 
         if vulns_to_assess:
+            logger.info(f'{len(vulns_to_assess)=}: {[v.cve() for v in vulns_to_assess]}')
             bdba_client.add_triage_raw({
                 'component': c.name(),
-                'version': c.version() or 'does-not-matter',
+                'version': c.version(),
                 'vulns': [v.cve() for v in vulns_to_assess],
                 'scope': protecode.model.TriageScope.RESULT.value,
                 'reason': 'OT',
                 'description': 'auto-assessed as irrelevant based on cve-categorisation',
                 'product_id': product_id,
             })
-            print(f'auto-assessed {len(vulns_to_assess)=}')
-
-        total_vulns += vulns_count
-        total_rescored += rescored_count
 
-    print(f'{total_vulns=}, {total_rescored=}')
-    if total_rescored > 0:
-        print(f'{total_rescored=} - retrieving result again from bdba (this may take a while)')
+    if vulns_to_assess:
+        logger.info('retrieving result again from bdba (this may take a while)')
         scan_result = bdba_client.scan_result(product_id=scan_result.product_id())
 
     return scan_result
```

### Comparing `gardener-cicd-dso-1.2030.0/protecode/scanning.py` & `gardener-cicd-dso-1.2031.0/protecode/scanning.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/protecode/util.py` & `gardener-cicd-dso-1.2031.0/protecode/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/setup.dso.py` & `gardener-cicd-dso-1.2031.0/setup.dso.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2030.0/setup.py` & `gardener-cicd-dso-1.2031.0/setup.py`

 * *Files identical despite different names*

