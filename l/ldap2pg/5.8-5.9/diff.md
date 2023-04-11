# Comparing `tmp/ldap2pg-5.8.tar.gz` & `tmp/ldap2pg-5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldap2pg-5.8.tar", last modified: Fri Jun 10 09:40:36 2022, max compression
+gzip compressed data, was "ldap2pg-5.9.tar", last modified: Tue Apr 11 12:04:31 2023, max compression
```

## Comparing `ldap2pg-5.8.tar` & `ldap2pg-5.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 bersace   (1000) bersace   (1000)        0 2022-06-10 09:40:36.897594 ldap2pg-5.8/
--rw-r--r--   0 bersace   (1000) bersace   (1000)     2665 2019-11-06 12:49:08.000000 ldap2pg-5.8/AUTHORS.md
--rw-r--r--   0 bersace   (1000) bersace   (1000)      918 2019-01-11 09:52:04.000000 ldap2pg-5.8/LICENSE
--rw-r--r--   0 bersace   (1000) bersace   (1000)     5062 2022-06-10 09:40:36.897594 ldap2pg-5.8/PKG-INFO
--rw-r--r--   0 bersace   (1000) bersace   (1000)     4334 2022-06-10 09:38:43.000000 ldap2pg-5.8/README.rst
-drwxr-xr-x   0 bersace   (1000) bersace   (1000)        0 2022-06-10 09:40:36.897594 ldap2pg-5.8/ldap2pg/
--rw-r--r--   0 bersace   (1000) bersace   (1000)      189 2022-05-04 13:27:19.000000 ldap2pg-5.8/ldap2pg/__init__.py
--rw-r--r--   0 bersace   (1000) bersace   (1000)    23989 2022-06-10 09:38:43.000000 ldap2pg-5.8/ldap2pg/config.py
--rw-r--r--   0 bersace   (1000) bersace   (1000)    12876 2022-06-10 09:38:43.000000 ldap2pg-5.8/ldap2pg/defaults.py
--rw-r--r--   0 bersace   (1000) bersace   (1000)     9579 2022-05-04 13:27:19.000000 ldap2pg-5.8/ldap2pg/format.py
--rw-r--r--   0 bersace   (1000) bersace   (1000)    12336 2022-06-10 09:38:43.000000 ldap2pg-5.8/ldap2pg/inspector.py
--rw-r--r--   0 bersace   (1000) bersace   (1000)    14808 2022-06-10 09:38:43.000000 ldap2pg-5.8/ldap2pg/ldap.py
--rw-r--r--   0 bersace   (1000) bersace   (1000)    12637 2022-06-10 09:38:43.000000 ldap2pg-5.8/ldap2pg/manager.py
--rw-r--r--   0 bersace   (1000) bersace   (1000)    11266 2022-06-10 09:38:43.000000 ldap2pg-5.8/ldap2pg/privilege.py
--rw-r--r--   0 bersace   (1000) bersace   (1000)     8354 2022-06-10 09:38:43.000000 ldap2pg-5.8/ldap2pg/psql.py
--rw-r--r--   0 bersace   (1000) bersace   (1000)    19312 2022-06-10 09:38:43.000000 ldap2pg-5.8/ldap2pg/role.py
--rw-r--r--   0 bersace   (1000) bersace   (1000)     4878 2022-06-10 09:38:43.000000 ldap2pg-5.8/ldap2pg/script.py
--rw-r--r--   0 bersace   (1000) bersace   (1000)     5010 2021-06-21 14:40:26.000000 ldap2pg-5.8/ldap2pg/utils.py
--rw-r--r--   0 bersace   (1000) bersace   (1000)    11069 2022-06-10 09:38:43.000000 ldap2pg-5.8/ldap2pg/validators.py
-drwxr-xr-x   0 bersace   (1000) bersace   (1000)        0 2022-06-10 09:40:36.897594 ldap2pg-5.8/ldap2pg.egg-info/
--rw-r--r--   0 bersace   (1000) bersace   (1000)     5062 2022-06-10 09:40:36.000000 ldap2pg-5.8/ldap2pg.egg-info/PKG-INFO
--rw-r--r--   0 bersace   (1000) bersace   (1000)      478 2022-06-10 09:40:36.000000 ldap2pg-5.8/ldap2pg.egg-info/SOURCES.txt
--rw-r--r--   0 bersace   (1000) bersace   (1000)        1 2022-06-10 09:40:36.000000 ldap2pg-5.8/ldap2pg.egg-info/dependency_links.txt
--rw-r--r--   0 bersace   (1000) bersace   (1000)       48 2022-06-10 09:40:36.000000 ldap2pg-5.8/ldap2pg.egg-info/entry_points.txt
--rw-r--r--   0 bersace   (1000) bersace   (1000)       19 2022-06-10 09:40:36.000000 ldap2pg-5.8/ldap2pg.egg-info/requires.txt
--rw-r--r--   0 bersace   (1000) bersace   (1000)        8 2022-06-10 09:40:36.000000 ldap2pg-5.8/ldap2pg.egg-info/top_level.txt
--rw-r--r--   0 bersace   (1000) bersace   (1000)      446 2022-06-10 09:40:36.897594 ldap2pg-5.8/setup.cfg
--rw-r--r--   0 bersace   (1000) bersace   (1000)      877 2022-06-10 09:40:06.000000 ldap2pg-5.8/setup.py
+drwxr-xr-x   0 bersace   (1000) bersace   (1000)        0 2023-04-11 12:04:31.006887 ldap2pg-5.9/
+-rw-r--r--   0 bersace   (1000) bersace   (1000)     2665 2019-11-06 12:49:08.000000 ldap2pg-5.9/AUTHORS.md
+-rw-r--r--   0 bersace   (1000) bersace   (1000)      918 2019-01-11 09:52:04.000000 ldap2pg-5.9/LICENSE
+-rw-r--r--   0 bersace   (1000) bersace   (1000)     5062 2023-04-11 12:04:31.006887 ldap2pg-5.9/PKG-INFO
+-rw-r--r--   0 bersace   (1000) bersace   (1000)     4334 2022-06-10 09:38:43.000000 ldap2pg-5.9/README.rst
+drwxr-xr-x   0 bersace   (1000) bersace   (1000)        0 2023-04-11 12:04:31.006887 ldap2pg-5.9/ldap2pg/
+-rw-r--r--   0 bersace   (1000) bersace   (1000)      189 2022-05-04 13:27:19.000000 ldap2pg-5.9/ldap2pg/__init__.py
+-rw-r--r--   0 bersace   (1000) bersace   (1000)    24223 2023-04-04 13:37:10.000000 ldap2pg-5.9/ldap2pg/config.py
+-rw-r--r--   0 bersace   (1000) bersace   (1000)    12880 2022-12-05 12:41:01.000000 ldap2pg-5.9/ldap2pg/defaults.py
+-rw-r--r--   0 bersace   (1000) bersace   (1000)     9579 2022-05-04 13:27:19.000000 ldap2pg-5.9/ldap2pg/format.py
+-rw-r--r--   0 bersace   (1000) bersace   (1000)    12336 2022-06-10 09:38:43.000000 ldap2pg-5.9/ldap2pg/inspector.py
+-rw-r--r--   0 bersace   (1000) bersace   (1000)    14809 2023-04-11 12:01:27.000000 ldap2pg-5.9/ldap2pg/ldap.py
+-rw-r--r--   0 bersace   (1000) bersace   (1000)    12701 2023-04-04 13:37:10.000000 ldap2pg-5.9/ldap2pg/manager.py
+-rw-r--r--   0 bersace   (1000) bersace   (1000)    11266 2022-06-10 09:38:43.000000 ldap2pg-5.9/ldap2pg/privilege.py
+-rw-r--r--   0 bersace   (1000) bersace   (1000)     8354 2022-06-10 09:38:43.000000 ldap2pg-5.9/ldap2pg/psql.py
+-rw-r--r--   0 bersace   (1000) bersace   (1000)    19622 2023-04-04 13:37:10.000000 ldap2pg-5.9/ldap2pg/role.py
+-rw-r--r--   0 bersace   (1000) bersace   (1000)     4884 2023-04-04 13:37:10.000000 ldap2pg-5.9/ldap2pg/script.py
+-rw-r--r--   0 bersace   (1000) bersace   (1000)     5010 2021-06-21 14:40:26.000000 ldap2pg-5.9/ldap2pg/utils.py
+-rw-r--r--   0 bersace   (1000) bersace   (1000)    11069 2022-06-10 09:38:43.000000 ldap2pg-5.9/ldap2pg/validators.py
+drwxr-xr-x   0 bersace   (1000) bersace   (1000)        0 2023-04-11 12:04:31.006887 ldap2pg-5.9/ldap2pg.egg-info/
+-rw-r--r--   0 bersace   (1000) bersace   (1000)     5062 2023-04-11 12:04:30.000000 ldap2pg-5.9/ldap2pg.egg-info/PKG-INFO
+-rw-r--r--   0 bersace   (1000) bersace   (1000)      478 2023-04-11 12:04:30.000000 ldap2pg-5.9/ldap2pg.egg-info/SOURCES.txt
+-rw-r--r--   0 bersace   (1000) bersace   (1000)        1 2023-04-11 12:04:30.000000 ldap2pg-5.9/ldap2pg.egg-info/dependency_links.txt
+-rw-r--r--   0 bersace   (1000) bersace   (1000)       48 2023-04-11 12:04:30.000000 ldap2pg-5.9/ldap2pg.egg-info/entry_points.txt
+-rw-r--r--   0 bersace   (1000) bersace   (1000)       19 2023-04-11 12:04:30.000000 ldap2pg-5.9/ldap2pg.egg-info/requires.txt
+-rw-r--r--   0 bersace   (1000) bersace   (1000)        8 2023-04-11 12:04:30.000000 ldap2pg-5.9/ldap2pg.egg-info/top_level.txt
+-rw-r--r--   0 bersace   (1000) bersace   (1000)      446 2023-04-11 12:04:31.010887 ldap2pg-5.9/setup.cfg
+-rw-r--r--   0 bersace   (1000) bersace   (1000)      877 2023-04-11 12:03:22.000000 ldap2pg-5.9/setup.py
```

### Comparing `ldap2pg-5.8/AUTHORS.md` & `ldap2pg-5.9/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `ldap2pg-5.8/LICENSE` & `ldap2pg-5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ldap2pg-5.8/PKG-INFO` & `ldap2pg-5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldap2pg
-Version: 5.8
+Version: 5.9
 Summary: Manage PostgreSQL roles and privileges from YAML or LDAP
 Home-page: https://labs.dalibo.com/ldap2pg
 Author: Dalibo
 Author-email: contact@dalibo.com
 License: PostgreSQL
 Project-URL: Documentation, https://ldap2pg.rtfd.io/
 Project-URL: Tracker, https://github.com/dalibo/ldap2pg/issues
```

### Comparing `ldap2pg-5.8/README.rst` & `ldap2pg-5.9/README.rst`

 * *Files identical despite different names*

### Comparing `ldap2pg-5.8/ldap2pg/config.py` & `ldap2pg-5.9/ldap2pg/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import re
 import sys
 
 import ldap
 import psycopg2
 import yaml
 from pkg_resources import get_distribution
+from datetime import datetime
 
 from .privilege import Privilege
 from .privilege import process_definitions as process_privileges
 from .psql import libpq_version
 from .utils import (
     deepget,
     deepset,
@@ -303,15 +304,16 @@
                 value = callable_(*args)
                 break
             except (AttributeError, KeyError):
                 continue
         else:
             value = default
 
-        return self.processor(value)
+        if value is not None:
+            return self.processor(value)
 
 
 class ConfigurationError(UserError):
     def __init__(self, message):
         super(ConfigurationError, self).__init__(
             message, exit_code=os.EX_CONFIG,
         )
@@ -427,15 +429,15 @@
         Mapping('ldap:uri', env=None),
         Mapping('ldap:host', env=None),
         Mapping('ldap:port', env=None),
         Mapping('ldap:starttls', env=None),
         Mapping('ldap:sasl_mech', env=None),
         Mapping('ldap:binddn', env=None),
         Mapping('ldap:user', env=None),
-        Mapping('ldap:password', secret=True, env=None),
+        Mapping('ldap:password', secret=True, env=None, processor=str),
         Mapping('ldap:referrals', env=None),
         Mapping(
             'postgres:dsn', env='PGDSN',
             secret=r'(?:password=|:[^/][^/].*@)',
         ),
         Mapping('postgres:databases_query', env=None),
         Mapping('postgres:fallback_owner', env=None),
@@ -534,15 +536,16 @@
         # and compute verbosity from cumulated args.
         args.verbosity[0] = V.VERBOSITIES.index(self['verbosity'])
         self['verbosity'] = V.verbosity(args.verbosity)
         if hasattr(args, 'color'):
             self['color'] = args.color
         dictConfig(self.logging_dict())
 
-        logger.info("Starting ldap2pg %s.", __version__)
+        logger.info("Starting ldap2pg %s at %s.", __version__,
+                    datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
 
         # File loading.
         filename, mode = self.find_filename(os.environ, args)
         if filename == '-':
             logger.info("Reading configuration from stdin.")
             file_config = self.read(sys.stdin, 'stdin', mode)
         else:
@@ -632,19 +635,21 @@
     def logging_dict(self):
         formatter = 'verbose' if self['verbosity'] == 'DEBUG' else 'info'
         return {
             'version': 1,
             'formatters': {
                 'info': {
                     '()': __name__ + '.MultilineFormatter',
-                    'format': '%(message)s',
+                    'format':
+                        '%(asctime)s %(levelname)s:  %(message)s',
                 },
                 'verbose': {
                     '()': __name__ + '.MultilineFormatter',
-                    'format': '[%(name)-20s %(levelname)5.5s] %(message)s',
+                    'format':
+                        '%(asctime)s %(levelname)s:  %(name)s: %(message)s',
                 },
             },
             'handlers': {
                 'raw': {
                     '()': 'logging.StreamHandler',
                     'formatter': formatter,
                 },
```

### Comparing `ldap2pg-5.8/ldap2pg/defaults.py` & `ldap2pg-5.9/ldap2pg/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         defaclrole,
         (aclexplode(defaclacl)).grantee AS grantee,
         (aclexplode(defaclacl)).privilege_type AS priv,
         defaclobjtype AS objtype
       FROM pg_catalog.pg_default_acl
     )
     SELECT
-      priv || '_on_' || objtype AS key,
+      CONCAT(priv, '_on_', objtype) AS key,
       nspname,
       COALESCE(rolname, 'public') AS rolname,
       TRUE AS full,
       pg_catalog.pg_get_userbyid(defaclrole) AS owner
     FROM grants
     JOIN pg_catalog.pg_namespace nsp ON nsp.oid = defaclnamespace
     LEFT OUTER JOIN pg_catalog.pg_roles AS rol ON grants.grantee = rol.oid
```

### Comparing `ldap2pg-5.8/ldap2pg/format.py` & `ldap2pg-5.9/ldap2pg/format.py`

 * *Files identical despite different names*

### Comparing `ldap2pg-5.8/ldap2pg/inspector.py` & `ldap2pg-5.9/ldap2pg/inspector.py`

 * *Files identical despite different names*

### Comparing `ldap2pg-5.8/ldap2pg/ldap.py` & `ldap2pg-5.9/ldap2pg/ldap.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
             auth = sasl.sasl({
                 sasl.CB_AUTHNAME: options['USER'],
                 sasl.CB_PASS: options['PASSWORD'],
             }, mech)
         elif 'GSSAPI' == mech:
             auth = sasl.gssapi(options.get('SASL_AUTHZID'))
         else:
-            raise UserError("Unmanaged SASL mech %s.", mech)
+            raise UserError("Unmanaged SASL mech %s." % mech)
 
         conn.sasl_interactive_bind_s("", auth)
 
     return conn
 
 
 class Options(dict):
```

### Comparing `ldap2pg-5.8/ldap2pg/manager.py` & `ldap2pg-5.9/ldap2pg/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,16 +282,18 @@
 
         logger.info("Inspecting roles in Postgres cluster...")
         self.inspector.roles_blacklist = self.inspector.fetch_roles_blacklist()
         me, issuper = self.inspector.fetch_me()
         if not match(me, self.roles_blacklist):
             self.inspector.roles_blacklist.append(me)
 
-        if not issuper:
-            logger.warning("Running ldap2pg as non superuser.")
+        if issuper:
+            logger.info("Running ldap2pg as superuser.")
+        else:
+            logger.info("Running ldap2pg as non superuser.")
             RoleOptions.filter_super_columns()
 
         databases = self.inspector.fetch_databases()
         pgallroles, pgmanagedroles = self.inspector.fetch_roles()
         pgallroles, pgmanagedroles = self.inspector.filter_roles(
             pgallroles, pgmanagedroles)
         pgallroles.resolve_membership()
```

### Comparing `ldap2pg-5.8/ldap2pg/privilege.py` & `ldap2pg-5.9/ldap2pg/privilege.py`

 * *Files identical despite different names*

### Comparing `ldap2pg-5.8/ldap2pg/psql.py` & `ldap2pg-5.9/ldap2pg/psql.py`

 * *Files identical despite different names*

### Comparing `ldap2pg-5.8/ldap2pg/role.py` & `ldap2pg-5.9/ldap2pg/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,29 +436,36 @@
             if managed:
                 self.add(oldrole)
 
         index = available.reindex()
 
         # Now update kept roles options and memberships, including renamed.
         kept = available & other
+        spurious = RoleSet(self - other - set(['public']))
         other_index = other.reindex()
         for role in kept:
             mine = index[role.name]
             # Rename back member to new role name, keeping objects synchronized
             # with Postgres instance.
             mine.rename_members(renamed)
             its = other_index[role.name]
             if role not in self:
                 logger.warning(
                     "Role %s already exists in cluster. Reusing.", role.name)
+            # Trim to be removed roles. Let DROP take care of membership. This
+            # avoid to remove a member that ldap2pg fails to drop afterward.
+            mine.members[:] = [
+                member
+                for member in mine.members
+                if member not in spurious
+            ]
             for qry in mine.alter(its):
                 yield qry
 
         # Don't forget to trash all spurious managed roles!
-        spurious = RoleSet(self - other - set(['public']))
         # reassign databases to fallback_owner
         for database in databases or []:
             if database.owner in spurious:
                 for query in database.reassign(fallback_owner):
                     yield query
                 # Update representation for the following queries.
                 database.owner = fallback_owner
```

### Comparing `ldap2pg-5.8/ldap2pg/script.py` & `ldap2pg-5.9/ldap2pg/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         config = config_obj.validate_raw_yaml(config, "dict")
 
     args = config_obj.read_argv(argv)
     config_obj.merge(config, environ, args)
     return config_obj
 
 
-def synchronize(config=None, environ=None, argv=None):
+def synchronize(config=None, environ=os.environ, argv=None):
     """Synchronize a Postgres cluster from LDAP directory
 
     This is the main entrypoint of ldap2pg logic. config is either a raw YAML
     string or a Python dict describing the ldap2pg configuration as documented
     in the YAML format.
 
     environ is a dict of environment variables, defaulting to os.environ. argv
```

### Comparing `ldap2pg-5.8/ldap2pg/utils.py` & `ldap2pg-5.9/ldap2pg/utils.py`

 * *Files identical despite different names*

### Comparing `ldap2pg-5.8/ldap2pg/validators.py` & `ldap2pg-5.9/ldap2pg/validators.py`

 * *Files identical despite different names*

### Comparing `ldap2pg-5.8/ldap2pg.egg-info/PKG-INFO` & `ldap2pg-5.9/ldap2pg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ldap2pg
-Version: 5.8
+Version: 5.9
 Summary: Manage PostgreSQL roles and privileges from YAML or LDAP
 Home-page: https://labs.dalibo.com/ldap2pg
 Author: Dalibo
 Author-email: contact@dalibo.com
 License: PostgreSQL
 Project-URL: Documentation, https://ldap2pg.rtfd.io/
 Project-URL: Tracker, https://github.com/dalibo/ldap2pg/issues
```

### Comparing `ldap2pg-5.8/setup.py` & `ldap2pg-5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     install_requires.extend([
         'argparse',
         'logutils',
     ])
 
 setup(
     name='ldap2pg',
-    version='5.8',
+    version='5.9',
     description='Manage PostgreSQL roles and privileges from YAML or LDAP',
     url='https://labs.dalibo.com/ldap2pg',
     project_urls={
         "Documentation": "https://ldap2pg.rtfd.io/",
         "Tracker": "https://github.com/dalibo/ldap2pg/issues",
         "Sources": "https://github.com/dalibo/ldap2pg",
     },
```

