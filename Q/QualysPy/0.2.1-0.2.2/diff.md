# Comparing `tmp/qualyspy-0.2.1.tar.gz` & `tmp/qualyspy-0.2.2.tar.gz`

## Comparing `qualyspy-0.2.1.tar` & `qualyspy-0.2.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.2.1/.vscode/launch.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.2.1/.vscode/settings.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.2.1/.vscode/tasks.json
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.2.1/debug/build.sh
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.2.1/debug/dtd.txt
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.2.1/debug/output.txt
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.2.1/debug/parse_dtd.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.2.1/debug/quickscan.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.2.1/debug/remove_cookies.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 qualyspy-0.2.1/debug/test.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.2.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.2.1/docs/make.bat
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.2.1/docs/source/conf.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.2.1/docs/source/index.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.2.1/docs/source/modules.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.1/docs/source/qualyspy.assets.host_list.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.2.1/docs/source/qualyspy.assets.host_list_detection.rst
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.2.1/docs/source/qualyspy.qualysapi.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.1/docs/source/qualyspy.qutils.rst
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.2.1/docs/source/qualyspy.rst
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.2.1/docs/source/qualyspy.scan_configuration.knowledgebase.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/__init__.py
--rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/qualysapi.py
--rw-r--r--   0        0        0    16363 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/qutils.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/urls.json
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/asset_mgmt_tagging/__init__.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/asset_mgmt_tagging/asset.py
--rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/asset_mgmt_tagging/tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/assets/__init__.py
--rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/assets/host_list.py
--rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/assets/host_list_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/certview/__init__.py
--rw-r--r--   0        0        0    15254 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/certview/certificate.py
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/certview/sql/certview_init.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/scan_configuration/__init__.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.2.1/qualyspy/scan_configuration/knowledgebase.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.2.1/requirements/deploy.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.2.1/requirements/dev.txt
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.2.1/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.2.1/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.2.1/README.md
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 qualyspy-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 qualyspy-0.2.2/.vscode/launch.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 qualyspy-0.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 qualyspy-0.2.2/.vscode/tasks.json
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/build.sh
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/dtd.txt
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/output.txt
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/parse_dtd.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/quickscan.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/remove_cookies.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 qualyspy-0.2.2/debug/test.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/make.bat
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/conf.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/index.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/modules.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/qualyspy.assets.host_list.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/qualyspy.assets.host_list_detection.rst
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/qualyspy.qualysapi.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/qualyspy.qutils.rst
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/qualyspy.rst
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 qualyspy-0.2.2/docs/source/qualyspy.scan_configuration.knowledgebase.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/__init__.py
+-rw-r--r--   0        0        0    17347 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/qualysapi.py
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/qutils.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/urls.json
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/asset_mgmt_tagging/__init__.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/asset_mgmt_tagging/asset.py
+-rw-r--r--   0        0        0     9905 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/asset_mgmt_tagging/tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/assets/__init__.py
+-rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/assets/host_list.py
+-rw-r--r--   0        0        0    40811 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/assets/host_list_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/certview/__init__.py
+-rw-r--r--   0        0        0    17219 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/certview/certificate.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/certview/sql/certview_init.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/scan_configuration/__init__.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.2.2/qualyspy/scan_configuration/knowledgebase.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.2.2/requirements/deploy.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 qualyspy-0.2.2/requirements/dev.txt
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 qualyspy-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.2.2/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 qualyspy-0.2.2/README.md
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 qualyspy-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 qualyspy-0.2.2/PKG-INFO
```

### Comparing `qualyspy-0.2.1/.vscode/launch.json` & `qualyspy-0.2.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/debug/dtd.txt` & `qualyspy-0.2.2/debug/dtd.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/debug/output.txt` & `qualyspy-0.2.2/debug/output.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/debug/parse_dtd.py` & `qualyspy-0.2.2/debug/parse_dtd.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/debug/quickscan.py` & `qualyspy-0.2.2/debug/quickscan.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/debug/remove_cookies.py` & `qualyspy-0.2.2/debug/remove_cookies.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/debug/test.py` & `qualyspy-0.2.2/debug/test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # type: ignore
 
 import inspect
 import os
 import sys
 
+import sqlalchemy as sa
+import sqlalchemy.orm as orm
+
 
 currentdir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
 parentdir = os.path.dirname(currentdir)
 sys.path.insert(0, parentdir)
 
 from qualyspy.qualysapi import Connection
 import qualyspy.certview.certificate as cert
 
 if __name__ == "__main__":
     conn = Connection(apis = ["CertView"])
-    #fvo = cert.Field_Value_Operator(field="certificate.serialNumber", operator="EQUALS", value="00b930ea6e650ce85c")
-    #filter = cert.Filter(filters=[fvo])
-    #input = cert.List_CertView_Certificates_v2_Input(filter=filter)
-    #cert = cert.list_certificates_v2(conn, input)
-
-    cert.init_db()
-    input = cert.List_CertView_Certificates_v2_Input(pageSize=200)
-    cert.list_certificates_v2(conn, input, load_db = True)
+    api = cert.List_Certificates_V2(conn)
+
+    # fvo = cert.Field_Value_Operator(field="certificate.id", operator="EQUALS", value="39534")
+    # filter = cert.Filter(filters=[fvo])
+    # input = cert.List_CertView_Certificates_V2_Input(filter=filter)
+    # test = api.call(input)
+
+    #api.reset(echo = True)
+    #test = api.load(echo=True)
+
+    stmt = sa.Select(cert.Certificate_ORM).where(cert.Certificate_ORM.self_signed == False)
+    test = api.query(stmt, echo = True)
 
     print("test")
```

### Comparing `qualyspy-0.2.1/docs/Makefile` & `qualyspy-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/docs/make.bat` & `qualyspy-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/docs/source/conf.py` & `qualyspy-0.2.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/qualyspy/qualysapi.py` & `qualyspy-0.2.2/qualyspy/qualysapi.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/qualyspy/qutils.py` & `qualyspy-0.2.2/qualyspy/qutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 import json
 import math
 import os
 import re
 import zoneinfo
 from collections.abc import MutableMapping, MutableSequence
 from typing import Any, Callable, Optional, TypeVar, Union
+import copy
 
 import lxml.etree
 import lxml.objectify
+import sqlalchemy.orm as orm
 
 _CONFIG_FILE = os.path.expanduser("~/qualysapi.conf")
 config = configparser.ConfigParser()
 config.read(_CONFIG_FILE)
 
 URLS = json.load(importlib.resources.files("qualyspy").joinpath("urls.json").open())
 DB_HOST = config["POSTGRESQL"]["host"]
@@ -447,14 +449,18 @@
 def to_lower_camel(string: str) -> str:
     if len(string) >= 1:
         pascal_string = to_camel(string)
         return pascal_string[0].lower() + pascal_string[1:]
     return string.lower()
 
 
+class Base(orm.DeclarativeBase):
+    pass
+
+
 _D = TypeVar("_D")
 re_classname = re.compile(r"(qualyspy[\w._]*)")
 re_sa_class = re.compile(r"sqlalchemy.orm")
 
 
 def _get_cls_inst_from_annot(mapped_cls: str) -> Any:
     m = re_classname.search(mapped_cls)
@@ -471,31 +477,31 @@
             raise ValueError("Annotation is not a Mapped class.")
 
 
 def to_orm_object(
     obj: dict[str, Any],
     out_cls: type[_D],
 ) -> _D:
+    obj_copy = copy.deepcopy(obj)
     annots = inspect.get_annotations(out_cls)
-    for k, v in obj.items():
+    for k, v in obj_copy.items():
         if isinstance(v, dict):
             mapped_cls = str(annots[k])
             child_cls = _get_cls_inst_from_annot(mapped_cls)
             if child_cls is None:
                 continue
-            obj[k] = to_orm_object(v, child_cls)
+            obj_copy[k] = to_orm_object(v, child_cls)
         elif isinstance(v, list) and len(v) > 0:
-            mapped_cls = str(annots[k])
-            child_cls = _get_cls_inst_from_annot(mapped_cls)
-            if child_cls is None:
-                continue
-            if isinstance(v[0], dict):
-                for i in range(len(v)):
-                    v[i] = to_orm_object(v[i], child_cls)
-            else:
-                child_annots = inspect.get_annotations(child_cls)
-                param = next(iter(child_annots))
-                for i in range(len(v)):
-                    bind = {param: v[i]}
-                    obj[k][i] = child_cls(**bind)
+            if not all(isinstance(item, Base) for item in v):
+                mapped_cls = str(annots[k])
+                child_cls = _get_cls_inst_from_annot(mapped_cls)
+                if child_cls is None:
+                    continue
+                if isinstance(v[0], dict):
+                    v = [to_orm_object(item, child_cls) for item in v]
+                else:
+                    child_annots = inspect.get_annotations(child_cls)
+                    param = next(iter(child_annots))
+                    v = [child_cls(**{param: item}) for item in v]
+            obj_copy[k] = v
 
-    return out_cls(**obj)
+    return out_cls(**obj_copy)
```

### Comparing `qualyspy-0.2.1/qualyspy/urls.json` & `qualyspy-0.2.2/qualyspy/urls.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/qualyspy/asset_mgmt_tagging/asset.py` & `qualyspy-0.2.2/qualyspy/asset_mgmt_tagging/asset.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/qualyspy/asset_mgmt_tagging/tags.py` & `qualyspy-0.2.2/qualyspy/asset_mgmt_tagging/tags.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/qualyspy/assets/host_list.py` & `qualyspy-0.2.2/qualyspy/assets/host_list.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/qualyspy/assets/host_list_detection.py` & `qualyspy-0.2.2/qualyspy/assets/host_list_detection.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/qualyspy/certview/certificate.py` & `qualyspy-0.2.2/qualyspy/certview/certificate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import datetime
 import importlib.resources
 import ipaddress
 from typing import Any
 
+import psycopg2.extensions
 import pydantic as pd
+import pydantic.networks
+import pydantic.utils
 import sqlalchemy as sa
-import sqlalchemy.orm as orm
 import sqlalchemy.dialects.postgresql as sa_pg
-import psycopg2.extensions
-import pydantic.networks
+import sqlalchemy.orm as orm
 
-from .. import qualysapi
-from .. import qutils
+from .. import qualysapi, qutils
 
 SQL = importlib.resources.files("qualyspy").joinpath("certview").joinpath("sql")
 
 
 class Base(orm.DeclarativeBase):
     pass
 
@@ -84,14 +84,16 @@
 
 class Subject_Alternative_Names(pd.BaseModel):
     dns_names = list[str]
     ip_address = list[str]
 
     class Config:
         alias_generator = qutils.to_lower_camel
+        orm_mode = True
+        allow_population_by_field_name = True
 
 
 ####################################################################################################
 
 ####################################################################################################
 # Subject
 
@@ -103,15 +105,17 @@
     locality: orm.Mapped[str]
     name: orm.Mapped[str] = orm.mapped_column(primary_key=True)
     state: orm.Mapped[str]
     country: orm.Mapped[str]
 
     organization_unit: orm.Mapped[list[str]] = orm.mapped_column(sa.ARRAY(sa.String))
 
-    certificate_id: orm.Mapped[int] = orm.mapped_column(sa.ForeignKey("certificate.id"))
+    certificate_id: orm.Mapped[int] = orm.mapped_column(
+        sa.ForeignKey("certificate.id"), primary_key=True
+    )
     certificate: orm.Mapped["Certificate_ORM"] = orm.relationship(
         back_populates="subject", uselist=False
     )
 
 
 class Subject(pd.BaseModel):
     organization: str
@@ -119,14 +123,16 @@
     name: str
     state: str
     country: str
     organization_unit: list[str] | None
 
     class Config:
         alias_generator = qutils.to_lower_camel
+        orm_mode = True
+        allow_population_by_field_name = True
 
 
 ####################################################################################################
 
 ####################################################################################################
 # Issuer
 
@@ -143,33 +149,19 @@
     locality: orm.Mapped[str]
 
     issuer_of: orm.Mapped[list["Certificate_ORM"]] = orm.relationship(
         back_populates="issuer"
     )
 
 
-class RootIssuer_OU_ORM(Base):
-    __tablename__ = "rootissuer_organization_unit"
-
-    id: orm.Mapped[str] = orm.mapped_column(primary_key=True)
-    name: orm.Mapped[str | None]
-
-    issuer_id: orm.Mapped[int] = orm.mapped_column(sa.ForeignKey("rootissuer.certhash"))
-    issuer: orm.Mapped["RootIssuer_ORM"] = orm.relationship(
-        back_populates="organization_unit", uselist=False
-    )
-
-
 class RootIssuer_ORM(Base):
     __tablename__ = "rootissuer"
 
     organization: orm.Mapped[str]
-    organization_unit: orm.Mapped[list[RootIssuer_OU_ORM]] = orm.relationship(
-        back_populates="issuer"
-    )
+    organization_unit: orm.Mapped[list[str]] = orm.mapped_column(sa.ARRAY(sa.String))
     name: orm.Mapped[str]
     country: orm.Mapped[str]
     state: orm.Mapped[str]
     certhash: orm.Mapped[str] = orm.mapped_column(primary_key=True)
     locality: orm.Mapped[str]
 
     rootissuer_of: orm.Mapped[list["Certificate_ORM"]] = orm.relationship(
@@ -184,26 +176,31 @@
     country: str
     state: str
     certhash: str
     locality: str
 
     class Config:
         alias_generator = qutils.to_lower_camel
+        orm_mode = True
+        allow_population_by_field_name = True
 
 
 ####################################################################################################
 # Host_Instance
 
 asset_host_instance_association_table = sa.Table(
     "asset_host_instance",
     Base.metadata,
+    sa.Column("asset_id", sa.INTEGER, sa.ForeignKey("asset.id"), primary_key=True),
     sa.Column(
-        "asset_id", sa.INTEGER, sa.ForeignKey("asset.id"), primary_key=True
+        "host_instance_id",
+        sa.INTEGER,
+        sa.ForeignKey("host_instance.id"),
+        primary_key=True,
     ),
-    sa.Column("host_instance_id", sa.INTEGER, sa.ForeignKey("host_instance.id"), primary_key=True),
 )
 
 
 class Host_Instance_ORM(Base):
     __tablename__ = "host_instance"
 
     id: orm.Mapped[int] = orm.mapped_column(primary_key=True)
@@ -222,14 +219,18 @@
     id: int
     port: int
     fqdn: str
     protocol: str
     service: str | None
     grade: str
 
+    class Config:
+        orm_mode = True
+        allow_population_by_field_name = True
+
 
 ####################################################################################################
 # Asset_Interface
 
 
 class Asset_Interface_ORM(Base):
     __tablename__ = "asset_interface"
@@ -245,14 +246,18 @@
     )
 
 
 class Asset_Interface(pd.BaseModel):
     hostname: str | None
     address: pd.IPvAnyAddress
 
+    class Config:
+        orm_mode = True
+        allow_population_by_field_name = True
+
 
 ####################################################################################################
 
 ####################################################################################################
 # Asset
 
 
@@ -284,14 +289,16 @@
     name: str
     operating_system: str | None
     host_instances: list[Host_Instance]
     asset_interfaces: list[Asset_Interface] | None
 
     class Config:
         alias_generator = qutils.to_lower_camel
+        orm_mode = True
+        allow_population_by_field_name = True
 
 
 ####################################################################################################
 # Certificate
 
 certificate_key_usage_association_table = sa.Table(
     "certificate_key_usage",
@@ -331,17 +338,17 @@
     valid_to_date: orm.Mapped[datetime.datetime]
     valid_to: orm.Mapped[int] = orm.mapped_column(sa.BigInteger)
     valid_from_date: orm.Mapped[datetime.datetime]
     valid_from: orm.Mapped[int] = orm.mapped_column(sa.BigInteger)
     signature_algorithm: orm.Mapped[str]
     extended_validation: orm.Mapped[bool]
     created_date: orm.Mapped[datetime.datetime]
-    dn: orm.Mapped[str]
+    dn: orm.Mapped[str | None]
     subject: orm.Mapped[Subject_ORM] = orm.relationship(
-        back_populates="certificate", uselist=False
+        back_populates="certificate", uselist=False, cascade="all, delete-orphan"
     )
     update_date: orm.Mapped[datetime.datetime]
     last_found: orm.Mapped[int] = orm.mapped_column(sa.BigInteger)
     imported: orm.Mapped[bool]
     self_signed: orm.Mapped[bool]
     issuer_certhash: orm.Mapped[str | None] = orm.mapped_column(
         sa.ForeignKey("issuer.certhash")
@@ -369,27 +376,38 @@
     subject_key_identifier: orm.Mapped[str | None]
     auth_key_identifier: orm.Mapped[str | None]
     subject_alternative_names: orm.Mapped[
         Subject_Alternative_Names_ORM | None
     ] = orm.relationship(back_populates="certificate", uselist=False)
 
 
+class Certiticate_Getter(pydantic.utils.GetterDict):
+    def get(self, key: str, default: Any = None) -> Any:
+        if key == "key_usage":
+            return [ku.usage for ku in self._obj.key_usage]
+        elif key == "enhanced_key_usage":
+            if self._obj.enhanced_key_usage is None:
+                return None
+            return [ku.usage for ku in self._obj.enhanced_key_usage]
+        return super().get(key, default)
+
+
 class Certificate(pd.BaseModel):
     id: int
     certhash: str
     key_size: int
     serial_number: str
     valid_to_date: datetime.datetime
     valid_to: int
     valid_from_date: datetime.datetime
     valid_from: int
     signature_algorithm: str
     extended_validation: bool
     created_date: datetime.datetime
-    dn: str
+    dn: str | None
     subject: Subject
     update_date: datetime.datetime
     last_found: int
     imported: bool
     self_signed: bool
     issuer: Issuer | None
     rootissuer: Issuer | None
@@ -402,14 +420,17 @@
     enhanced_key_usage: list[str] | None
     subject_key_identifier: str | None
     auth_key_identifier: str | None
     subject_alternative_names: Subject_Alternative_Names | None
 
     class Config:
         alias_generator = qutils.to_lower_camel
+        orm_mode = True
+        allow_population_by_field_name = True
+        getter_dict = Certiticate_Getter
 
 
 ####################################################################################################
 
 ####################################################################################################
 # Function input
 
@@ -421,86 +442,115 @@
 
 
 class Filter(pd.BaseModel):
     filters: list[Field_Value_Operator]
     operation: str = "AND"
 
 
-class List_CertView_Certificates_v2_Input(pd.BaseModel):
-    filter: Filter | None
+class List_CertView_Certificates_V2_Input(pd.BaseModel):
+    filter: Filter | None = None
     page_number: int = 0
-    page_size: int | None
-    exclude_fields: str | None
+    page_size: int | None = None
+    exclude_fields: str | None = None
 
     class Config:
         alias_generator = qutils.to_lower_camel
+        allow_population_by_field_name = True
 
 
 ####################################################################################################
 
 
-def list_certificates_v2(
-    conn: qualysapi.Connection,
-    api_input: List_CertView_Certificates_v2_Input = List_CertView_Certificates_v2_Input(
-        filter=None, page_size=None, exclude_fields=None
-    ),
-    load_db: bool = False,
-) -> list[Certificate] | None:
-    input_data = api_input.dict(by_alias=True, exclude_none=True)
-    input_data["includes"] = [
-        "ASSET_INTERFACES",
-        "SSL_PROTOCOLS",
-        "CIPHER_SUITES",
-        "EXTENSIVE_CERTIFICATE_INFO",
-    ]
-
-    if load_db:
-        e_url = qutils.E_URL
-        engine = sa.create_engine(e_url, echo=True)
-    else:
+class List_Certificates_V2:
+    def __init__(self, conn: qualysapi.Connection) -> None:
+        self.conn = conn
+
+    def __call_once(
+        self, params: List_CertView_Certificates_V2_Input
+    ) -> list[Certificate] | None:
+        input_data = params.dict(by_alias=True, exclude_none=True)
+        input_data["includes"] = [
+            "ASSET_INTERFACES",
+            "SSL_PROTOCOLS",
+            "CIPHER_SUITES",
+            "EXTENSIVE_CERTIFICATE_INFO",
+        ]
+
+        raw = self.conn.post(qutils.URLS["List CertView Certificates"], input_data)
+
+        if len(raw) > 0:
+            certificates: list[Certificate] = []
+            for cert in raw:
+                c = Certificate.parse_obj(cert)
+
+                # subject.name somtimes includes null characters "\x00", even though the GUI doesn't
+                # show these.  I've opened a ticket with Qualys about it.  In the meanwhile, this
+                # will replace them with something PostgreSQL is happy with.
+                # Also other fields, apparently...
+                c.subject.name = c.subject.name.replace("\x00", "\uFFFD")
+                c.subject.locality = c.subject.locality.replace("\x00", "\uFFFD")
+                c.subject.state = c.subject.state.replace("\x00", "\uFFFD")
+
+                certificates.append(c)
+            return certificates
+        else:
+            return None
+
+    def call(
+        self,
+        params: List_CertView_Certificates_V2_Input = List_CertView_Certificates_V2_Input(),
+    ) -> list[Certificate]:
         certificates: list[Certificate] = []
 
-    raw = conn.post(qutils.URLS["List CertView Certificates"], input_data)
+        while (new_certs := self.__call_once(params)) is not None:
+            certificates.extend(new_certs)
+
+            params.page_number += 1
+
+        return certificates
+
+    def init_db(self, *, echo: bool = False) -> None:
+        engine = sa.create_engine(qutils.E_URL, echo=echo)
+
+        with engine.connect() as conn:
+            conn.execute(sa.schema.CreateSchema("certificate", if_not_exists=True))
+            conn.commit()
+
+        Base.metadata.create_all(engine)
+
+    def load(self, *, echo: bool = False) -> None:
+        params = List_CertView_Certificates_V2_Input(page_size=200)
 
-    while len(raw) > 0:
-        for cert in raw:
-            c = Certificate.parse_obj(cert)
-
-            # subject.name somtimes includes null characters "\x00", even though the GUI doesn't
-            # show these.  I've opened a ticket with Qualys about it.  In the meanwhile, this
-            # will replace them with something PostgreSQL is happy with.
-            # Also other fields, apparently...
-            c.subject.name = c.subject.name.replace("\x00", "\uFFFD")
-            c.subject.locality = c.subject.locality.replace("\x00", "\uFFFD")
-            c.subject.state = c.subject.state.replace("\x00", "\uFFFD")
+        engine = sa.create_engine(qutils.E_URL, echo=echo)
 
-            if load_db:
+        while (new_certs := self.__call_once(params)) is not None:
+            for c in new_certs:
                 with orm.Session(engine) as session:
                     obj = qutils.to_orm_object(
                         c.dict(exclude_none=True), Certificate_ORM
                     )
                     obj = session.merge(obj)
                     session.add(obj)
                     session.commit()
-            else:
-                certificates.append(c)
 
-        input_data["pageNumber"] += 1
-        raw = conn.post(
-            qutils.URLS["List CertView Certificates"],
-            input_data,
-        )
+            params.page_number += 1
 
-    if not load_db:
-        return certificates
-    else:
-        return None
+    def query(self, stmt: Any, *, echo: bool = False) -> list[Certificate]:
+        engine = sa.create_engine(qutils.E_URL, echo=echo)
 
+        certificates: list[Certificate] = []
+        with orm.Session(engine) as session:
+            results = session.scalars(stmt)
+            for result in results.all():
+                c = Certificate.from_orm(result)
+                certificates.append(c)
 
-def init_db() -> None:
-    engine = sa.create_engine(qutils.E_URL, echo=True)
+        return certificates
 
-    with engine.connect() as conn:
-        conn.execute(sa.schema.CreateSchema("certificate", if_not_exists=True))
-        conn.commit()
+    def reset(self, *, echo: bool = False) -> None:
+        engine = sa.create_engine(qutils.E_URL, echo=echo)
 
-    Base.metadata.create_all(engine)
+        stmt = sa.text("DROP SCHEMA IF EXISTS certificate CASCADE")
+        with orm.Session(engine) as session:
+            session.execute(stmt)
+            session.commit()
+        self.init_db(echo=echo)
```

### Comparing `qualyspy-0.2.1/qualyspy/certview/sql/certview_init.sql` & `qualyspy-0.2.2/qualyspy/certview/sql/certview_init.sql`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/qualyspy/scan_configuration/knowledgebase.py` & `qualyspy-0.2.2/qualyspy/scan_configuration/knowledgebase.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/.gitignore` & `qualyspy-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/LICENSE` & `qualyspy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qualyspy-0.2.1/pyproject.toml` & `qualyspy-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "QualysPy"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Jordan Barnartt", email="jbarnart@uwaterloo.ca" },
 ]
 description = "A Python wrapper for the Qualys API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -35,8 +35,10 @@
 "Bug Tracker" = "https://github.com/JordanBarnartt/qualyspy/issues"
 
 [tool.pyright]
 reportUnboundVariable = false
 reportUnknownArgumentType = false
 reportPrivateUsage = false
 reportUnknownVariableType = false
-reportUnknownMemberType = false
+reportUnknownMemberType = false
+reportGeneralTypeIssues = false
+reportUntypedBaseClass = false
```

### Comparing `qualyspy-0.2.1/PKG-INFO` & `qualyspy-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QualysPy
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python wrapper for the Qualys API.
 Project-URL: Homepage, https://github.com/JordanBarnartt/qualyspy
 Project-URL: Bug Tracker, https://github.com/JordanBarnartt/qualyspy/issues
 Author-email: Jordan Barnartt <jbarnart@uwaterloo.ca>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

