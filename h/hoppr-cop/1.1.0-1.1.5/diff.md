# Comparing `tmp/hoppr_cop-1.1.0.tar.gz` & `tmp/hoppr_cop-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_cop-1.1.0.tar", max compression
+gzip compressed data, was "hoppr_cop-1.1.5.tar", max compression
```

## Comparing `hoppr_cop-1.1.0.tar` & `hoppr_cop-1.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1084 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/LICENSE.md
--rw-r--r--   0        0        0       55 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/__init__.py
--rw-r--r--   0        0        0        0 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/combined/__init__.py
--rw-r--r--   0        0        0     2719 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/combined/cli.py
--rw-r--r--   0        0        0     4488 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/combined/combined_scanner.py
--rw-r--r--   0        0        0        0 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/gemnasium/__init__.py
--rw-r--r--   0        0        0     9223 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/gemnasium/gemnasium_scanner.py
--rw-r--r--   0        0        0     1134 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/gemnasium/models.py
--rwxr-xr-x   0        0        0      113 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/gemnasium/semver
--rw-r--r--   0        0        0        0 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/grype/__init__.py
--rw-r--r--   0        0        0     5953 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/grype/grype_scanner.py
--rw-r--r--   0        0        0     5269 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/grype/models.py
--rw-r--r--   0        0        0     7725 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/hoppr_plugin/hopprcop_plugin.py
--rw-r--r--   0        0        0      478 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/ossindex/README.md
--rw-r--r--   0        0        0        0 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/ossindex/__init__.py
--rw-r--r--   0        0        0      832 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/ossindex/api/__init__.py
--rw-r--r--   0        0        0      899 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/ossindex/api/exception.py
--rw-r--r--   0        0        0     9487 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/ossindex/api/model.py
--rw-r--r--   0        0        0    11634 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/ossindex/api/ossindex.py
--rw-r--r--   0        0        0      153 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/ossindex/api/py.typed
--rw-r--r--   0        0        0     3147 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/ossindex/api/serializer.py
--rw-r--r--   0        0        0     4924 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/ossindex/oss_index_scanner.py
--rw-r--r--   0        0        0        0 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/trivy/__init__.py
--rw-r--r--   0        0        0     3293 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/hopprcop/trivy/trivy_scanner.py
--rw-r--r--   0        0        0      856 2023-03-02 22:09:07.000000 hoppr_cop-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 hoppr_cop-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/LICENSE.md
+-rw-r--r--   0        0        0       55 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/combined/__init__.py
+-rw-r--r--   0        0        0     3336 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/combined/cli.py
+-rw-r--r--   0        0        0     4488 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/combined/combined_scanner.py
+-rw-r--r--   0        0        0        0 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/gemnasium/__init__.py
+-rw-r--r--   0        0        0     9223 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/gemnasium/gemnasium_scanner.py
+-rw-r--r--   0        0        0     1134 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/gemnasium/models.py
+-rwxr-xr-x   0        0        0      113 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/gemnasium/semver
+-rw-r--r--   0        0        0        0 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/grype/__init__.py
+-rw-r--r--   0        0        0     5953 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/grype/grype_scanner.py
+-rw-r--r--   0        0        0     5289 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/grype/models.py
+-rw-r--r--   0        0        0     9731 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/hoppr_plugin/hopprcop_plugin.py
+-rw-r--r--   0        0        0      478 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/__init__.py
+-rw-r--r--   0        0        0      832 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/api/__init__.py
+-rw-r--r--   0        0        0     1029 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/api/exception.py
+-rw-r--r--   0        0        0     9487 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/api/model.py
+-rw-r--r--   0        0        0    11624 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/api/ossindex.py
+-rw-r--r--   0        0        0      153 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/api/py.typed
+-rw-r--r--   0        0        0     3147 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/api/serializer.py
+-rw-r--r--   0        0        0     4924 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/ossindex/oss_index_scanner.py
+-rw-r--r--   0        0        0        0 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/trivy/__init__.py
+-rw-r--r--   0        0        0     5558 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/hopprcop/trivy/trivy_scanner.py
+-rw-r--r--   0        0        0      853 2023-04-11 21:46:26.000000 hoppr_cop-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 hoppr_cop-1.1.5/PKG-INFO
```

### Comparing `hoppr_cop-1.1.0/LICENSE.md` & `hoppr_cop-1.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.0/hopprcop/combined/cli.py` & `hoppr_cop-1.1.5/hopprcop/combined/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """A Vulnerability Scanner that combines results from all configured scanners"""
 # pylint: disable=duplicate-code
+import traceback
 from pathlib import Path
 from typing import List
 
 import typer
 from security_commons.common.reporting.models import ReportFormat
 from security_commons.common.reporting.reporting import Reporting
 from security_commons.common.utils import parse_sbom, parse_sbom_json_string
@@ -37,37 +38,56 @@
         help=(
             "The operating system distribution; this is important "
             "to ensure accurate reporting of OS vulnerabilities from grype. "
             "Examples include rhel:8.6 or rocky:9 "
         ),
         envvar="OS_DISTRIBUTION",
     ),
+    trace: bool = typer.Option(
+        False, help="Print traceback information on unhandled error"
+    ),
 ):
     """Generates vulnerability reports based on the specified BOM and formats"""
+
     try:
         if base_report_name is None:
             if bom.endswith(".json"):
                 base_report_name = bom.removesuffix(".json")
             elif bom.endswith(".xml"):
                 base_report_name = bom.removesuffix(".xml")
             else:
                 base_report_name = "hoppr-cop-report"
 
         reporting = Reporting(output_dir, base_report_name)
         combined = CombinedScanner()
         grype_scanner = GrypeScanner()
+        trivy_scanner = TrivyScanner()
         grype_scanner.grype_os_distro = os_distro
+        trivy_scanner.trivy_os_distro = os_distro
         combined.set_scanners(
-            [grype_scanner, TrivyScanner(), OSSIndexScanner(), GemnasiumScanner()]
+            [grype_scanner, trivy_scanner, OSSIndexScanner(), GemnasiumScanner()]
         )
 
         parsed_bom = None
 
         if bom.endswith(".json") or bom.endswith(".xml"):
+            if not Path(bom).exists():
+                msg = typer.style(
+                    bom + " does not exist",
+                    fg=typer.colors.RED,
+                )
+                typer.echo(msg)
+                raise typer.Exit(code=1)
             parsed_bom = parse_sbom(Path(bom))
         else:
             parsed_bom = parse_sbom_json_string(bom, "The json provided sbom")
 
         results = combined.get_vulnerabilities_by_sbom(parsed_bom)
         reporting.generate_vulnerability_reports(formats, results, parsed_bom)
     except Exception as exc:  # pylint: disable=broad-except
-        print(f"unexpected error: {exc}")
+        if trace:
+            print(traceback.format_exc())
+        msg = typer.style(
+            f"unexpected error: {exc}",
+            fg=typer.colors.RED,
+        )
+        typer.echo(msg)
```

### Comparing `hoppr_cop-1.1.0/hopprcop/combined/combined_scanner.py` & `hoppr_cop-1.1.5/hopprcop/combined/combined_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.0/hopprcop/gemnasium/gemnasium_scanner.py` & `hoppr_cop-1.1.5/hopprcop/gemnasium/gemnasium_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.0/hopprcop/gemnasium/models.py` & `hoppr_cop-1.1.5/hopprcop/gemnasium/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.0/hopprcop/grype/grype_scanner.py` & `hoppr_cop-1.1.5/hopprcop/grype/grype_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.0/hopprcop/grype/models.py` & `hoppr_cop-1.1.5/hopprcop/grype/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     advisories: List
 
 
 class RelatedVulnerability(BaseModel):
     id: str
     data_source: str = Field(..., alias="dataSource")
     namespace: str
-    severity: str
+    severity: Optional[str]
     urls: List[str]
     description: str
     cvss: List[Cvs]
 
 
 class SearchedBy(BaseModel):
     language: Optional[str]
@@ -176,15 +176,15 @@
     exclude: List
     db: Db
     external_sources: ExternalSources = Field(..., alias="externalSources")
     dev: Dev
     fail_on_severity: str = Field(..., alias="fail-on-severity")
     registry: Registry
     log: Log
-    attestation: Attestation
+    attestation: Optional[Attestation]
 
 
 class Db1(BaseModel):
     built: str
     schema_version: int = Field(..., alias="schemaVersion")
     location: str
     checksum: str
```

### Comparing `hoppr_cop-1.1.0/hopprcop/hoppr_plugin/hopprcop_plugin.py` & `hoppr_cop-1.1.5/hopprcop/hoppr_plugin/hopprcop_plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 import uuid
+
 from copy import deepcopy
 from pathlib import Path
-from typing import List
 
-from hoppr.base_plugins.hoppr import HopprPlugin, hoppr_process
-from hoppr.result import Result
-from hoppr.hoppr_types.bom_access import BomAccess
-from hoppr_cyclonedx_models.cyclonedx_1_4 import (
-    Component,
-    CyclonedxSoftwareBillOfMaterialsStandard as Bom_1_4,
-    Vulnerability,
-    Affect,
-)
+from hoppr import BomAccess, Component, HopprPlugin, Result, Sbom, hoppr_process
 
-from security_commons.common.reporting.reporting import Reporting
+from hoppr_cyclonedx_models.cyclonedx_1_4 import Affect, Vulnerability
+from packageurl import PackageURL
 from security_commons.common.reporting.models import ReportFormat
+from security_commons.common.reporting.reporting import Reporting
 from security_commons.common.vulnerability_combiner import combine_vulnerabilities
-from hopprcop.combined.combined_scanner import CombinedScanner
 
 from hopprcop import __version__
+from hopprcop.combined.combined_scanner import CombinedScanner
 
 
 class HopprCopPlugin(HopprPlugin):
     """
     hoppr plugin wrapper for hopprcop integration
     """
 
     EMBEDDED_VEX = "embedded_cyclone_dx_vex"
     LINKED_VEX = "linked_cyclone_dx_vex"
 
     bom_access = BomAccess.FULL_ACCESS
 
+    supported_purl_types = [
+        "golang",
+        "npm",
+        "maven",
+        "pypi",
+        "nuget",
+        "gem",
+        "rpm",
+        "deb",
+    ]
+
     def get_version(self) -> str:
         """
         __version__ required for all HopprPlugin implementations
         """
         return __version__
 
     @hoppr_process
     def pre_stage_process(self) -> Result:
         """
         Supply sbom to hoppr cop to perform vulnerabilty check
         """
         self.get_logger().info("[ Executing hopprcop vulnerability check ]")
-        self.get_logger().flush()
 
         output_dir = self.config.get(
             "output_dir", Path(self.context.collect_root_dir, "generic")
         )
         base_report_name = self.config.get(
             "base_report_name", "hopprcop-vulnerability-results"
         )
@@ -57,22 +61,30 @@
         output_dir.mkdir(parents=True, exist_ok=True)
 
         reporting = Reporting(output_dir, base_report_name)
         combined = CombinedScanner()
         combined.set_scanners(scanners)
         parsed_bom = self.context.delivered_sbom
 
+        parsed_bom.components = list(
+            filter(
+                lambda x: PackageURL.from_string(x.purl).type
+                in self.supported_purl_types,
+                parsed_bom.components,
+            )
+        )
+
         results = combined.get_vulnerabilities_by_sbom(parsed_bom)
 
         # Map bom ref to results - uses purl as ref
         bom_ref_to_results = dict[str, self.ComponentVulnerabilityWrapper]()
 
-        # Map purls to components
+        # Map purls to components, try to normalize purls to lowercase
         purl_to_component = {
-            component.purl: component for component in parsed_bom.components
+            component.purl.lower(): component for component in parsed_bom.components
         }
 
         # Delivered Bom version
         bom_version = 1 if parsed_bom.version is not None else parsed_bom.version
 
         # Generate Delivered Bom Serial Number if it doesn't exist
         bom_serial_number = (
@@ -84,73 +96,108 @@
         parsed_bom.serialNumber = f"urn:uuid:{bom_serial_number}"
         parsed_bom.vulnerabilities = (
             [] if parsed_bom.vulnerabilities is None else parsed_bom.vulnerabilities
         )
 
         # Build dictionary to go from bom-ref to vulnerabilities
         for purl in results:
-            component = purl_to_component[purl]
-            bom_ref = component.purl  # component.bom_ref.__root__
-
-            if len(parsed_bom.vulnerabilities) > 0:
-                # Account for existing vulnerabilites on bom
-                for existing_vulnerability in parsed_bom.vulnerabilities:
-                    for affect in existing_vulnerability.affects:
-                        if (
-                            affect.ref == bom_ref
-                            or affect.ref == component.bom_ref.__root__
-                        ):
-                            results[purl].append(existing_vulnerability)
-
-                results[purl] = combine_vulnerabilities([{purl: results[purl]}])[0]
-
-            updated_results = deepcopy(results[purl])
-
-            wrapper = self.ComponentVulnerabilityWrapper(
-                bom_serial_number, bom_version, updated_results
-            )
-            bom_ref_to_results[bom_ref] = wrapper
+            # Different purl values being returned from different scanners, attempt to normalize the data
+            # by making it lower case and if not found, reversing pypi expectations with - to _.
+            adjusted_purl = purl.lower()
+            if adjusted_purl not in purl_to_component and "pypi" in adjusted_purl:
+                adjusted_purl = adjusted_purl.replace("-", "_")
+
+            if adjusted_purl in purl_to_component:
+                component = purl_to_component[adjusted_purl]
+                bom_ref = component.purl  # component.bom_ref.__root__
+                if (
+                    len(parsed_bom.vulnerabilities) > 0
+                    and bom_ref not in bom_ref_to_results
+                ):
+                    # Account for existing vulnerabilites on bom
+                    for existing_vulnerability in parsed_bom.vulnerabilities:
+                        for affect in existing_vulnerability.affects:
+                            if (
+                                affect.ref == bom_ref
+                                or affect.ref == component.bom_ref.__root__
+                            ):
+                                results[purl].append(existing_vulnerability)
+
+                    results[purl] = combine_vulnerabilities([{purl: results[purl]}])[0]
+
+                updated_results = deepcopy(results[purl])
+
+                if bom_ref not in bom_ref_to_results:
+                    wrapper = self.ComponentVulnerabilityWrapper(
+                        bom_serial_number, bom_version, updated_results
+                    )
+                    bom_ref_to_results[bom_ref] = wrapper
+                elif (
+                    len(bom_ref_to_results[bom_ref].vulnerabilities) > 0
+                    and len(updated_results) > 0
+                ):
+                    existing_vulnerabilities: list[Vulnerability] = bom_ref_to_results[
+                        bom_ref
+                    ].vulnerabilities
+                    bom_ref_to_results[
+                        bom_ref
+                    ].vulnerabilities = combine_vulnerabilities(
+                        [{purl: updated_results + existing_vulnerabilities}]
+                    )[
+                        0
+                    ]
+            else:
+                self.get_logger().info(f"Could not find purl ({purl}) in component map")
 
         hoppr_delivered_bom = self.__perform_hoppr_bom_updates(
             reporting, deepcopy(parsed_bom), bom_ref_to_results, formats
         )
         self.__perform_hopprcop_reporting(reporting, parsed_bom, results, formats)
 
+        self.get_logger().flush()
+
         return Result.success(return_obj=hoppr_delivered_bom)
 
     def __add_bom_ref_and_flatten(
         self,
         reporting: Reporting,
-        bom_ref_to_component: dict[str, List[Component]],
+        bom_ref_to_component: dict[str, list[Component]],
         external_ref: bool = False,
-    ) -> List[Vulnerability]:
-        flattened_vulnerabilities: List[Vulnerability] = []
+    ) -> list[Vulnerability]:
+        flattened_vulnerabilities: list[Vulnerability] = []
+        # Capture vulnerability id to vulnerability to account multiple components affected by the same vulnerability
+        vuln_id_to_vuln = {}
         for bom_ref in bom_ref_to_component:
             for vuln in bom_ref_to_component[bom_ref].vulnerabilities:
-                vuln.affects = [] if vuln.affects is None else vuln.affects
+                existing_vuln = vuln
+                if existing_vuln.id not in vuln_id_to_vuln:
+                    existing_vuln.affects = []
+                else:
+                    existing_vuln = vuln_id_to_vuln[vuln.id]
+
                 if external_ref:
-                    vuln.affects.append(
+                    existing_vuln.affects.append(
                         Affect(
-                            **{
-                                "ref": f"urn:cdx:{bom_ref_to_component[bom_ref].serial_number}/{bom_ref_to_component[bom_ref].version}#{bom_ref}"
-                            }
+                            ref=f"urn:cdx:{bom_ref_to_component[bom_ref].serial_number}/{bom_ref_to_component[bom_ref].version}#{bom_ref}"
                         )
                     )
                 else:
-                    vuln.affects.append(Affect(**{"ref": bom_ref}))
+                    existing_vuln.affects.append(Affect(ref=bom_ref))
 
-                flattened_vulnerabilities.append(vuln)
+                vuln_id_to_vuln[vuln.id] = existing_vuln
 
+        flattened_vulnerabilities = list(vuln_id_to_vuln.values())
         flattened_vulnerabilities.sort(key=reporting.get_score, reverse=True)
+
         return flattened_vulnerabilities
 
     def __perform_hoppr_bom_updates(
         self,
         reporting: Reporting,
-        parsed_bom: Bom_1_4,
+        parsed_bom: Sbom,
         bom_ref_to_results: dict[str, any],
         formats,
     ):
         if self.EMBEDDED_VEX in formats:
             flattened_results = self.__add_bom_ref_and_flatten(
                 reporting, bom_ref_to_results
             )
@@ -173,17 +220,17 @@
                 file.close()
 
         return parsed_bom
 
     def __perform_hopprcop_reporting(
         self,
         reporting: Reporting,
-        parsed_bom: Bom_1_4,
-        results: dict[str, List[Vulnerability]],
-        formats: List[str],
+        parsed_bom: Sbom,
+        results: dict[str, list[Vulnerability]],
+        formats: list[str],
     ):
         filtered_formats = list(
             filter(lambda x: x != self.LINKED_VEX and x != self.EMBEDDED_VEX, formats)
         )
 
         if len(filtered_formats) > 0:
             filtered_formats = [
@@ -196,15 +243,15 @@
     class ComponentVulnerabilityWrapper:
         def __init__(self, serial_number=None, version=None, vulnerabilities=None):
             self.serial_number = serial_number
             self.version = version
             self.vulnerabilities = vulnerabilities
 
 
-def get_scanners() -> List[str]:
+def get_scanners() -> list[str]:
     """Defines scanners to use for hoppr cop"""
     return [
         "hopprcop.gemnasium.gemnasium_scanner.GemnasiumScanner",
         "hopprcop.grype.grype_scanner.GrypeScanner",
         "hopprcop.trivy.trivy_scanner.TrivyScanner",
         "hopprcop.ossindex.oss_index_scanner.OSSIndexScanner",
     ]
```

### Comparing `hoppr_cop-1.1.0/hopprcop/ossindex/api/__init__.py` & `hoppr_cop-1.1.5/hopprcop/ossindex/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.0/hopprcop/ossindex/api/exception.py` & `hoppr_cop-1.1.5/hopprcop/ossindex/api/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,7 +22,13 @@
     """
 
 
 class AccessDeniedException(OssIndexException):
     """
     Raised if supplied credentials for Oss Index are invalid.
     """
+
+
+class RateLimitException(OssIndexException):
+    """
+    Raised if oss index returns a 429 too many requests exception.
+    """
```

### Comparing `hoppr_cop-1.1.0/hopprcop/ossindex/api/model.py` & `hoppr_cop-1.1.5/hopprcop/ossindex/api/model.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.0/hopprcop/ossindex/api/ossindex.py` & `hoppr_cop-1.1.5/hopprcop/ossindex/api/ossindex.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import yaml
 
 # See https://github.com/package-url/packageurl-python/issues/65
 from packageurl import PackageURL  # type: ignore
 from tinydb import TinyDB, Query
 from tinydb.table import Document
 
-from .exception import AccessDeniedException
+from .exception import AccessDeniedException, RateLimitException
 from .model import OssIndexComponent
 from .serializer import json_decoder, OssIndexJsonEncoder
 
 logger = logging.getLogger("ossindex")
 
 if sys.version_info >= (3, 8):
     from importlib.metadata import version as meta_version
@@ -219,16 +219,15 @@
             json={"coordinates": list(map(lambda p: str(p.to_string()), packages))},
             auth=self.oss_index_authentication,
         )
 
         if not response.status_code == 200:
             print(response.status_code)
             if response.status_code == 429:
-                time.sleep(90)
-            raise AccessDeniedException()
+                raise RateLimitException()
 
         results: List[OssIndexComponent] = []
         for oic in response.json(object_hook=json_decoder):
             results.append(oic)
 
         if self._caching_enabled:
             self._upsert_cache_with_oss_index_responses(oss_components=results)
```

### Comparing `hoppr_cop-1.1.0/hopprcop/ossindex/api/serializer.py` & `hoppr_cop-1.1.5/hopprcop/ossindex/api/serializer.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.0/hopprcop/ossindex/oss_index_scanner.py` & `hoppr_cop-1.1.5/hopprcop/ossindex/oss_index_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.1.0/pyproject.toml` & `hoppr_cop-1.1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 [tool.poetry]
 name = "hoppr-cop"
-version = "1.1.0"
+version = "1.1.5"
 description = ""
 authors = ["kganger <keith.e.ganger@lmco.com>"]
 license = "MIT"
 
 [[tool.poetry.packages]]
 include = "hopprcop"
 
 [tool.poetry.dependencies]
-python = "^3.10 "
+python = "^3.10"
 hoppr-cyclonedx-models = ">=0.4.7"
 typer = "^0.7.0"
 PyYAML = "^6.0"
 cvss = "^2.5"
 packageurl-python = "^0.10.1"
 tabulate = "^0.9.0"
 tinydb = "^4.7.0"
 rich = ">12.5.1"
 mkdocs = "^1.3.1"
 mkdocs-mermaid2-plugin = "^0.6.0"
-hoppr = "^1.7.2"
-pytest = "7.2.1"
+hoppr = "^1.8.0"
+pytest = "7.3.0"
 coverage = "^7.0.0"
 hoppr-security-commons = "^0.0.13"
 mkdocs-glightbox = "^0.3.1"
 pygments = "^2.14.0"
 pymdown-extensions = "^9.9.2"
 
 [tool.poetry.scripts]
 hoppr-cop = "hopprcop.combined.cli:app"
 
-
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 black = "^23.0.0"
 pylint = "^2.14.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
-
```

### Comparing `hoppr_cop-1.1.0/PKG-INFO` & `hoppr_cop-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: hoppr-cop
-Version: 1.1.0
+Version: 1.1.5
 Summary: 
 License: MIT
 Author: kganger
 Author-email: keith.e.ganger@lmco.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: coverage (>=7.0.0,<8.0.0)
 Requires-Dist: cvss (>=2.5,<3.0)
-Requires-Dist: hoppr (>=1.7.2,<2.0.0)
+Requires-Dist: hoppr (>=1.8.0,<2.0.0)
 Requires-Dist: hoppr-cyclonedx-models (>=0.4.7)
 Requires-Dist: hoppr-security-commons (>=0.0.13,<0.0.14)
 Requires-Dist: mkdocs (>=1.3.1,<2.0.0)
 Requires-Dist: mkdocs-glightbox (>=0.3.1,<0.4.0)
 Requires-Dist: mkdocs-mermaid2-plugin (>=0.6.0,<0.7.0)
 Requires-Dist: packageurl-python (>=0.10.1,<0.11.0)
 Requires-Dist: pygments (>=2.14.0,<3.0.0)
 Requires-Dist: pymdown-extensions (>=9.9.2,<10.0.0)
-Requires-Dist: pytest (==7.2.1)
+Requires-Dist: pytest (==7.3.0)
 Requires-Dist: rich (>12.5.1)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tinydb (>=4.7.0,<5.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
```

