# Comparing `tmp/django-peeringdb-2.9.0.tar.gz` & `tmp/django-peeringdb-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-peeringdb-2.9.0.tar", max compression
+gzip compressed data, was "django-peeringdb-3.0.0.tar", max compression
```

## Comparing `django-peeringdb-2.9.0.tar` & `django-peeringdb-3.0.0.tar`

### file list

```diff
@@ -1,39 +1,48 @@
--rw-r--r--   0        0        0    11358 2021-09-14 07:25:23.256754 django-peeringdb-2.9.0/LICENSE.txt
--rw-r--r--   0        0        0      791 2021-09-14 07:25:23.256754 django-peeringdb-2.9.0/README.md
--rw-r--r--   0        0        0     1632 2021-09-14 07:33:04.930232 django-peeringdb-2.9.0/pyproject.toml
--rw-r--r--   0        0        0      175 2021-09-14 07:25:23.266754 django-peeringdb-2.9.0/src/django_peeringdb/__init__.py
--rw-r--r--   0        0        0      183 2021-09-14 07:25:23.270087 django-peeringdb-2.9.0/src/django_peeringdb/admin/__init__.py
--rw-r--r--   0        0        0     2505 2021-09-14 07:25:23.273420 django-peeringdb-2.9.0/src/django_peeringdb/admin/views.py
--rw-r--r--   0        0        0       70 2021-09-14 07:25:23.280087 django-peeringdb-2.9.0/src/django_peeringdb/client_adaptor/__init__.py
--rw-r--r--   0        0        0     7229 2021-09-14 07:25:23.280087 django-peeringdb-2.9.0/src/django_peeringdb/client_adaptor/backend.py
--rw-r--r--   0        0        0     1103 2021-09-14 07:25:23.280087 django-peeringdb-2.9.0/src/django_peeringdb/client_adaptor/load.py
--rw-r--r--   0        0        0      812 2021-09-14 07:25:23.283420 django-peeringdb-2.9.0/src/django_peeringdb/client_adaptor/setup.py
--rw-r--r--   0        0        0     4410 2021-09-14 07:25:23.283420 django-peeringdb-2.9.0/src/django_peeringdb/const.py
--rw-r--r--   0        0        0      806 2021-09-14 07:25:23.283420 django-peeringdb-2.9.0/src/django_peeringdb/default_settings.py
--rw-r--r--   0        0        0     2135 2021-09-14 07:25:23.283420 django-peeringdb-2.9.0/src/django_peeringdb/fields.py
--rw-r--r--   0        0        0        0 2021-09-14 07:25:23.283420 django-peeringdb-2.9.0/src/django_peeringdb/management/__init__.py
--rw-r--r--   0        0        0        0 2021-09-14 07:25:23.283420 django-peeringdb-2.9.0/src/django_peeringdb/management/commands/__init__.py
--rw-r--r--   0        0        0      662 2021-09-14 07:25:23.283420 django-peeringdb-2.9.0/src/django_peeringdb/management/commands/pdb_sync.py
--rw-r--r--   0        0        0    31572 2021-09-14 07:25:23.290087 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0001_initial.py
--rw-r--r--   0        0        0     1242 2021-09-14 07:25:23.293420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0002_network_fields_help_text.py
--rw-r--r--   0        0        0      564 2021-09-14 07:25:23.293420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0003_never_via_route_servers.py
--rw-r--r--   0        0        0      744 2021-09-14 07:25:23.293420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0004_rs_lg_fields.py
--rw-r--r--   0        0        0      921 2021-09-14 07:25:23.293420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0005_fac_contacts.py
--rw-r--r--   0        0        0      401 2021-09-14 07:25:23.293420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0006_net_operational.py
--rw-r--r--   0        0        0      366 2021-09-14 07:25:23.293420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0007_add_verbose_names.py
--rw-r--r--   0        0        0     2300 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0008_traffic_levels.py
--rw-r--r--   0        0        0      398 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0009_ixlanprefix_in_dfz.py
--rw-r--r--   0        0        0      821 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0010_ix_ixf_fields.py
--rw-r--r--   0        0        0     1090 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0011_ixlan_ixf_fields.py
--rw-r--r--   0        0        0     2157 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0012_change_network_prefixes_and_info_type.py
--rw-r--r--   0        0        0     2784 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0013_add_phone_help_text.py
--rw-r--r--   0        0        0      999 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0014_add_suite_and_floor.py
--rw-r--r--   0        0        0     2058 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0015_add_aka_longname.py
--rw-r--r--   0        0        0     1622 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0016_add_ix_service_and_terms.py
--rw-r--r--   0        0        0     2339 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/0017_facility_fields.py
--rw-r--r--   0        0        0        0 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/migrations/__init__.py
--rw-r--r--   0        0        0      260 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/models/__init__.py
--rw-r--r--   0        0        0    15161 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/models/abstract.py
--rw-r--r--   0        0        0     4302 2021-09-14 07:25:23.303420 django-peeringdb-2.9.0/src/django_peeringdb/models/concrete.py
--rw-r--r--   0        0        0     1886 2021-09-14 07:33:08.088343 django-peeringdb-2.9.0/setup.py
--rw-r--r--   0        0        0     1944 2021-09-14 07:33:08.089077 django-peeringdb-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1303 2022-10-10 13:03:11.610570 django-peeringdb-3.0.0/LICENSE.txt
+-rw-r--r--   0        0        0      831 2022-07-15 13:10:53.610434 django-peeringdb-3.0.0/README.md
+-rw-r--r--   0        0        0     1616 2023-04-11 13:16:39.413699 django-peeringdb-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2022-07-15 13:10:53.610434 django-peeringdb-3.0.0/src/django_peeringdb/__init__.py
+-rw-r--r--   0        0        0      183 2022-07-15 13:10:53.610434 django-peeringdb-3.0.0/src/django_peeringdb/admin/__init__.py
+-rw-r--r--   0        0        0     2505 2022-07-15 13:10:53.610434 django-peeringdb-3.0.0/src/django_peeringdb/admin/views.py
+-rw-r--r--   0        0        0       70 2022-07-15 13:10:53.610434 django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/__init__.py
+-rw-r--r--   0        0        0     7373 2023-03-08 12:36:10.126224 django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/backend.py
+-rw-r--r--   0        0        0     1103 2022-07-15 13:10:53.613767 django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/load.py
+-rw-r--r--   0        0        0      812 2022-07-15 13:10:53.613767 django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/setup.py
+-rw-r--r--   0        0        0    18324 2023-04-11 13:16:27.426957 django-peeringdb-3.0.0/src/django_peeringdb/const.py
+-rw-r--r--   0        0        0      806 2022-07-15 13:10:53.613767 django-peeringdb-3.0.0/src/django_peeringdb/default_settings.py
+-rw-r--r--   0        0        0     2529 2023-03-08 12:36:10.126224 django-peeringdb-3.0.0/src/django_peeringdb/fields.py
+-rw-r--r--   0        0        0        0 2022-07-15 13:10:53.613767 django-peeringdb-3.0.0/src/django_peeringdb/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-15 13:10:53.613767 django-peeringdb-3.0.0/src/django_peeringdb/management/commands/__init__.py
+-rw-r--r--   0        0        0      662 2022-07-15 13:10:53.613767 django-peeringdb-3.0.0/src/django_peeringdb/management/commands/pdb_sync.py
+-rw-r--r--   0        0        0    31571 2023-03-08 12:36:10.126224 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1241 2023-03-08 12:36:10.126224 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0002_network_fields_help_text.py
+-rw-r--r--   0        0        0      563 2023-03-08 12:36:10.126224 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0003_never_via_route_servers.py
+-rw-r--r--   0        0        0      743 2023-03-08 12:36:10.126224 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0004_rs_lg_fields.py
+-rw-r--r--   0        0        0      920 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0005_fac_contacts.py
+-rw-r--r--   0        0        0      400 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0006_net_operational.py
+-rw-r--r--   0        0        0      365 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0007_add_verbose_names.py
+-rw-r--r--   0        0        0     2298 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0008_traffic_levels.py
+-rw-r--r--   0        0        0      397 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0009_ixlanprefix_in_dfz.py
+-rw-r--r--   0        0        0      820 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0010_ix_ixf_fields.py
+-rw-r--r--   0        0        0     1089 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0011_ixlan_ixf_fields.py
+-rw-r--r--   0        0        0     2156 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0012_change_network_prefixes_and_info_type.py
+-rw-r--r--   0        0        0     2783 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0013_add_phone_help_text.py
+-rw-r--r--   0        0        0      998 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0014_add_suite_and_floor.py
+-rw-r--r--   0        0        0     2057 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0015_add_aka_longname.py
+-rw-r--r--   0        0        0     1621 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0016_add_ix_service_and_terms.py
+-rw-r--r--   0        0        0     2338 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0017_facility_fields.py
+-rw-r--r--   0        0        0      990 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0018_add_region_continent_field.py
+-rw-r--r--   0        0        0     1050 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0019_ix_add_sales_phone_email.py
+-rw-r--r--   0        0        0     1176 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0020_status_dashboard.py
+-rw-r--r--   0        0        0      720 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0021_rir_fields.py
+-rw-r--r--   0        0        0     4784 2023-03-08 12:36:10.132891 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0022_carriers.py
+-rw-r--r--   0        0        0      514 2023-03-08 12:36:10.132891 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0023_mtu.py
+-rw-r--r--   0        0        0      517 2023-03-08 12:36:10.132891 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0024_carrier_website_optional.py
+-rw-r--r--   0        0        0     3332 2023-03-08 12:36:10.132891 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0025_campus.py
+-rw-r--r--   0        0        0     1612 2023-04-11 13:16:27.426957 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0026_add_social_media.py
+-rw-r--r--   0        0        0        0 2022-07-15 13:10:53.620434 django-peeringdb-3.0.0/src/django_peeringdb/migrations/__init__.py
+-rw-r--r--   0        0        0      260 2022-07-15 13:10:53.620434 django-peeringdb-3.0.0/src/django_peeringdb/models/__init__.py
+-rw-r--r--   0        0        0    18192 2023-04-11 13:16:27.426957 django-peeringdb-3.0.0/src/django_peeringdb/models/abstract.py
+-rw-r--r--   0        0        0     5601 2023-03-08 12:36:10.132891 django-peeringdb-3.0.0/src/django_peeringdb/models/concrete.py
+-rw-r--r--   0        0        0     1942 2023-04-11 13:17:13.497629 django-peeringdb-3.0.0/setup.py
+-rw-r--r--   0        0        0     1974 2023-04-11 13:17:13.498307 django-peeringdb-3.0.0/PKG-INFO
```

### Comparing `django-peeringdb-2.9.0/README.md` & `django-peeringdb-3.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # django-peeringdb
 
 [![PyPI](https://img.shields.io/pypi/v/django_peeringdb.svg?maxAge=2592000)](https://pypi.python.org/pypi/django_peeringdb)
 [![PyPI](https://img.shields.io/pypi/pyversions/django-peeringdb.svg)](https://pypi.python.org/pypi/django-peeringdb)
-[![Tests](https://github.com/peeringdb/django-peeringdb/workflows/tests/badge.svg)](https://github.com/peeringdb/django-peeringdb)
-[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/20c/django-peeringdb)](https://lgtm.com/projects/g/20c/django-peeringdb/alerts/)
+[![Tests](https://github.com/peeringdb/django-peeringdb/workflows/tests/badge.svg)](https://github.com/peeringdb/django-peeringdb/actions/workflows/tests.yml)
+[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/peeringdb/django-peeringdb)](https://lgtm.com/projects/g/peeringdb/django-peeringdb/alerts/)
 [![Codecov](https://img.shields.io/codecov/c/github/peeringdb/django-peeringdb/master.svg?maxAge=2592000)](https://codecov.io/github/peeringdb/django-peeringdb)
 
 Django models for PeeringDB
 
 See the docs at http://peeringdb.github.io/django-peeringdb/
```

### Comparing `django-peeringdb-2.9.0/pyproject.toml` & `django-peeringdb-3.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 [tool.poetry]
 name = "django-peeringdb"
-version = "2.9.0"
+version = "3.0.0"
 description = "PeeringDB Django models"
 readme = "README.md"
 repository = "https://github.com/peeringdb/django-peeringdb"
 authors = ["PeeringDB <support@peeringdb.com>"]
 license = "Apache-2.0"
 
 classifiers = [
   "Development Status :: 5 - Production/Stable",
-  "Framework :: Django :: 2.2",
-  "Framework :: Django :: 3.0",
   "Framework :: Django :: 3.1",
   "Framework :: Django :: 3.2",
+  "Framework :: Django :: 4.0",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
-  "Programming Language :: Python :: 3.6",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Internet",
 ]
 
 packages = [{ include = "django_peeringdb", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.7"
 django_countries = ">1"
 django_handleref = "^1"
 django_inet = "^1"
+asgiref = "^3"
 
 [tool.poetry.dev-dependencies]
 # testing
-codecov = "*"
-pytest = "^6.0.1"
-pytest-django = "^3.8.0"
+codecov = ">=2"
+coverage = ">=5"
+pytest = ">=6"
+pytest-django = ">=3.8"
 pytest-cov = "*"
 tox = ">=3.24"
 
 # linting
-# bandit = "^1.6.2"
-black = { version = ">=20", allow-prereleases = true }
-isort = "^5.7.0"
-flake8 = "^3.8.4"
-mypy = "^0.812"
-pre-commit = "^2.13"
-pyupgrade = "^2.19.4"
+# bandit = ">=1.6.2"
+black = ">=20"
+isort = ">=5.7"
+flake8 = ">=3.8"
+mypy = ">=0.950"
+pre-commit = ">=2.13"
+pyupgrade = ">=2.19"
 
 # docs
 markdown = "*"
 markdown-include = ">=0.5,<1"
-mkdocs = "^1"
+mkdocs = "^1.2.3"
 
 # ctl
-ctl = "^1"
-jinja2 = "^2.11.2"
-tmpl = "^1"
+ctl = ">=1"
+jinja2 = ">=2"
+tmpl = ">=1"
+# v4 released 2022-03-31
 twine = "^3.3.0"
 
 [tool.poetry.plugins."markdown.extensions"]
 pymdgen = "pymdgen.md:Extension"
 
 [build-system]
 requires = ["poetry>=0.12"]
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/admin/views.py` & `django-peeringdb-3.0.0/src/django_peeringdb/admin/views.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/client_adaptor/backend.py` & `django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,35 +16,37 @@
 from peeringdb.backend import Interface, reftag_to_cls
 
 from django_peeringdb import __version__  # noqa
 from django_peeringdb.models import concrete
 
 
 class Backend(Interface):
-
     # Non-builtin scalar types
     CUSTOM_FIELDS = (
         Decimal,
         Country,
         IPv4Address,
         IPv6Address,
     )
 
     # Resource (abstract) and model (concrete) definitions
     RESOURCE_MAP = {
+        resource.Carrier: concrete.Carrier,
+        resource.CarrierFacility: concrete.CarrierFacility,
         resource.Facility: concrete.Facility,
         resource.InternetExchange: concrete.InternetExchange,
         resource.InternetExchangeFacility: concrete.InternetExchangeFacility,
         resource.InternetExchangeLan: concrete.IXLan,
         resource.InternetExchangeLanPrefix: concrete.IXLanPrefix,
         resource.Network: concrete.Network,
         resource.NetworkContact: concrete.NetworkContact,
         resource.NetworkFacility: concrete.NetworkFacility,
         resource.NetworkIXLan: concrete.NetworkIXLan,
         resource.Organization: concrete.Organization,
+        resource.Campus: concrete.Campus,
     }
 
     ERROR_PATTERNS = {
         "mysql": {
             "unique": [(r"Duplicate entry '[^\']+' for key '(?P<field_name>\w+)'", 1)],
         },
         "sqlite": {
@@ -179,15 +181,14 @@
 
         for name, err in list(exc.error_dict.items()):
             if re.search(pattern, str(err)):
                 fields.append(name)
         return fields or None
 
     def _detect_integrity_error(self, exc):
-
         engine = connection.vendor
         patterns = self.ERROR_PATTERNS[engine]
 
         assert isinstance(exc, IntegrityError)
         # for name, err in exc.error_dict.items():
         for pattern, index in patterns.get("unique"):
             m = re.search(pattern, str(exc.args[index]))
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/client_adaptor/load.py` & `django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/load.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/client_adaptor/setup.py` & `django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/setup.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/default_settings.py` & `django-peeringdb-3.0.0/src/django_peeringdb/default_settings.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/fields.py` & `django-peeringdb-3.0.0/src/django_peeringdb/fields.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,16 +10,18 @@
     Field that can take a set of string values
     and store them in a charfield using a delimiter
 
     This needs to be compatible with django-rest-framework's
     multiple choice field.
     """
 
-    def clean_choices(self, values):
+    def cleaned_values(self, values):
+        return [value.strip("{}' ") for value in values]
 
+    def clean_choices(self, values):
         for value in values:
             exists = False
             for choice, label in self.choices:
                 if choice == value:
                     exists = True
                     break
 
@@ -27,57 +29,63 @@
                 raise ValidationError(_("Invalid value: {}").format(value))
 
     def validate(self, value, model_instance):
         if not self.editable:
             # Skip validation for non-editable fields.
             return
 
-        self.clean_choices(value)
+        self.clean_choices(self.cleaned_values(value))
 
         if value is None and not self.null:
             raise ValidationError(self.error_messages["null"], code="null")
 
         if not self.blank and value in self.empty_values:
             raise ValidationError(self.error_messages["blank"], code="blank")
 
     def from_db_value(self, value, expression, connection):
-
         if value is None:
             return None
 
-        if not value:
+        if not value or value == "[]":
             return []
 
-        values = value.split(",")
+        values = self.cleaned_values(value.split(","))
 
         self.clean_choices(values)
 
         return values
 
     def get_prep_value(self, value):
-
         if value is None:
             return ""
 
         picked = []
         for choice, label in self.choices:
             if choice in value:
                 picked.append(choice)
+
         return ",".join(picked)
 
     def to_python(self, value):
         if isinstance(value, (list, set, tuple)):
             return value
 
         if value is None:
             return value
 
-        values = value.split(",")
+        if value == "[]":
+            return None
 
+        values = self.cleaned_values(value.split(","))
         self.clean_choices(values)
 
         return values
 
     def formfield(self, **kwargs):
         defaults = {"form_class": django.forms.MultipleChoiceField}
         defaults.update(**kwargs)
         return super().formfield(**defaults)
+
+    def value_to_string(self, obj):
+        values = self.value_from_object(obj)
+        self.clean_choices(self.cleaned_values(values))
+        return ",".join(values)
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/management/commands/pdb_sync.py` & `django-peeringdb-3.0.0/src/django_peeringdb/management/commands/pdb_sync.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0001_initial.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import django_inet.models
 from django.db import migrations, models
 
 import django_peeringdb.models.abstract
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="Facility",
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0002_network_fields_help_text.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0002_network_fields_help_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 1.11.23 on 2019-12-09 09:06
 
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("django_peeringdb", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="network",
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0003_never_via_route_servers.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0003_never_via_route_servers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 1.11.23 on 2019-12-10 12:12
 
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("django_peeringdb", "0002_network_fields_help_text"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="network",
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0004_rs_lg_fields.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0004_rs_lg_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from django.db import migrations
 
 import django_peeringdb.models.abstract
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("django_peeringdb", "0003_never_via_route_servers"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="network",
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0005_fac_contacts.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0005_fac_contacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 2.2.12 on 2020-04-03 20:42
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("django_peeringdb", "0004_rs_lg_fields"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="facility",
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0008_traffic_levels.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0008_traffic_levels.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from django.db import migrations, models
 
 
 def adjust_traffic_levels(apps, schema_editor):
     Network = apps.get_model("django_peeringdb", "Network")
 
     for net in Network.handleref.all():
-
         # only save networks that actually had to have their value
         # adjusted
 
         save = False
 
         # remove spaces
 
@@ -34,15 +33,14 @@
             save = True
 
         if save:
             net.save()
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("django_peeringdb", "0007_add_verbose_names"),
     ]
 
     operations = [
         migrations.RunPython(adjust_traffic_levels),
         migrations.AlterField(
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0010_ix_ixf_fields.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0010_ix_ixf_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import django_inet.models
 from django.db import migrations, models
 
 import django_peeringdb.models.abstract
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("django_peeringdb", "0009_ixlanprefix_in_dfz"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="internetexchange",
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0011_ixlan_ixf_fields.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0011_ixlan_ixf_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import django_inet.models
 from django.db import migrations, models
 
 import django_peeringdb.models.abstract
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("django_peeringdb", "0010_ix_ixf_fields"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="ixlan",
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0012_change_network_prefixes_and_info_type.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0012_change_network_prefixes_and_info_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import django_inet.models
 from django.db import migrations, models
 
 import django_peeringdb.models.abstract
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("django_peeringdb", "0011_ixlan_ixf_fields"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="network",
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0013_add_phone_help_text.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0013_add_phone_help_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.1.2 on 2020-11-17 23:48
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("django_peeringdb", "0012_change_network_prefixes_and_info_type"),
     ]
 
     operations = [
         migrations.AlterField(
             model_name="networkcontact",
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0014_add_suite_and_floor.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0014_add_suite_and_floor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.1.2 on 2020-11-23 21:01
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("django_peeringdb", "0013_add_phone_help_text"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="facility",
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0015_add_aka_longname.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0015_add_aka_longname.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.1.2 on 2021-03-05 18:12
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("django_peeringdb", "0014_add_suite_and_floor"),
     ]
 
     operations = [
         # Facilities need "name_long" and "aka"
         migrations.AddField(
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0016_add_ix_service_and_terms.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0016_add_ix_service_and_terms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.1.2 on 2021-04-13 18:58
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("django_peeringdb", "0015_add_aka_longname"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="internetexchange",
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/migrations/0017_facility_fields.py` & `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0017_facility_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from django.db import migrations, models
 
 import django_peeringdb.fields
 import django_peeringdb.models.abstract
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("django_peeringdb", "0016_add_ix_service_and_terms"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="facility",
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/models/abstract.py` & `django-peeringdb-3.0.0/src/django_peeringdb/models/abstract.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 class OrganizationBase(HandleRefModel, AddressModel):
     name = models.CharField(_("Name"), max_length=255, unique=True)
 
     aka = models.CharField(_("Also Known As"), max_length=255, blank=True)
     name_long = models.CharField(_("Long Name"), max_length=255, blank=True)
 
     website = URLField(_("Website"), blank=True)
+    social_media = models.JSONField(_("Social Media"), default=dict, blank=True)
     notes = models.TextField(_("Notes"), blank=True)
 
     class Meta:
         abstract = True
         db_table = "%sorganization" % settings.TABLE_PREFIX
         verbose_name = _("Organization")
         verbose_name_plural = _("Organizations")
@@ -77,14 +78,15 @@
     def __str__(self):
         return self.name
 
 
 class FacilityBase(HandleRefModel, AddressModel):
     name = models.CharField(_("Name"), max_length=255, unique=True)
     website = URLField(_("Website"), blank=True)
+    social_media = models.JSONField(_("Social Media"), default=dict, blank=True)
 
     aka = models.CharField(_("Also Known As"), max_length=255, blank=True)
     name_long = models.CharField(_("Long Name"), max_length=255, blank=True)
 
     clli = models.CharField(_("CLLI Code"), max_length=18, blank=True)
     rencode = models.CharField(_("Rencode"), max_length=18, blank=True)
     npanxx = models.CharField(_("NPA-NXX"), max_length=21, blank=True)
@@ -130,14 +132,24 @@
         help_text=_(
             "The alternating current voltage available to users of the facility either directly from the landlord or delivered by the utility separately."
         ),
     )
 
     notes = models.TextField(_("Notes"), blank=True)
 
+    region_continent = models.CharField(
+        _("Continental Region"),
+        max_length=255,
+        choices=const.REGIONS,
+        blank=True,
+        null=True,
+    )
+
+    status_dashboard = URLField(_("Status Dashboard"), null=True, blank=True)
+
     class Meta:
         abstract = True
         db_table = "%sfacility" % settings.TABLE_PREFIX
         verbose_name = _("Facility")
         verbose_name_plural = _("Facilities")
 
     class HandleRef:
@@ -187,14 +199,15 @@
         help_text=_(
             "Reference to an AS-SET or "
             "ROUTE-SET in Internet "
             "Routing Registry (IRR)"
         ),
     )
     website = URLField(_("Website"), blank=True)
+    social_media = models.JSONField(_("Social Media"), default=dict, blank=True)
     looking_glass = LG_URLField(_("Looking Glass URL"), blank=True)
     route_server = LG_URLField(_("Route Server URL"), blank=True)
 
     notes = models.TextField(_("Notes"), blank=True)
     notes_private = models.TextField(_("Private notes"), blank=True)
 
     info_traffic = models.CharField(
@@ -268,14 +281,26 @@
     policy_contracts = models.CharField(
         _("Contract Requirement"),
         max_length=36,
         blank=True,
         choices=const.POLICY_CONTRACTS,
     )
 
+    status_dashboard = URLField(_("Status Dashboard"), null=True, blank=True)
+
+    rir_status = models.CharField(
+        _("RIR status"),
+        null=True,
+        default=None,
+        max_length=255,
+    )
+    rir_status_updated = models.DateTimeField(
+        _("RIR status updated"), blank=True, null=True
+    )
+
     class Meta:
         abstract = True
         db_table = "%snetwork" % settings.TABLE_PREFIX
         verbose_name = _("Network")
         verbose_name_plural = _("Networks")
 
     class HandleRef:
@@ -302,28 +327,34 @@
     )
     media = models.CharField(_("Media Type"), max_length=128, choices=const.MEDIA)
     proto_unicast = models.BooleanField(_("Unicast IPv4"), default=False)
     proto_multicast = models.BooleanField(_("Multicast"), default=False)
     proto_ipv6 = models.BooleanField(_("Unicast IPv6"), default=False)
 
     website = URLField(_("Company Website"), blank=True)
+    social_media = models.JSONField(_("Social Media"), default=dict, blank=True)
     url_stats = URLField(_("Traffic Stats Website"), blank=True)
 
     tech_email = models.EmailField(_("Technical Email"), max_length=254, blank=True)
     tech_phone = models.CharField(
         _("Technical Phone"),
         max_length=192,
         blank=True,
         help_text=const.PHONE_HELP_TEXT,
     )
     policy_email = models.EmailField(_("Policy Email"), max_length=254, blank=True)
     policy_phone = models.CharField(
         _("Policy Phone"), max_length=192, blank=True, help_text=const.PHONE_HELP_TEXT
     )
 
+    sales_email = models.EmailField(_("Sales Email"), max_length=254, blank=True)
+    sales_phone = models.CharField(
+        _("Sales Phone"), max_length=192, blank=True, help_text=const.PHONE_HELP_TEXT
+    )
+
     ixf_net_count = models.IntegerField(_("IX-F Network Count"), default=0)
     ixf_last_import = models.DateTimeField(_("IX-F Last Import"), null=True, blank=True)
 
     service_level = models.CharField(
         _("Service Level"),
         max_length=60,
         blank=True,
@@ -335,14 +366,16 @@
         _("Terms"),
         max_length=60,
         blank=True,
         choices=const.TERMS_TYPES,
         default="Not Disclosed",
     )
 
+    status_dashboard = URLField(_("Status Dashboard"), null=True, blank=True)
+
     class Meta:
         abstract = True
         db_table = "%six" % settings.TABLE_PREFIX
         verbose_name = _("Internet Exchange")
         verbose_name_plural = _("Internet Exchanges")
 
     class HandleRef:
@@ -363,15 +396,15 @@
     class HandleRef:
         tag = "ixfac"
 
 
 class IXLanBase(HandleRefModel):
     name = models.CharField(_("Name"), max_length=255, blank=True)
     descr = models.TextField(_("Description"), blank=True)
-    mtu = models.PositiveIntegerField("MTU", null=True, blank=True)
+    mtu = models.PositiveIntegerField("MTU", default=1500, choices=const.MTUS)
     vlan = models.PositiveIntegerField("VLAN", null=True, blank=True)
     dot1q_support = models.BooleanField("802.1Q", default=False)
     rs_asn = ASNField(
         verbose_name=_("Route Server ASN"), null=True, blank=True, default=0
     )
     arp_sponge = MacAddressField(
         verbose_name=_("ARP sponging MAC"), null=True, unique=True, blank=True
@@ -443,7 +476,65 @@
         abstract = True
         db_table = "%snetwork_ixlan" % settings.TABLE_PREFIX
         verbose_name = _("Public Peering Exchange Point")
         verbose_name_plural = _("Public Peering Exchange Points")
 
     class HandleRef:
         tag = "netixlan"
+
+
+class CarrierBase(HandleRefModel):
+    name = models.CharField(_("Name"), max_length=255, unique=True)
+
+    aka = models.CharField(_("Also Known As"), max_length=255, blank=True)
+    name_long = models.CharField(_("Long Name"), max_length=255, blank=True)
+
+    website = URLField(_("Website"), blank=True, null=True)
+    social_media = models.JSONField(_("Social Media"), default=dict, blank=True)
+    notes = models.TextField(_("Notes"), blank=True)
+
+    class Meta:
+        abstract = True
+        db_table = f"{settings.TABLE_PREFIX}carrier"
+        verbose_name = _("Carrier")
+        verbose_name_plural = _("Carriers")
+
+    class HandleRef:
+        tag = "carrier"
+        delete_cascade = ["carrierfac_set"]
+
+    def __str__(self):
+        return self.name
+
+
+class CarrierFacilityBase(HandleRefModel):
+    class Meta:
+        abstract = True
+        db_table = f"{settings.TABLE_PREFIX}carrier_facility"
+        verbose_name = _("Carrier presence at facility")
+        verbose_name_plural = _("Carrier presences at facility")
+
+    class HandleRef:
+        tag = "carrierfac"
+
+
+class CampusBase(HandleRefModel):
+    name = models.CharField(_("Campus Name"), max_length=255, unique=True)
+
+    name_long = models.CharField(_("Long Name"), max_length=255, blank=True, null=True)
+    aka = models.CharField(_("Also Known As"), max_length=255, blank=True, null=True)
+
+    website = URLField(_("Website"), blank=True, null=True)
+    social_media = models.JSONField(_("Social Media"), default=dict, blank=True)
+    notes = models.TextField(_("Notes"), blank=True)
+
+    class Meta:
+        abstract = True
+        db_table = "%scampus" % settings.TABLE_PREFIX
+        verbose_name = _("Campus")
+        verbose_name_plural = _("Campuses")
+
+    class HandleRef:
+        tag = "campus"
+
+    def __str__(self):
+        return self.name
```

### Comparing `django-peeringdb-2.9.0/src/django_peeringdb/models/concrete.py` & `django-peeringdb-3.0.0/src/django_peeringdb/models/concrete.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from django.conf import settings
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from django_peeringdb.models import (
+    CampusBase,
+    CarrierBase,
+    CarrierFacilityBase,
     ContactBase,
     FacilityBase,
     InternetExchangeBase,
     InternetExchangeFacilityBase,
     IXLanBase,
     IXLanPrefixBase,
     NetworkBase,
@@ -37,21 +40,39 @@
 
 @expose_model
 class Organization(OrganizationBase):
     pass
 
 
 @expose_model
+class Campus(CampusBase):
+    org = models.ForeignKey(
+        Organization,
+        related_name="campus_set",
+        verbose_name=_("Organization"),
+        on_delete=models.CASCADE,
+    )
+
+
+@expose_model
 class Facility(FacilityBase):
     org = models.ForeignKey(
         Organization,
         related_name="fac_set",
         verbose_name=_("Organization"),
         on_delete=models.CASCADE,
     )
+    campus = models.ForeignKey(
+        Campus,
+        related_name="fac_set",
+        verbose_name=_("Campus"),
+        on_delete=models.CASCADE,
+        null=True,
+        blank=True,
+    )
 
 
 @expose_model
 class Network(NetworkBase):
     org = models.ForeignKey(
         Organization,
         related_name="net_set",
@@ -71,14 +92,48 @@
 
     @property
     def fac_set(self):
         return [ixfac.fac for ixfac in self.ixfac_set]
 
 
 @expose_model
+class Carrier(CarrierBase):
+    org = models.ForeignKey(
+        Organization,
+        related_name="carrier_set",
+        verbose_name=_("Organization"),
+        on_delete=models.CASCADE,
+    )
+
+
+@expose_model
+class CarrierFacility(CarrierFacilityBase):
+    carrier = models.ForeignKey(
+        Carrier,
+        related_name="carrierfac_set",
+        verbose_name=_("Carrier"),
+        on_delete=models.CASCADE,
+    )
+    fac = models.ForeignKey(
+        Facility,
+        default=0,
+        related_name="carrierfac_set",
+        verbose_name=_("Facility"),
+        on_delete=models.CASCADE,
+    )
+
+    class Meta(CarrierFacilityBase.Meta):
+        unique_together = ("carrier", "fac")
+        db_table = "%six_carrier_facility" % settings.TABLE_PREFIX
+
+    def __str__(self):
+        return f"{self.carrier} @ {self.fac}"
+
+
+@expose_model
 class InternetExchangeFacility(InternetExchangeFacilityBase):
     ix = models.ForeignKey(
         InternetExchange,
         related_name="ixfac_set",
         verbose_name=_("Internet Exchange"),
         on_delete=models.CASCADE,
     )
```

### Comparing `django-peeringdb-2.9.0/setup.py` & `django-peeringdb-3.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,32 +13,35 @@
  'django_peeringdb.migrations',
  'django_peeringdb.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['django_countries>1', 'django_handleref>=1,<2', 'django_inet>=1,<2']
+['asgiref>=3,<4',
+ 'django_countries>1',
+ 'django_handleref>=1,<2',
+ 'django_inet>=1,<2']
 
 entry_points = \
 {'markdown.extensions': ['pymdgen = pymdgen.md:Extension']}
 
 setup_kwargs = {
     'name': 'django-peeringdb',
-    'version': '2.9.0',
+    'version': '3.0.0',
     'description': 'PeeringDB Django models',
-    'long_description': '\n# django-peeringdb\n\n[![PyPI](https://img.shields.io/pypi/v/django_peeringdb.svg?maxAge=2592000)](https://pypi.python.org/pypi/django_peeringdb)\n[![PyPI](https://img.shields.io/pypi/pyversions/django-peeringdb.svg)](https://pypi.python.org/pypi/django-peeringdb)\n[![Tests](https://github.com/peeringdb/django-peeringdb/workflows/tests/badge.svg)](https://github.com/peeringdb/django-peeringdb)\n[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/20c/django-peeringdb)](https://lgtm.com/projects/g/20c/django-peeringdb/alerts/)\n[![Codecov](https://img.shields.io/codecov/c/github/peeringdb/django-peeringdb/master.svg?maxAge=2592000)](https://codecov.io/github/peeringdb/django-peeringdb)\n\nDjango models for PeeringDB\n\nSee the docs at http://peeringdb.github.io/django-peeringdb/\n\n',
+    'long_description': '\n# django-peeringdb\n\n[![PyPI](https://img.shields.io/pypi/v/django_peeringdb.svg?maxAge=2592000)](https://pypi.python.org/pypi/django_peeringdb)\n[![PyPI](https://img.shields.io/pypi/pyversions/django-peeringdb.svg)](https://pypi.python.org/pypi/django-peeringdb)\n[![Tests](https://github.com/peeringdb/django-peeringdb/workflows/tests/badge.svg)](https://github.com/peeringdb/django-peeringdb/actions/workflows/tests.yml)\n[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/peeringdb/django-peeringdb)](https://lgtm.com/projects/g/peeringdb/django-peeringdb/alerts/)\n[![Codecov](https://img.shields.io/codecov/c/github/peeringdb/django-peeringdb/master.svg?maxAge=2592000)](https://codecov.io/github/peeringdb/django-peeringdb)\n\nDjango models for PeeringDB\n\nSee the docs at http://peeringdb.github.io/django-peeringdb/\n\n',
     'author': 'PeeringDB',
     'author_email': 'support@peeringdb.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/peeringdb/django-peeringdb',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.6.2,<4.0.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `django-peeringdb-2.9.0/PKG-INFO` & `django-peeringdb-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: django-peeringdb
-Version: 2.9.0
+Version: 3.0.0
 Summary: PeeringDB Django models
 Home-page: https://github.com/peeringdb/django-peeringdb
 License: Apache-2.0
 Author: PeeringDB
 Author-email: support@peeringdb.com
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: asgiref (>=3,<4)
 Requires-Dist: django_countries (>1)
 Requires-Dist: django_handleref (>=1,<2)
 Requires-Dist: django_inet (>=1,<2)
 Project-URL: Repository, https://github.com/peeringdb/django-peeringdb
 Description-Content-Type: text/markdown
 
 
 # django-peeringdb
 
 [![PyPI](https://img.shields.io/pypi/v/django_peeringdb.svg?maxAge=2592000)](https://pypi.python.org/pypi/django_peeringdb)
 [![PyPI](https://img.shields.io/pypi/pyversions/django-peeringdb.svg)](https://pypi.python.org/pypi/django-peeringdb)
-[![Tests](https://github.com/peeringdb/django-peeringdb/workflows/tests/badge.svg)](https://github.com/peeringdb/django-peeringdb)
-[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/20c/django-peeringdb)](https://lgtm.com/projects/g/20c/django-peeringdb/alerts/)
+[![Tests](https://github.com/peeringdb/django-peeringdb/workflows/tests/badge.svg)](https://github.com/peeringdb/django-peeringdb/actions/workflows/tests.yml)
+[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/peeringdb/django-peeringdb)](https://lgtm.com/projects/g/peeringdb/django-peeringdb/alerts/)
 [![Codecov](https://img.shields.io/codecov/c/github/peeringdb/django-peeringdb/master.svg?maxAge=2592000)](https://codecov.io/github/peeringdb/django-peeringdb)
 
 Django models for PeeringDB
 
 See the docs at http://peeringdb.github.io/django-peeringdb/
```

