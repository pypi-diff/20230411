# Comparing `tmp/odoo_addon_session_db-16.0.1.0.3-py3-none-any.whl.zip` & `tmp/odoo_addon_session_db-16.0.1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,18 @@
-Zip file size: 21978 bytes, number of entries: 14
--rw-r--r--  2.0 unx     3398 b- defN 23-Feb-21 09:49 odoo/addons/session_db/README.rst
--rw-r--r--  2.0 unx       31 b- defN 23-Feb-21 09:49 odoo/addons/session_db/__init__.py
--rw-r--r--  2.0 unx      251 b- defN 23-Feb-21 09:49 odoo/addons/session_db/__manifest__.py
--rw-r--r--  2.0 unx     4341 b- defN 23-Feb-21 09:49 odoo/addons/session_db/pg_session_store.py
--rw-r--r--  2.0 unx      341 b- defN 23-Feb-21 09:49 odoo/addons/session_db/i18n/session_db.pot
--rw-r--r--  2.0 unx      206 b- defN 23-Feb-21 09:49 odoo/addons/session_db/readme/DESCRIPTION.rst
--rw-r--r--  2.0 unx       83 b- defN 23-Feb-21 09:49 odoo/addons/session_db/readme/ROADMAP.rst
--rw-r--r--  2.0 unx      312 b- defN 23-Feb-21 09:49 odoo/addons/session_db/readme/USAGE.rst
--rw-r--r--  2.0 unx     9455 b- defN 23-Feb-21 09:49 odoo/addons/session_db/static/description/icon.png
--rw-r--r--  2.0 unx    12745 b- defN 23-Feb-21 09:49 odoo/addons/session_db/static/description/index.html
--rw-r--r--  2.0 unx     3944 b- defN 23-Feb-21 09:49 odoo_addon_session_db-16.0.1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-21 09:49 odoo_addon_session_db-16.0.1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Feb-21 09:49 odoo_addon_session_db-16.0.1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1352 b- defN 23-Feb-21 09:49 odoo_addon_session_db-16.0.1.0.3.dist-info/RECORD
-14 files, 36556 bytes uncompressed, 19652 bytes compressed:  46.2%
+Zip file size: 23398 bytes, number of entries: 16
+-rw-r--r--  2.0 unx     3398 b- defN 23-Apr-11 14:47 odoo/addons/session_db/README.rst
+-rw-r--r--  2.0 unx       31 b- defN 23-Apr-11 14:47 odoo/addons/session_db/__init__.py
+-rw-r--r--  2.0 unx      251 b- defN 23-Apr-11 14:47 odoo/addons/session_db/__manifest__.py
+-rw-r--r--  2.0 unx     4699 b- defN 23-Apr-11 14:47 odoo/addons/session_db/pg_session_store.py
+-rw-r--r--  2.0 unx      341 b- defN 23-Apr-11 14:47 odoo/addons/session_db/i18n/session_db.pot
+-rw-r--r--  2.0 unx      206 b- defN 23-Apr-11 14:47 odoo/addons/session_db/readme/DESCRIPTION.rst
+-rw-r--r--  2.0 unx       83 b- defN 23-Apr-11 14:47 odoo/addons/session_db/readme/ROADMAP.rst
+-rw-r--r--  2.0 unx      312 b- defN 23-Apr-11 14:47 odoo/addons/session_db/readme/USAGE.rst
+-rw-r--r--  2.0 unx     9455 b- defN 23-Apr-11 14:47 odoo/addons/session_db/static/description/icon.png
+-rw-r--r--  2.0 unx    12745 b- defN 23-Apr-11 14:47 odoo/addons/session_db/static/description/index.html
+-rw-r--r--  2.0 unx       36 b- defN 23-Apr-11 14:47 odoo/addons/session_db/tests/__init__.py
+-rw-r--r--  2.0 unx     3057 b- defN 23-Apr-11 14:47 odoo/addons/session_db/tests/test_pg_session_store.py
+-rw-r--r--  2.0 unx     3944 b- defN 23-Apr-11 14:47 odoo_addon_session_db-16.0.1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 14:47 odoo_addon_session_db-16.0.1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-11 14:47 odoo_addon_session_db-16.0.1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1557 b- defN 23-Apr-11 14:47 odoo_addon_session_db-16.0.1.0.4.dist-info/RECORD
+16 files, 40212 bytes uncompressed, 20734 bytes compressed:  48.4%
```

## zipnote {}

```diff
@@ -24,20 +24,26 @@
 
 Filename: odoo/addons/session_db/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/session_db/static/description/index.html
 Comment: 
 
-Filename: odoo_addon_session_db-16.0.1.0.3.dist-info/METADATA
+Filename: odoo/addons/session_db/tests/__init__.py
 Comment: 
 
-Filename: odoo_addon_session_db-16.0.1.0.3.dist-info/WHEEL
+Filename: odoo/addons/session_db/tests/test_pg_session_store.py
 Comment: 
 
-Filename: odoo_addon_session_db-16.0.1.0.3.dist-info/top_level.txt
+Filename: odoo_addon_session_db-16.0.1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addon_session_db-16.0.1.0.3.dist-info/RECORD
+Filename: odoo_addon_session_db-16.0.1.0.4.dist-info/WHEEL
+Comment: 
+
+Filename: odoo_addon_session_db-16.0.1.0.4.dist-info/top_level.txt
+Comment: 
+
+Filename: odoo_addon_session_db-16.0.1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/session_db/__manifest__.py

```diff
@@ -1,8 +1,8 @@
 {
     "name": "Store sessions in DB",
-    "version": "16.0.1.0.3",
+    "version": "16.0.1.0.4",
     "author": "Odoo SA,ACSONE SA/NV,Odoo Community Association (OCA)",
     "license": "LGPL-3",
     "website": "https://github.com/OCA/server-tools",
     "maintainers": ["sbidoul"],
 }
```

## odoo/addons/session_db/pg_session_store.py

```diff
@@ -41,48 +41,60 @@
 
 def with_cursor(func):
     def wrapper(self, *args, **kwargs):
         tries = 0
         while True:
             tries += 1
             try:
+                self._ensure_connection()
                 return func(self, *args, **kwargs)
-            except (psycopg2.InterfaceError, psycopg2.OperationalError) as e:
-                _logger.info("Session in DB connection Retry %s/5" % tries)
+            except (psycopg2.InterfaceError, psycopg2.OperationalError):
+                self._close_connection()
                 if tries > 4:
-                    raise e
-                self._open_connection()
+                    _logger.warning(
+                        "session_db operation try %s/5 failed, aborting", tries
+                    )
+                    raise
+                _logger.info("session_db operation try %s/5 failed, retrying", tries)
 
     return wrapper
 
 
 class PGSessionStore(sessions.SessionStore):
     def __init__(self, uri, session_class=None):
         super().__init__(session_class)
         self._uri = uri
         self._cr = None
         self._open_connection()
         self._setup_db()
 
     def __del__(self):
-        if self._cr is not None:
-            self._cr.close()
+        self._close_connection()
+
+    @with_lock
+    def _ensure_connection(self):
+        if self._cr is None:
+            self._open_connection()
 
     @with_lock
     def _open_connection(self):
-        # return cursor to the pool
+        self._close_connection()
+        cnx = odoo.sql_db.db_connect(self._uri, allow_uri=True)
+        self._cr = cnx.cursor()
+        self._cr._cnx.autocommit = True
+
+    @with_lock
+    def _close_connection(self):
+        """Return cursor to the pool."""
         if self._cr is not None:
             try:
                 self._cr.close()
             except Exception:  # pylint: disable=except-pass
                 pass
             self._cr = None
-        cnx = odoo.sql_db.db_connect(self._uri, allow_uri=True)
-        self._cr = cnx.cursor()
-        self._cr._cnx.autocommit = True
 
     @with_lock
     @with_cursor
     def _setup_db(self):
         self._cr.execute(
             """
                 CREATE TABLE IF NOT EXISTS http_sessions (
```

## Comparing `odoo_addon_session_db-16.0.1.0.3.dist-info/METADATA` & `odoo_addon_session_db-16.0.1.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addon-session-db
-Version: 16.0.1.0.3
+Version: 16.0.1.0.4
 Summary: Store sessions in DB
 Home-page: https://github.com/OCA/server-tools
 Author: Odoo SA,ACSONE SA/NV,Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: LGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `odoo_addon_session_db-16.0.1.0.3.dist-info/RECORD` & `odoo_addon_session_db-16.0.1.0.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 odoo/addons/session_db/README.rst,sha256=0-lBHLjixU92kg1QIBCSL6EhO94jWxxlmPpae2PEudg,3398
 odoo/addons/session_db/__init__.py,sha256=PVM3bucL2EzItoVUqRcC9hplW7KuhmOTCjv6leqVXWQ,31
-odoo/addons/session_db/__manifest__.py,sha256=lm-iTsOIm4nZYALBnAxoE8b6-fOP5J64Cumeq3owQ3A,251
-odoo/addons/session_db/pg_session_store.py,sha256=mAnrSs9RRNrs-Rps4y-5nPQx68I0ZJkZ64pvWK7cS1Q,4341
+odoo/addons/session_db/__manifest__.py,sha256=VgzAftgZy-YgX8Tn3_7CfnCt0HJjVCiBlqOkEOYZFo0,251
+odoo/addons/session_db/pg_session_store.py,sha256=03YIdCwlnSxl4MMD4C7MhFhzdq2-aB5hBHNPzB3nfuY,4699
 odoo/addons/session_db/i18n/session_db.pot,sha256=leB6MlaWiU1sPOdcOTxNVY5KVORnHv0MfD14HgQJIIs,341
 odoo/addons/session_db/readme/DESCRIPTION.rst,sha256=d84Ye-2qA3Vb3-CKkhLDgPrwDzLYcGSHpwsKDqmwDdA,206
 odoo/addons/session_db/readme/ROADMAP.rst,sha256=tjuz6o7GPU_OvBRxMrjauZZ_o_4nBoNy9ZcmEuS-agk,83
 odoo/addons/session_db/readme/USAGE.rst,sha256=3mtjrhdBiktzD_z1Elmw1NAIv5zzjCiXScf7nFPTeO8,312
 odoo/addons/session_db/static/description/icon.png,sha256=6xBPJauaFOF0KDHfHgQopSc28kKvxMaeoQFQWZtfZDo,9455
 odoo/addons/session_db/static/description/index.html,sha256=y43VOGs-jHVyNIm3fnRatu41Qztld3TLb1AC8yjdGwo,12745
-odoo_addon_session_db-16.0.1.0.3.dist-info/METADATA,sha256=NbBGqQW5ESQBy6Gi0_WS7eiz89U7ehFwx1q9CDa5o_A,3944
-odoo_addon_session_db-16.0.1.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-odoo_addon_session_db-16.0.1.0.3.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo_addon_session_db-16.0.1.0.3.dist-info/RECORD,,
+odoo/addons/session_db/tests/__init__.py,sha256=T3ue0WvaufnQmExTwvSf9HF6U__NPpbi8HudWcRwTA4,36
+odoo/addons/session_db/tests/test_pg_session_store.py,sha256=1ytD1TOE9pcOAP74BOKa2Gp211T47Tyn567YKN5PKkY,3057
+odoo_addon_session_db-16.0.1.0.4.dist-info/METADATA,sha256=MZJa3YZQPNUzSjxHYYgb7rI7et82gKESc4hd05WivgY,3944
+odoo_addon_session_db-16.0.1.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+odoo_addon_session_db-16.0.1.0.4.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo_addon_session_db-16.0.1.0.4.dist-info/RECORD,,
```

