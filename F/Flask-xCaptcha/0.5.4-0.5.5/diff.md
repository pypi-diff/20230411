# Comparing `tmp/Flask-xCaptcha-0.5.4.tar.gz` & `tmp/Flask-xCaptcha-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-xCaptcha-0.5.4.tar", last modified: Fri Jun 17 22:29:56 2022, max compression
+gzip compressed data, was "Flask-xCaptcha-0.5.5.tar", last modified: Tue Apr 11 20:07:14 2023, max compression
```

## Comparing `Flask-xCaptcha-0.5.4.tar` & `Flask-xCaptcha-0.5.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 admin     (1000) users      (100)        0 2022-06-17 22:29:56.720156 Flask-xCaptcha-0.5.4/
-drwxr-xr-x   0 admin     (1000) users      (100)        0 2022-06-17 22:29:56.720156 Flask-xCaptcha-0.5.4/Flask_xCaptcha.egg-info/
--rw-r--r--   0 admin     (1000) users      (100)     5748 2022-06-17 22:29:55.000000 Flask-xCaptcha-0.5.4/Flask_xCaptcha.egg-info/PKG-INFO
--rw-r--r--   0 admin     (1000) users      (100)      280 2022-06-17 22:29:56.000000 Flask-xCaptcha-0.5.4/Flask_xCaptcha.egg-info/SOURCES.txt
--rw-r--r--   0 admin     (1000) users      (100)        1 2022-06-17 22:29:55.000000 Flask-xCaptcha-0.5.4/Flask_xCaptcha.egg-info/dependency_links.txt
--rw-r--r--   0 admin     (1000) users      (100)        1 2022-06-17 15:57:58.000000 Flask-xCaptcha-0.5.4/Flask_xCaptcha.egg-info/not-zip-safe
--rw-r--r--   0 admin     (1000) users      (100)       26 2022-06-17 22:29:56.000000 Flask-xCaptcha-0.5.4/Flask_xCaptcha.egg-info/requires.txt
--rw-r--r--   0 admin     (1000) users      (100)       15 2022-06-17 22:29:56.000000 Flask-xCaptcha-0.5.4/Flask_xCaptcha.egg-info/top_level.txt
--rwxr-xr-x   0 admin     (1000) users      (100)     1090 2022-06-17 15:36:21.000000 Flask-xCaptcha-0.5.4/LICENSE
--rw-r--r--   0 admin     (1000) users      (100)     5748 2022-06-17 22:29:56.720156 Flask-xCaptcha-0.5.4/PKG-INFO
--rw-r--r--   0 admin     (1000) users      (100)     4539 2022-06-17 15:51:20.000000 Flask-xCaptcha-0.5.4/README.md
--rw-r--r--   0 admin     (1000) users      (100)     3509 2022-06-17 22:28:39.000000 Flask-xCaptcha-0.5.4/flask_xcaptcha.py
--rw-r--r--   0 admin     (1000) users      (100)       79 2022-06-17 22:29:56.720156 Flask-xCaptcha-0.5.4/setup.cfg
--rw-r--r--   0 admin     (1000) users      (100)     1704 2022-06-17 16:26:17.000000 Flask-xCaptcha-0.5.4/setup.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 20:07:14.228338 Flask-xCaptcha-0.5.5/
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 20:07:14.223337 Flask-xCaptcha-0.5.5/Flask_xCaptcha.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     5880 2023-04-11 20:07:14.000000 Flask-xCaptcha-0.5.5/Flask_xCaptcha.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)      309 2023-04-11 20:07:14.000000 Flask-xCaptcha-0.5.5/Flask_xCaptcha.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2023-04-11 20:07:14.000000 Flask-xCaptcha-0.5.5/Flask_xCaptcha.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2023-04-11 20:07:13.000000 Flask-xCaptcha-0.5.5/Flask_xCaptcha.egg-info/not-zip-safe
+-rw-r--r--   0 max       (1000) max       (1000)       26 2023-04-11 20:07:14.000000 Flask-xCaptcha-0.5.5/Flask_xCaptcha.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)       15 2023-04-11 20:07:14.000000 Flask-xCaptcha-0.5.5/Flask_xCaptcha.egg-info/top_level.txt
+-rwxr-xr-x   0 max       (1000) max       (1000)     1090 2023-04-11 19:55:11.000000 Flask-xCaptcha-0.5.5/LICENSE
+-rw-r--r--   0 max       (1000) max       (1000)     5880 2023-04-11 20:07:14.229346 Flask-xCaptcha-0.5.5/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     4671 2023-04-11 20:03:01.000000 Flask-xCaptcha-0.5.5/README.md
+-rw-r--r--   0 max       (1000) max       (1000)     3757 2023-04-11 20:03:01.000000 Flask-xCaptcha-0.5.5/flask_xcaptcha.py
+-rw-r--r--   0 max       (1000) max       (1000)       79 2023-04-11 20:07:14.239347 Flask-xCaptcha-0.5.5/setup.cfg
+-rw-r--r--   0 max       (1000) max       (1000)     1704 2023-04-11 19:55:11.000000 Flask-xCaptcha-0.5.5/setup.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-11 20:07:14.226339 Flask-xCaptcha-0.5.5/tests/
+-rw-r--r--   0 max       (1000) max       (1000)     1348 2023-04-11 19:55:11.000000 Flask-xCaptcha-0.5.5/tests/test_flask_xcaptcha.py
```

### Comparing `Flask-xCaptcha-0.5.4/Flask_xCaptcha.egg-info/PKG-INFO` & `Flask-xCaptcha-0.5.5/Flask_xCaptcha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-xCaptcha
-Version: 0.5.4
+Version: 0.5.5
 Summary: The new xCaptcha implementation for Flask without Flask-WTF
 Home-page: https://github.com/bmaximuml/flask-xcaptcha
 Download-URL: https://github.com/bmaximuml/flask-xcaptcha/tarball/master
 Author: Max Levine
 Author-email: max@maxlevine.co.uk
 License: MIT
 Keywords: flask,recaptcha,hcaptcha,xcaptcha,validate
@@ -120,14 +120,15 @@
 XCAPTCHA_THEME      | Theme for the xCaptcha element | light / dark (service dependent) | "light" | Optional
 XCAPTCHA_TYPE       | Type of xCaptcha | service dependent | "image" | Optional
 XCAPTCHA_SIZE       | Size of xCaptcha | normal / compact (service dependent) | "normal" | Optional
 XCAPTCHA_TABINDEX   | Set the tabindex of the widget and popup | integer | 0 | Optional
 XCAPTCHA_VERIFY_URL | The URL to verify the filled in xCaptcha at | URL | "https://www.google.com/recaptcha/api/siteverify" | Optional
 XCAPTCHA_API_URL    | The URL of the xCaptcha API JS script | URL | "//www.google.com/recaptcha/api.js" | Optional
 XCAPTCHA_DIV_CLASS  | The class of the div element surrounding the xCaptcha | string | "g-recaptcha" | Optional
+XCAPTCHA_CALLBACK   | The string that recaptcha finds on a button to see when a button is submitted | "OnSubmitCallback" | Optional
 
 ### In your template: `{{ xcaptcha }}`
 
 Inside of the form you want to protect, include the tag: `{{ xcaptcha }}`
 
 It will insert the code automatically
 
@@ -182,8 +183,8 @@
 
 Returns a bool indicating whether or not the xCaptcha was successfully completed
 
 ## `{{ xcaptcha }}`
 
 This will insert an HTML div element containing the captcha into a Jinja2 template
 
-(c) 2022 Max Levine
+(c) 2023 Max Levine
```

### Comparing `Flask-xCaptcha-0.5.4/LICENSE` & `Flask-xCaptcha-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-xCaptcha-0.5.4/PKG-INFO` & `Flask-xCaptcha-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-xCaptcha
-Version: 0.5.4
+Version: 0.5.5
 Summary: The new xCaptcha implementation for Flask without Flask-WTF
 Home-page: https://github.com/bmaximuml/flask-xcaptcha
 Download-URL: https://github.com/bmaximuml/flask-xcaptcha/tarball/master
 Author: Max Levine
 Author-email: max@maxlevine.co.uk
 License: MIT
 Keywords: flask,recaptcha,hcaptcha,xcaptcha,validate
@@ -120,14 +120,15 @@
 XCAPTCHA_THEME      | Theme for the xCaptcha element | light / dark (service dependent) | "light" | Optional
 XCAPTCHA_TYPE       | Type of xCaptcha | service dependent | "image" | Optional
 XCAPTCHA_SIZE       | Size of xCaptcha | normal / compact (service dependent) | "normal" | Optional
 XCAPTCHA_TABINDEX   | Set the tabindex of the widget and popup | integer | 0 | Optional
 XCAPTCHA_VERIFY_URL | The URL to verify the filled in xCaptcha at | URL | "https://www.google.com/recaptcha/api/siteverify" | Optional
 XCAPTCHA_API_URL    | The URL of the xCaptcha API JS script | URL | "//www.google.com/recaptcha/api.js" | Optional
 XCAPTCHA_DIV_CLASS  | The class of the div element surrounding the xCaptcha | string | "g-recaptcha" | Optional
+XCAPTCHA_CALLBACK   | The string that recaptcha finds on a button to see when a button is submitted | "OnSubmitCallback" | Optional
 
 ### In your template: `{{ xcaptcha }}`
 
 Inside of the form you want to protect, include the tag: `{{ xcaptcha }}`
 
 It will insert the code automatically
 
@@ -182,8 +183,8 @@
 
 Returns a bool indicating whether or not the xCaptcha was successfully completed
 
 ## `{{ xcaptcha }}`
 
 This will insert an HTML div element containing the captcha into a Jinja2 template
 
-(c) 2022 Max Levine
+(c) 2023 Max Levine
```

### Comparing `Flask-xCaptcha-0.5.4/README.md` & `Flask-xCaptcha-0.5.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,15 @@
 XCAPTCHA_THEME      | Theme for the xCaptcha element | light / dark (service dependent) | "light" | Optional
 XCAPTCHA_TYPE       | Type of xCaptcha | service dependent | "image" | Optional
 XCAPTCHA_SIZE       | Size of xCaptcha | normal / compact (service dependent) | "normal" | Optional
 XCAPTCHA_TABINDEX   | Set the tabindex of the widget and popup | integer | 0 | Optional
 XCAPTCHA_VERIFY_URL | The URL to verify the filled in xCaptcha at | URL | "https://www.google.com/recaptcha/api/siteverify" | Optional
 XCAPTCHA_API_URL    | The URL of the xCaptcha API JS script | URL | "//www.google.com/recaptcha/api.js" | Optional
 XCAPTCHA_DIV_CLASS  | The class of the div element surrounding the xCaptcha | string | "g-recaptcha" | Optional
+XCAPTCHA_CALLBACK   | The string that recaptcha finds on a button to see when a button is submitted | "OnSubmitCallback" | Optional
 
 ### In your template: `{{ xcaptcha }}`
 
 Inside of the form you want to protect, include the tag: `{{ xcaptcha }}`
 
 It will insert the code automatically
 
@@ -153,8 +154,8 @@
 
 Returns a bool indicating whether or not the xCaptcha was successfully completed
 
 ## `{{ xcaptcha }}`
 
 This will insert an HTML div element containing the captcha into a Jinja2 template
 
-(c) 2022 Max Levine
+(c) 2023 Max Levine
```

### Comparing `Flask-xCaptcha-0.5.4/flask_xcaptcha.py` & `Flask-xCaptcha-0.5.5/flask_xcaptcha.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 The new xCaptcha implementation for Flask without Flask-WTF
 """
 
 __NAME__ = "Flask-xCaptcha"
-__version__ = "0.5.4"
+__version__ = "0.5.5"
 __license__ = "MIT"
 __author__ = "Max Levine"
-__copyright__ = "(c) 2022 Max Levine"
+__copyright__ = "(c) 2023 Max Levine"
 
 try:
     from flask import request
     try:
         from jinja2 import Markup
     except ImportError:
         from markupsafe import Markup
@@ -21,40 +21,43 @@
 
 class DEFAULTS(object):
     IS_ENABLED = True
     THEME = "light"
     TYPE = "image"
     SIZE = "normal"
     TABINDEX = 0
+    CALLBACK = "onSubmitCallback"
     VERIFY_URL = "https://www.google.com/recaptcha/api/siteverify"
     API_URL = "//www.google.com/recaptcha/api.js"
     DIV_CLASS = "g-recaptcha"
 
 
 class XCaptcha(object):
     def __init__(self,
         app=None,
         site_key=None,
         secret_key=None,
         is_enabled=DEFAULTS.IS_ENABLED,
         theme=DEFAULTS.THEME,
         xtype=DEFAULTS.TYPE,
+        callback=DEFAULTS.CALLBACK,
         size=DEFAULTS.SIZE,
         tabindex=DEFAULTS.TABINDEX,
         verify_url=DEFAULTS.VERIFY_URL,
         api_url=DEFAULTS.API_URL,
         div_class=DEFAULTS.DIV_CLASS,
         **kwargs
     ):
         if app is not None:
             self.site_key = app.config.get("XCAPTCHA_SITE_KEY", site_key)
             self.secret_key = app.config.get('XCAPTCHA_SECRET_KEY', secret_key)
             self.is_enabled = app.config.get("XCAPTCHA_ENABLED", is_enabled)
             self.theme = app.config.get("XCAPTCHA_THEME", theme)
             self.type = app.config.get("XCAPTCHA_TYPE", xtype)
+            self.callback = app.config.get("XCAPTCHA_CALLBACK", callback)
             self.size = app.config.get("XCAPTCHA_SIZE", size)
             self.tabindex = app.config.get("XCAPTCHA_TABINDEX", tabindex)
             self.verify_url = app.config.get("XCAPTCHA_VERIFY_URL", verify_url)
             self.api_url = app.config.get("XCAPTCHA_API_URL", api_url)
             self.div_class = app.config.get("XCAPTCHA_DIV_CLASS", div_class)
 
             @app.context_processor
@@ -63,35 +66,37 @@
 
         elif site_key is not None:
             self.site_key = site_key
             self.secret_key = secret_key
             self.is_enabled = is_enabled
             self.theme = theme
             self.type = xtype
+            self.callback = callback
             self.size = size
             self.tabindex = tabindex
             self.verify_url = verify_url
             self.api_url = api_url
             self.div_class = div_class
 
     def get_code(self):
         """
         Returns the new XCaptcha code
         :return:
         """
         return "" if not self.is_enabled else ("""
         <script src='{API_URL}'></script>
-        <div class="{DIV_CLASS}" data-sitekey="{SITE_KEY}" data-theme="{THEME}" data-type="{TYPE}" data-size="{SIZE}"\
+        <div class="{DIV_CLASS}" data-sitekey="{SITE_KEY}" data-theme="{THEME}" data-type="{TYPE}" data-callback="{CALLBACK}" data-size="{SIZE}"\
          data-tabindex="{TABINDEX}"></div>
         """.format(
                 DIV_CLASS=self.div_class,
                 API_URL=self.api_url,
                 SITE_KEY=self.site_key,
                 THEME=self.theme,
                 TYPE=self.type,
+                CALLBACK=self.callback,
                 SIZE=self.size,
                 TABINDEX=self.tabindex
             )
         )
 
     def verify(self, response=None, remote_ip=None):
         if self.is_enabled:
```

### Comparing `Flask-xCaptcha-0.5.4/setup.py` & `Flask-xCaptcha-0.5.5/setup.py`

 * *Files identical despite different names*

