# Comparing `tmp/muffin_babel-1.4.0.tar.gz` & `tmp/muffin_babel-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_babel-1.4.0.tar", max compression
+gzip compressed data, was "muffin_babel-1.4.1.tar", max compression
```

## Comparing `muffin_babel-1.4.0.tar` & `muffin_babel-1.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4396 2023-04-10 06:15:52.596801 muffin_babel-1.4.0/README.rst
--rw-r--r--   0        0        0    10134 2023-04-10 06:15:52.596801 muffin_babel-1.4.0/muffin_babel/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 06:15:52.596801 muffin_babel-1.4.0/muffin_babel/py.typed
--rw-r--r--   0        0        0     2030 2023-04-10 06:15:52.596801 muffin_babel-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     5691 1970-01-01 00:00:00.000000 muffin_babel-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4396 2023-04-11 04:53:29.650874 muffin_babel-1.4.1/README.rst
+-rw-r--r--   0        0        0    10310 2023-04-11 04:53:29.650874 muffin_babel-1.4.1/muffin_babel/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 04:53:29.650874 muffin_babel-1.4.1/muffin_babel/py.typed
+-rw-r--r--   0        0        0     2030 2023-04-11 04:53:29.650874 muffin_babel-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5691 1970-01-01 00:00:00.000000 muffin_babel-1.4.1/PKG-INFO
```

### Comparing `muffin_babel-1.4.0/README.rst` & `muffin_babel-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_babel-1.4.0/muffin_babel/__init__.py` & `muffin_babel-1.4.1/muffin_babel/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,32 +40,33 @@
         "sources_map": [
             ("**.py", "python"),
             ("**.html", "jinja2"),
         ],
         "options_map": {"**.html": {"encoding": "utf-8"}},
     }
 
-    def setup(self, app: Application, **options):  # noqa: C901
+    def setup(self, app: Application, **options):  # noqa: C901,PLR0915
         """Setup the plugin's commands."""
         super(Plugin, self).setup(app, **options)
+        self.domain = self.cfg.domain
 
         self.__locale_selector: Callable[
             [Request],
             Awaitable[Optional[str]],
         ] = select_locale_by_request
 
         # Install a middleware for autodetection
         if self.cfg.auto_detect_locale:
             app.middleware(self.__middleware__, insert_first=True)
 
         @app.manage(lifespan=False)
         def babel_extract_messages(
             *dirnames: str,
             project: str = app.cfg.name,
-            domain: str = self.cfg.domain,
+            domain: str = self.domain,
             locations: bool = True,
             charset: str = "utf-8",
             locale: str = self.cfg.default_locale,
         ):
             """Extract messages from source code.
 
             :param charset: charset to use in the output
@@ -110,15 +111,15 @@
                 output.parent.mkdir(parents=True)
 
             logger.info("writing PO template file to %s", output)
             with output.open("wb") as f:
                 write_po(f, catalog, sort_output=not locations, sort_by_file=locations)
 
         @app.manage(lifespan=False)
-        def babel_compile_messages(*, use_fuzzy=False, domain=self.cfg.domain):
+        def babel_compile_messages(*, use_fuzzy=False, domain=self.domain):
             """Compile messages for locales.
 
             :param domain:  set domain name for locales
             """
             for locales_dir in self.cfg.locale_folders:
                 source = Path(locales_dir)
                 for locale in source.iterdir():
@@ -132,17 +133,15 @@
                     mo_file = po_file.with_suffix(".mo")
 
                     with mo_file.open("wb") as mo:
                         logger.info("writing MO template file to %s", mo_file)
                         write_mo(mo, catalog, use_fuzzy=use_fuzzy)
 
         @app.manage(lifespan=False)
-        def babel_export_csv(
-            *, domain: str = self.cfg.domain, locale: str = self.cfg.default_locale
-        ):
+        def babel_export_csv(*, domain: str = self.domain, locale: str = self.cfg.default_locale):
             """Export messages from a PO files as CSV."""
             writer = csv.writer(sys.stdout)
             writer.writerow(["id", "string", "context", "comment"])
             for locales_dir in self.cfg.locale_folders:
                 po_file = Path(locales_dir) / locale / "LC_MESSAGES" / f"{domain}.po"
                 if not po_file.exists():
                     continue
@@ -208,15 +207,15 @@
         current_locale.set(old_locale)
 
     def get_translations(
         self, domain: Optional[str] = None, locale: Optional[Locale] = None
     ) -> support.Translations:
         """Load and cache translations."""
         locale = locale or self.current_locale
-        domain = domain or self.cfg.domain
+        domain = domain or self.domain
         if (domain, locale.language) not in TRANSLATIONS:
             translations = None
             for path in reversed(self.cfg.locale_folders):
                 trans = support.Translations.load(path, locales=locale.language, domain=domain)
                 if translations:
                     translations._catalog.update(trans._catalog)
                 else:
@@ -225,15 +224,15 @@
             TRANSLATIONS[(domain, locale.language)] = translations  # type: ignore[assignment]
 
         return TRANSLATIONS[(domain, locale.language)]
 
     def gettext(self, string: str, domain: Optional[str] = None, **variables) -> str:
         """Translate a string with the current locale."""
         t = self.get_translations(domain)
-        return t.ugettext(string) % variables
+        return render(t.ugettext(string), variables)
 
     def ngettext(
         self, singular: str, plural: str, num: int, domain: Optional[str] = None, **variables
     ) -> str:
         """Translate a string wity the current locale.
 
         The `num` parameter is used to dispatch between singular and various plural forms of the
@@ -243,15 +242,15 @@
         variables.setdefault("num", num)
         t = self.get_translations(domain)
         return t.ungettext(singular, plural, num) % variables
 
     def pgettext(self, context: str, string: str, domain: Optional[str] = None, **variables) -> str:
         """Like :meth:`gettext` but with a context."""
         t = self.get_translations(domain)
-        return t.upgettext(context, string) % variables
+        return render(t.upgettext(context, string), variables)
 
     def npgettext(
         self,
         context: str,
         singular: str,
         plural: str,
         num: int,
@@ -260,8 +259,15 @@
     ) -> str:
         """Like :meth:`ngettext` but with a context."""
         variables.setdefault("num", num)
         t = self.get_translations(domain)
         return t.unpgettext(context, singular, plural, num) % variables
 
 
+def render(value: str, variables) -> str:
+    """Render a string with variables."""
+    if variables:
+        return value % variables
+    return value
+
+
 # ruff: noqa: PLR0913
```

### Comparing `muffin_babel-1.4.0/pyproject.toml` & `muffin_babel-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-babel"
-version = "1.4.0"
+version = "1.4.1"
 description = "Localization support for the Muffin Framework"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["localization", "internationalization", "muffin", "babel", "asyncio", "trio", "asgi"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `muffin_babel-1.4.0/PKG-INFO` & `muffin_babel-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-babel
-Version: 1.4.0
+Version: 1.4.1
 Summary: Localization support for the Muffin Framework
 Home-page: https://github.com/klen/muffin-babel
 License: MIT
 Keywords: localization,internationalization,muffin,babel,asyncio,trio,asgi
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

