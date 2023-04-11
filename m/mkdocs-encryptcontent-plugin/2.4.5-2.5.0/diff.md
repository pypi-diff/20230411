# Comparing `tmp/mkdocs-encryptcontent-plugin-2.4.5.tar.gz` & `tmp/mkdocs-encryptcontent-plugin-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-encryptcontent-plugin-2.4.5.tar", last modified: Thu Jan 26 16:55:08 2023, max compression
+gzip compressed data, was "mkdocs-encryptcontent-plugin-2.5.0.tar", last modified: Tue Apr 11 19:45:56 2023, max compression
```

## Comparing `mkdocs-encryptcontent-plugin-2.4.5.tar` & `mkdocs-encryptcontent-plugin-2.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-01-26 16:55:08.067522 mkdocs-encryptcontent-plugin-2.4.5/
--rw-rw-rw-   0        0        0     1070 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.4.5/LICENSE.md
--rw-rw-rw-   0        0        0    30343 2023-01-26 16:55:08.066522 mkdocs-encryptcontent-plugin-2.4.5/PKG-INFO
--rw-rw-rw-   0        0        0    24241 2023-01-19 18:42:22.000000 mkdocs-encryptcontent-plugin-2.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-01-26 16:55:07.936520 mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/
--rw-rw-rw-   0        0        0        0 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-26 16:55:07.853525 mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/contrib/
-drwxrwxrwx   0        0        0        0 2023-01-26 16:55:07.853525 mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/contrib/templates/
-drwxrwxrwx   0        0        0        0 2023-01-26 16:55:08.034521 mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/contrib/templates/search/
--rw-rw-rw-   0        0        0    99860 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/contrib/templates/search/lunr.js
--rw-rw-rw-   0        0        0     3670 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/contrib/templates/search/main.js
--rw-rw-rw-   0        0        0     4195 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/contrib/templates/search/worker.js
--rw-rw-rw-   0        0        0    14476 2022-12-31 13:16:34.000000 mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/decrypt-contents.tpl.js
--rw-rw-rw-   0        0        0     1043 2022-12-18 17:37:04.000000 mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/decrypt-form.tpl.html
--rw-rw-rw-   0        0        0    29308 2023-01-19 20:38:28.000000 mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/plugin.py
-drwxrwxrwx   0        0        0        0 2023-01-26 16:55:08.064520 mkdocs-encryptcontent-plugin-2.4.5/mkdocs_encryptcontent_plugin.egg-info/
--rw-rw-rw-   0        0        0    30343 2023-01-26 16:55:07.000000 mkdocs-encryptcontent-plugin-2.4.5/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-01-26 16:55:07.000000 mkdocs-encryptcontent-plugin-2.4.5/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-26 16:55:07.000000 mkdocs-encryptcontent-plugin-2.4.5/mkdocs_encryptcontent_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-01-26 16:55:07.000000 mkdocs-encryptcontent-plugin-2.4.5/mkdocs_encryptcontent_plugin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       42 2023-01-26 16:55:07.000000 mkdocs-encryptcontent-plugin-2.4.5/mkdocs_encryptcontent_plugin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-01-26 16:55:07.000000 mkdocs-encryptcontent-plugin-2.4.5/mkdocs_encryptcontent_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-26 16:55:08.067522 mkdocs-encryptcontent-plugin-2.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1780 2023-01-19 15:22:07.000000 mkdocs-encryptcontent-plugin-2.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:45:56.562727 mkdocs-encryptcontent-plugin-2.5.0/
+-rw-rw-rw-   0        0        0     1070 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.0/LICENSE.md
+-rw-rw-rw-   0        0        0    33921 2023-04-11 19:45:56.561728 mkdocs-encryptcontent-plugin-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    27027 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 19:45:56.475730 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/
+-rw-rw-rw-   0        0        0        0 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:45:56.454730 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/
+drwxrwxrwx   0        0        0        0 2023-04-11 19:45:56.454730 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/
+drwxrwxrwx   0        0        0        0 2023-04-11 19:45:56.538730 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/
+-rw-rw-rw-   0        0        0    99860 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/lunr.js
+-rw-rw-rw-   0        0        0     3670 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/main.js
+-rw-rw-rw-   0        0        0     4195 2022-11-15 20:50:32.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/worker.js
+-rw-rw-rw-   0        0        0    14540 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/decrypt-contents.tpl.js
+-rw-rw-rw-   0        0        0     1206 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/decrypt-form.tpl.html
+-rw-rw-rw-   0        0        0    35943 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/plugin.py
+drwxrwxrwx   0        0        0        0 2023-04-11 19:45:56.559730 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/
+-rw-rw-rw-   0        0        0    33921 2023-04-11 19:45:56.000000 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-04-11 19:45:56.000000 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 19:45:56.000000 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-04-11 19:45:56.000000 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 19:45:56.000000 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-11 19:45:56.000000 mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 19:45:56.562727 mkdocs-encryptcontent-plugin-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1780 2023-04-11 19:41:08.000000 mkdocs-encryptcontent-plugin-2.5.0/setup.py
```

### Comparing `mkdocs-encryptcontent-plugin-2.4.5/LICENSE.md` & `mkdocs-encryptcontent-plugin-2.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.4.5/PKG-INFO` & `mkdocs-encryptcontent-plugin-2.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-encryptcontent-plugin
-Version: 2.4.5
+Version: 2.5.0
 Summary: A MkDocs plugin that encrypt/decrypt markdown content with AES
 Home-page: https://github.com/unverbuggt/mkdocs-encryptcontent-plugin
 Author: unverbuggt
 Author-email: unverbuggt@xn--rthlein-n2a.de
 License: MIT
 Description: # mkdocs-encryptcontent-plugin
         
@@ -28,37 +28,43 @@
         >
         > If a password is defined in an article or a page, it is always used even if there is a global password.
         >
         > If a password is defined as an empty character string, the content is not protected.
         
         ![encryptcontent_demo](https://user-images.githubusercontent.com/12155947/177001700-f0920d4b-0c41-4d11-8164-9f63d29d8a6a.gif)
         
+        # Todo for 2.6.x
+        
+        * Rework password handling or inventory of some sort
+        * ...to be defined
         
         # Table of Contents
         
           * [Installation](#installation)
           * [Usage](#usage)
             * [Global password protection](#global-password-protection)
-            * [Secret from environment](#secret-from-environment) **(UPDATE)**
+            * [Secret from environment](#secret-from-environment)
             * [Customization](#default-vars-customization)
+            * [Translations](#translations)
+            * [Obfuscate pages](#obfuscate-pages) **NEW**
           * [Features](#features)
             * [HighlightJS support](#highlightjs-support) *(default)*
             * [Arithmatex support](#arithmatex-support) *(default)*
             * [Mermaid2 support](#mermaid-support) *(default)*
             * [Tag encrypted page](#tag-encrypted-page) *(default)*
             * [Remember password](#remember-password)
             * [Encrypt something](#encrypt-something)
-            * [Inject decrypt-form.tpl to theme](#inject-decrypt-formtpl-to-theme) **(NEW)**
+            * [Inject decrypt-form.tpl to theme](#inject-decrypt-formtpl-to-theme)
             * [Search index encryption](#search-index-encryption)
-            * [Search index encryption for mkdocs-material](#search-index-encryption-for-mkdocs-material) **(NEW)**
+            * [Search index encryption for mkdocs-material](#search-index-encryption-for-mkdocs-material)
             * [Override default templates](#override-default-templates)
             * [Add button](#add-button)
             * [Reload scripts](#reload-scripts)
-            * [Self-host crypto-js](#self-host-crypto-js) **(NEW)**
-            * [Translations](#translations) **(NEW)**
+            * [Self-host crypto-js](#self-host-crypto-js) *UPDATE*
+            * [File name obfuscation](#file-name-obfuscation) **NEW**
           * [Contributing](#contributing)
         
         
         # Installation
         
         Install the package with pip:
         
@@ -67,15 +73,15 @@
         ```
         
         Install the package from source with pip:
         
         ```bash
         cd mkdocs-encryptcontent-plugin/
         python setup.py sdist bdist_wheel
-        pip install dist/mkdocs_encryptcontent_plugin-2.4.5-py3-none-any.whl
+        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.0-py3-none-any.whl
         ```
         
         Enable the plugin in your `mkdocs.yml`:
         
         ```yaml
         plugins:
             - search: {}
@@ -97,15 +103,16 @@
         plugins:
             - encryptcontent:
                 global_password: 'your_password'
         ```
         
         If a password is defined in an article, it will **ALWAYS** overwrite the global password. 
         
-        > **NOTE** Keep in mind that if the `password:` tag exists without value in an article, it will **not be protected** !
+        > **NOTE** Keep in mind that if the `password:` tag exists without value in a page, it will **not be protected** !
+        > Use this to **disable** `global_password` on specific pages.
         
         
         ### Secret from environment
         
         Instead of specifying a password in the mkdocs.yml file, you can use an environment variable to load your secret. 
         
         This process is in two steps:
@@ -122,28 +129,28 @@
         
         > **NOTE** Keep in mind that if the `use_secret:` configuration is set, it will always be used even if you have also set a global password with the `global_password` variable.
         >
         > If this environment variable is empty or missing, then the build will fail to prevent the unwanted leak of information.
         > However this can be converted into a warning by setting `ignore_missing_secret: true`. 
         > Use this only if you use a secret environment variable for production and a plain password for testing. You have been warned.
         
-        > **NEW** The meta tag `use_secret` can also be set to achieve the same functionality on page level.
+        > The meta tag `use_secret` can also be set to achieve the same functionality on page level.
         
         ### Default vars customization
         
         Optionally you can use some extra variables in plugin configuration to customize default messages.
         
         ```yaml
         plugins:
             - encryptcontent:
                 title_prefix: '[LOCK]'
                 summary: 'another informational message to encrypted content'
                 placeholder: 'another password placeholder'
-                decryption_failure_message: 'another informational message when decryption fail'
-                encryption_info_message: 'another information message when you dont have acess !'
+                decryption_failure_message: 'another informational message when decryption fails'
+                encryption_info_message: "another information message when you don't have access !"
                 input_class: 'md-search__form md-search__input'
                 button_class: 'md-search__icon'
         ```
         
         Default prefix title is `[Protected]`.
         
         Default summary message is `This content is protected with AES encryption.`.
@@ -152,15 +159,46 @@
         
         Default decryption failure message is `Invalid password.`.
         
         Defaut encryption information message is `Contact your administrator for access to this page.`.
         
         > **NOTE** Adding a prefix to the title does not change the default navigation path !
         
-        Use `input_class` and `button_class` to optionally set a CSS class for the password field and the button.
+        ### Translations
+        
+        If the plugin is used in conjunction with the [static-i18n](https://ultrabug.github.io/mkdocs-static-i18n/) plugin you can provide `translations` for the used `i18n_page_file_locale`.
+        
+        ```yaml
+            - encryptcontent:
+                #...
+                translations:
+                  de:
+                    title_prefix: '[Verschlüsselt] '
+                    summary: 'Der Inhalt dieser Seite ist mit AES verschlüsselt. '
+                    placeholder: 'Mit Strg+Enter wird das Passwort global gesetzt'
+                    password_button_text: 'Entschlüsseln'
+                    decryption_failure_message: 'Falsches passwort.'
+                    encryption_info_message: 'Bitte wenden Sie sich an den Systemadministrator um auf diese Seite zuzugreifen.'
+        ```
+        
+        #### Custom per-page strings
+        
+        You can set the  meta tag `encryption_summary` to customize `summary` and `encryption_info_message` on every page.
+        
+        ### Obfuscate pages
+        
+        If you want to make it harder for search engines to scrape you pages content,
+        you can set `obfuscate: SomeNotSoSecretPassword` meta tag in markdown.
+        
+        The page than will display `summary` and `encryption_info_message` together with a button labeled with.
+        `password_button_text`. In order to view the pages content one hast to press the button first.
+        
+        If a `password` or `use_secret` is set, then the `obfuscate` feature will be disabled.
+        If you want to use `obfuscate` in a configuration where `global_password` is defined, 
+        you'll need to set `password:` meta tag (with no password defined) to undefine the password on this page.
         
         # Features
         
         ### HighlightJS support
         
         > **Enable by default**
         
@@ -216,16 +254,15 @@
         
         > **Enable by default**
         
         Related to [issue #7](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin/issues/7)
         
         This feature add an additional attribute `encrypted` with value `True` to the mkdocs type `mkdocs.nav.page` object.
         
-        You can add `tag_encrypted_page: False` in plugin configuration, to disable tagging of encrypted pages. **BUT** This feature is neccessary for others feature working correctly. 
-        If you disable this feature, f.ex. [Encrypt something](#encrypt-something) and [Search index encryption](#search-index-encryption) won't work.
+        You can add `tag_encrypted_page: False` in plugin configuration, to disable tagging of encrypted pages. 
         
         When enable, it becomes possible to use `encrypted` attribute in the jinja template of your theme, as a condition to perform custom modification.
         
         ```jinja
         {%- for nav_item in nav %}
             {% if nav_item.encrypted %}
                 <!-- Do something --> 
@@ -253,37 +290,39 @@
         When enabled, each time you fill password form and press `Enter` a key on session storage is create with your password
         as value. When you reload the page, if you already have an 'encryptcontent' key in the session storage of your browser,
         the page will be automatically decrypted using the value previously created.
         
         By default, the key is created with a name relative to the page on which it was generated.
         This 'relative' key will always be used as first attempt to decrypt the current page when loading.
         
-        If your password is a [global password](#global-password-protection), you can fill in the form field  `mkdocs-content-password`, then use the keyboard shortcut `CTRL + ENTER` instead of the classic `ENTER`. 
+        If your password is a [global password](#global-password-protection), you can fill in the form
+        field  `mkdocs-content-password`, then use the keyboard shortcut `CTRL + ENTER` instead of the classic `ENTER`. 
         The key that will be created with a generic name to making it accessible, by default, on all the pages of your site.
         
         The form of decryption remains visible as long as the content has not been successfully decrypted, which allows in case of error to retry. 
         All keys created with this feature on sessionStorage/localStorage have an default expire time daly set to 24 hours, just cause ...
         
         However *(optionally)*, its possible to change the default expire time by setting options `default_expire_delay: <number>` in your `mkdocs.yml`. Your configuration should look like this when you enabled this feature :
         ```yaml
         plugins:
             - encryptcontent:
                 remember_password: True
                 default_expire_delay: 24   # <-- Default expire delay in hours (optional)
         ```
         
-        > **NOTE** The expired elements of the localStorage are only deleted by the execution of the decrypt-content.js scripts and therefore by the navigation on the site. Secret items can therefore remain visible in local storage after their expiration dates. 
-        > Now The default is to use sessionStorage instead of localStorage, so the browser forgets the password after the current tab was closed. However it can be set to use localStorage by setting `session_storage: False`
+        > **NOTE** The expired elements of the localStorage are only deleted by the execution of the decrypt-content.js
+        > scripts and therefore by the navigation on the site. Secret items can therefore remain visible in local storage
+        > after their expiration dates. 
+        > Now The default is to use sessionStorage instead of localStorage, so the browser forgets the password after
+        > the current tab was closed. However it can be set to use localStorage by setting `session_storage: False`
         
         ### Encrypt something
         
         Related to [issue #9](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin/issues/9)
         
-        The [tag encrypted page feature](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin#tag-encrypted-page) **MUST** be enabled (it's default) for this feature to work properly.
-        
         Add `encrypted_something: {}` in the plugin configuration variable, to encrypt something else.
         
         The syntax of this new variable **MUST** follow the yaml format of a dictionary. 
         Child elements of `encrypted_something` are build with a key `<unique name>` in string format and a list as value. 
         The list have to be contructed with the name of an HTML element `<html tag>` as first item and `id` or `class` as the second item.
         
         ```yaml
@@ -327,15 +366,15 @@
         ```yaml
         plugins:
             - encryptcontent:
                 encrypted_something:
                     mkdocs-encrypted-toc: [div, id]
         ```
         
-        2. Other example, with multiples target. In you Material Theme, you want to encrypt ToC content and Footer.
+        2. Other example, with multiples target. In your custom Material theme, you want to encrypt ToC content and Footer.
         
         Materiel generate 2 `<nav>` structure with the same template `toc.html`, so you need to use a `class` instead of an id for this part.
         The footer part, is generated by the `footer.html` template in a classic div so an `id` is sufficient
         
         After modification, your template looks like this :
         ```jinja (toc.html)
         <nav class="md-nav md-nav--secondary {% if page.encrypted %}mkdocs-encrypted-toc{% endif %}" aria-label="{{ lang.t('toc.title') }}">
@@ -346,25 +385,26 @@
         ```jinja (footer.html)
         <footer class="md-footer">
             <div class="md-footer-nav" {% if page.encrypted %}id="mkdocs-encrypted-footer"{% endif %}> ... </div>
             <div class="md-footer-meta md-typeset" {% if page.encrypted %}id="mkdocs-encrypted-footer-meta"{% endif %}>
         </footer>
         ```
         
-        Your configuration like this :
+        Your configuration would look like this :
         ```yaml
         plugins:
             - encryptcontent:
                 encrypted_something:
                     mkdocs-encrypted-toc: [nav, class]
                     mkdocs-encrypted-footer: [div, id]
                     mkdocs-encrypted-footer-meta: [div, id]
         ```
         
-        3. If you are using mkdocs-material, then this example will also encrypt menu, toc and footer
+        3. If you are using unmodified mkdocs-material, then this example will encrypt menu, toc and footer
+        But you'd need the Navigation pruning feature to hide the title of encrypted pages from navigation (or see 2.).
         
         ```yaml
         plugins:
             - encryptcontent:
                 encrypted_something:
                     md-footer__inner: [nav, class]
                     md-nav: [nav, class]
@@ -391,14 +431,16 @@
                 encrypted_something:
                     md-footer__inner: [nav, class] #Footer
                     md-nav: [nav, class] #Menu and toc
                 inject:
                     md-content: [div, class]
         ```
         
+        > This feature overrides the normal practice of replacing the rendered content of a page.
+        
         ### Search index encryption
         
         > **Default value is "encrypted"**
         
         Related to [issue #13](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin/issues/13)
         
         > :warning: **The configuration mode "clear" of this functionality can cause DATA LEAK**
@@ -408,41 +450,47 @@
         > You have been warned 
         
         This feature allows you to control the behavior of the encryption plugin with the search index. 
         Three configuration modes are possible:
         
          * **clear** : Search index is not encrypted. Search is possible even on protected pages.
          * **dynamically** : Search index is encrypted on build. Search is possible once the pages have been decrypted.
-         * **encrypted** : Search index of encrypted pages is removed on build. Search is not possible on all encrypted pages.
+         * **encrypted** : Search index of encrypted pages is removed on build. Search is not possible on encrypted pages.
         
         You can set `search_index: '<mode_name>'` in your `mkdocs.yml` to change the search index encryption mode. Possible values are `clear`, `dynamically`, `encrypted`. The default mode is "**encrypted**".
         
         ```yaml
         plugins:
             - encryptcontent:
                 search_index: 'dynamically'
         ```
         
         This functionality modifies the search index created by the “search” plug-in.
-        Some themes might override the default “search” plug-in provided by mkdocs, but so far the structure of the `search/search_index.json` file is consistent.
+        Some themes might override the default search plug-in provided by mkdocs, 
+        but so far the structure of the `search/search_index.json` file is consistent.
         
         > The modification of the search index is carried out last (if `encryptcontent` is also last in `plugins`).
         > But always double-check the generated index after `mkdocs build` to see if your information is protected.
         
-        When the configuration mode is set to "**dynamically**", the [javascripts contribution files](https://github.com/unverbuggt/mkdocs-encryptcontent-plugin/tree/master/encryptcontent/contrib/templates/search)
-        are used to override the default search plugin files provided by MkDocs. They include a process of decrypting and keeping the search index in a SessionStorage.
+        When the configuration mode is set to "**dynamically**", the 
+        [javascripts contribution files](https://github.com/unverbuggt/mkdocs-encryptcontent-plugin/tree/master/encryptcontent/contrib/templates/search)
+        are used to override the default search plugin files provided by MkDocs. 
+        They include a process of decrypting and keeping the search index in a SessionStorage.
         
         ### Search index encryption for mkdocs-material
         
-        [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) uses a different search plugin that cannot "easily" be overridden like the default search plugin.
-        However this Plugin will still remove encrypted pages (`encrypted`) or encrypt the search entries (`dynamically`) for `mkdocs-material`.
+        [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) uses a different search plugin that
+        cannot "easily" be overridden like the default search plugin.
+        However this Plugin will still remove encrypted pages (`encrypted`) or encrypt the search entries (`dynamically`)
+        for `mkdocs-material`.
         
         In order to be able to decrypt the search index (`dynamically`) `mkdocs-material` needs to be customized (patched).
         
-        You'll need some [prerequisites](https://squidfunk.github.io/mkdocs-material/customization/#environment-setup) and also execute these commands:
+        You'll need some [prerequisites](https://squidfunk.github.io/mkdocs-material/customization/#environment-setup)
+        and also execute these commands:
         
         ```bash
         git clone https://github.com/squidfunk/mkdocs-material
         cd mkdocs-material
         pip install mkdocs-minify-plugin
         pip install mkdocs-redirects
         npm install
@@ -456,24 +504,33 @@
         
         > Note: this currently doesn't work with mkdocs-material-9.x.x
         
         ### Override default templates
         
         Related to [issue #32](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin/issues/32)
         
-        You can override the default templates with your own templates by providing an actual replacement path in the `html_template_path` *(HTML)* and `js_template_path` *(JS)* directives. Overridden templates **completely** replace the default templates. You **must** therefore copy the default templates to keep this module working.
+        You can override the default templates with your own templates by providing an actual replacement
+        path in the `html_template_path` *(HTML)* and `js_template_path` *(JS)* directives. 
+        Overridden templates **completely** replace the default templates. You **must** therefore copy the
+        default templates to keep this module working.
         
         ```yaml
         plugins:
             - encryptcontent:
                 html_template_path: "/root/real/path/mkdocs_poc/my_html_template.html"
                 js_template_path: "/root/real/path/mkdocs_poc/my_js_template.js"
+                input_class: 'md-search__form md-search__input'
+                button_class: 'md-search__icon'
         ```
         
-        When you overriding the default templates, you can add and use your own Jinja variables to condition and enrich your template, by defining `html_extra_vars` and `js_extra_vars` directives in key/value format. Added values can be used in your Jinja templates via the variable `extra`.
+        Use `input_class` and `button_class` to optionally set a CSS class for the password input field and the button.
+        
+        When you overriding the default templates, you can add and use your own Jinja variables to condition
+        and enrich your template, by defining `html_extra_vars` and `js_extra_vars` directives in key/value format.
+        Added values can be used in your Jinja templates via the variable `extra`.
         
         ```yaml
         plugins:
             - encryptcontent:
                 html_extra_vars:
                     my_extra: "extra value"
                     <key>: <value>
@@ -486,15 +543,17 @@
         
         ```jinja
         [ ... ] 
         <h2>{{ extra.my_extra }}</h2>
         [ ... ]
         ```
         
-        > **NOTE** You must avoid replacing/overwriting the variables used by default by this module. The limitations are the same as those of the jinja models. Issues related to template override will not be addressed.
+        > **NOTE** You must avoid replacing/overwriting the variables used by default by this module.
+        > The limitations are the same as those of the jinja models.
+        > Issues related to template override will not be addressed.
         
         ### Add button
         
         Add `password_button: True` in plugin configuration variable, to add button to the right of the password field.
         
         When enable, it allows to decrypt the content just like the classic keypress ENTER. If remember password feature is activated, use button to decrypt generate a 'relative' key on your local storage. You cannot use password button to create global password value.
         
@@ -524,42 +583,71 @@
         This feature now doesn't use JQuery anymore.
         
         It is also possible to reload a script id like `<script id="autoexec">console.log('test');</script>` that was encrypted within the page (related to [issue #30](https://github.com/unverbuggt/mkdocs-encryptcontent-plugin/issues/30)).
         
         ### Self-host crypto-js
         
         If you enable `selfhost` then you'll choose to upload crypto-js to your web server rather than using cloudflare CDN.
+        The self-host location is "SITE_URL/assets/javascripts/cryptojs/".
         
-        Additionally if you set `selfhost_download` then the required files will be downloaded **every time** on `mkdocs serve` or `mkdocs build`. 
-        Be aware that this costs additional build time and it is better to copy the files from `site/assets/javascripts/cryptojs/*` to `docs/assets/javascripts/cryptojs/*` to speed things up.
+        Additionally if you set `selfhost_download` then the required files will be automatically downloaded if needed.
+        The files are checked for their MD5 hash and saved to `docs_dir` or `selfhost_dir` (relative to `mkdocs.yml`).
         
         ```yaml
         plugins:
             - encryptcontent:
                 selfhost: true
                 selfhost_download: false
+                selfhost_dir: 'theme_overrides'
         ```
         
-        ### Translations
+        ### File name obfuscation
         
-        If the plugin is used in conjunction with the [static-i18n](https://ultrabug.github.io/mkdocs-static-i18n/) plugin you can provide `translations` for the used `i18n_page_file_locale`.
+        Imagine your pages contain many images and you labeled them "1.jpg", "2.jpg" and so on for some reason.
+        If you'd like to encrypt one of these pages, an attacker could try guessing the image file names
+        and would be able to download them despite not having the password to the page.
+        
+        This feature should make it impossible or at least way harder for an external attacker to guess the file names.
+        Please also check and disable directory listing for that matter.
+        Keep in mind that you hosting provider is still able to see all your images and files.
+        
+        To counter file name guessing you could active the feature like this:
         
         ```yaml
+        plugins:
             - encryptcontent:
-                #...
-                translations:
-                  de:
-                    title_prefix: '[Verschlüsselt] '
-                    summary: 'Der Inhalt dieser Seite ist mit AES verschlüsselt. '
-                    placeholder: 'Mit Strg+Enter wird das Passwort global gesetzt'
-                    password_button_text: 'Entschlüsseln'
-                    decryption_failure_message: 'Falsches passwort.'
-                    encryption_info_message: 'Bitte wenden Sie sich an den Systemadministrator um auf diese Seite zuzugreifen.'
-        ```
+                selfhost: true
+                selfhost_download: false
+                hash_filenames:
+                  extensions:
+                    - 'png'
+                    - 'jpg'
+                    - 'jpeg'
+                    - 'svg'
+                  except:
+                    - 'lilien.svg'
+        ```
+        
+        At `extensions` we define which file name extensions to obfuscate
+        (extension is taken from the part after the last ".",
+        so the extension of "image.jpg" is "jpg" and of "archive.tar.gz" is "gz").
+        
+        You can define multiple exceptions at the `except` list.
+        The file names that end with these strings will be skipped.
+        You should use this if some images are used by themes or other plugins.
+        Otherwise, you'd need to change these file names to the obfuscated ones.
+        
+        The file names are obfuscated in a way that the corresponding file is hashed with MD5
+        and the hash is added to the file name
+        (If the file content is not changed the file name also not changes), like this:
+        
+        some_image_1_bb80db433751833b8f8b4ad23767c0fc.jpg
+        ("bb80db433751833b8f8b4ad23767c0fc" being the MD5 hash of said image.)
         
+        > The file name obfuscation is currently applied to the whole site - not just the encrypted pages...
         
         # Contributing
         
         From reporting a bug to submitting a pull request: every contribution is appreciated and welcome.
         
         Report bugs, ask questions and request features using [Github issues][github-issues].
```

### Comparing `mkdocs-encryptcontent-plugin-2.4.5/README.md` & `mkdocs-encryptcontent-plugin-2.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,37 +20,43 @@
 >
 > If a password is defined in an article or a page, it is always used even if there is a global password.
 >
 > If a password is defined as an empty character string, the content is not protected.
 
 ![encryptcontent_demo](https://user-images.githubusercontent.com/12155947/177001700-f0920d4b-0c41-4d11-8164-9f63d29d8a6a.gif)
 
+# Todo for 2.6.x
+
+* Rework password handling or inventory of some sort
+* ...to be defined
 
 # Table of Contents
 
   * [Installation](#installation)
   * [Usage](#usage)
     * [Global password protection](#global-password-protection)
-    * [Secret from environment](#secret-from-environment) **(UPDATE)**
+    * [Secret from environment](#secret-from-environment)
     * [Customization](#default-vars-customization)
+    * [Translations](#translations)
+    * [Obfuscate pages](#obfuscate-pages) **NEW**
   * [Features](#features)
     * [HighlightJS support](#highlightjs-support) *(default)*
     * [Arithmatex support](#arithmatex-support) *(default)*
     * [Mermaid2 support](#mermaid-support) *(default)*
     * [Tag encrypted page](#tag-encrypted-page) *(default)*
     * [Remember password](#remember-password)
     * [Encrypt something](#encrypt-something)
-    * [Inject decrypt-form.tpl to theme](#inject-decrypt-formtpl-to-theme) **(NEW)**
+    * [Inject decrypt-form.tpl to theme](#inject-decrypt-formtpl-to-theme)
     * [Search index encryption](#search-index-encryption)
-    * [Search index encryption for mkdocs-material](#search-index-encryption-for-mkdocs-material) **(NEW)**
+    * [Search index encryption for mkdocs-material](#search-index-encryption-for-mkdocs-material)
     * [Override default templates](#override-default-templates)
     * [Add button](#add-button)
     * [Reload scripts](#reload-scripts)
-    * [Self-host crypto-js](#self-host-crypto-js) **(NEW)**
-    * [Translations](#translations) **(NEW)**
+    * [Self-host crypto-js](#self-host-crypto-js) *UPDATE*
+    * [File name obfuscation](#file-name-obfuscation) **NEW**
   * [Contributing](#contributing)
 
 
 # Installation
 
 Install the package with pip:
 
@@ -59,15 +65,15 @@
 ```
 
 Install the package from source with pip:
 
 ```bash
 cd mkdocs-encryptcontent-plugin/
 python setup.py sdist bdist_wheel
-pip install dist/mkdocs_encryptcontent_plugin-2.4.5-py3-none-any.whl
+pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.0-py3-none-any.whl
 ```
 
 Enable the plugin in your `mkdocs.yml`:
 
 ```yaml
 plugins:
     - search: {}
@@ -89,15 +95,16 @@
 plugins:
     - encryptcontent:
         global_password: 'your_password'
 ```
 
 If a password is defined in an article, it will **ALWAYS** overwrite the global password. 
 
-> **NOTE** Keep in mind that if the `password:` tag exists without value in an article, it will **not be protected** !
+> **NOTE** Keep in mind that if the `password:` tag exists without value in a page, it will **not be protected** !
+> Use this to **disable** `global_password` on specific pages.
 
 
 ### Secret from environment
 
 Instead of specifying a password in the mkdocs.yml file, you can use an environment variable to load your secret. 
 
 This process is in two steps:
@@ -114,28 +121,28 @@
 
 > **NOTE** Keep in mind that if the `use_secret:` configuration is set, it will always be used even if you have also set a global password with the `global_password` variable.
 >
 > If this environment variable is empty or missing, then the build will fail to prevent the unwanted leak of information.
 > However this can be converted into a warning by setting `ignore_missing_secret: true`. 
 > Use this only if you use a secret environment variable for production and a plain password for testing. You have been warned.
 
-> **NEW** The meta tag `use_secret` can also be set to achieve the same functionality on page level.
+> The meta tag `use_secret` can also be set to achieve the same functionality on page level.
 
 ### Default vars customization
 
 Optionally you can use some extra variables in plugin configuration to customize default messages.
 
 ```yaml
 plugins:
     - encryptcontent:
         title_prefix: '[LOCK]'
         summary: 'another informational message to encrypted content'
         placeholder: 'another password placeholder'
-        decryption_failure_message: 'another informational message when decryption fail'
-        encryption_info_message: 'another information message when you dont have acess !'
+        decryption_failure_message: 'another informational message when decryption fails'
+        encryption_info_message: "another information message when you don't have access !"
         input_class: 'md-search__form md-search__input'
         button_class: 'md-search__icon'
 ```
 
 Default prefix title is `[Protected]`.
 
 Default summary message is `This content is protected with AES encryption.`.
@@ -144,15 +151,46 @@
 
 Default decryption failure message is `Invalid password.`.
 
 Defaut encryption information message is `Contact your administrator for access to this page.`.
 
 > **NOTE** Adding a prefix to the title does not change the default navigation path !
 
-Use `input_class` and `button_class` to optionally set a CSS class for the password field and the button.
+### Translations
+
+If the plugin is used in conjunction with the [static-i18n](https://ultrabug.github.io/mkdocs-static-i18n/) plugin you can provide `translations` for the used `i18n_page_file_locale`.
+
+```yaml
+    - encryptcontent:
+        #...
+        translations:
+          de:
+            title_prefix: '[Verschlüsselt] '
+            summary: 'Der Inhalt dieser Seite ist mit AES verschlüsselt. '
+            placeholder: 'Mit Strg+Enter wird das Passwort global gesetzt'
+            password_button_text: 'Entschlüsseln'
+            decryption_failure_message: 'Falsches passwort.'
+            encryption_info_message: 'Bitte wenden Sie sich an den Systemadministrator um auf diese Seite zuzugreifen.'
+```
+
+#### Custom per-page strings
+
+You can set the  meta tag `encryption_summary` to customize `summary` and `encryption_info_message` on every page.
+
+### Obfuscate pages
+
+If you want to make it harder for search engines to scrape you pages content,
+you can set `obfuscate: SomeNotSoSecretPassword` meta tag in markdown.
+
+The page than will display `summary` and `encryption_info_message` together with a button labeled with.
+`password_button_text`. In order to view the pages content one hast to press the button first.
+
+If a `password` or `use_secret` is set, then the `obfuscate` feature will be disabled.
+If you want to use `obfuscate` in a configuration where `global_password` is defined, 
+you'll need to set `password:` meta tag (with no password defined) to undefine the password on this page.
 
 # Features
 
 ### HighlightJS support
 
 > **Enable by default**
 
@@ -208,16 +246,15 @@
 
 > **Enable by default**
 
 Related to [issue #7](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin/issues/7)
 
 This feature add an additional attribute `encrypted` with value `True` to the mkdocs type `mkdocs.nav.page` object.
 
-You can add `tag_encrypted_page: False` in plugin configuration, to disable tagging of encrypted pages. **BUT** This feature is neccessary for others feature working correctly. 
-If you disable this feature, f.ex. [Encrypt something](#encrypt-something) and [Search index encryption](#search-index-encryption) won't work.
+You can add `tag_encrypted_page: False` in plugin configuration, to disable tagging of encrypted pages. 
 
 When enable, it becomes possible to use `encrypted` attribute in the jinja template of your theme, as a condition to perform custom modification.
 
 ```jinja
 {%- for nav_item in nav %}
     {% if nav_item.encrypted %}
         <!-- Do something --> 
@@ -245,37 +282,39 @@
 When enabled, each time you fill password form and press `Enter` a key on session storage is create with your password
 as value. When you reload the page, if you already have an 'encryptcontent' key in the session storage of your browser,
 the page will be automatically decrypted using the value previously created.
 
 By default, the key is created with a name relative to the page on which it was generated.
 This 'relative' key will always be used as first attempt to decrypt the current page when loading.
 
-If your password is a [global password](#global-password-protection), you can fill in the form field  `mkdocs-content-password`, then use the keyboard shortcut `CTRL + ENTER` instead of the classic `ENTER`. 
+If your password is a [global password](#global-password-protection), you can fill in the form
+field  `mkdocs-content-password`, then use the keyboard shortcut `CTRL + ENTER` instead of the classic `ENTER`. 
 The key that will be created with a generic name to making it accessible, by default, on all the pages of your site.
 
 The form of decryption remains visible as long as the content has not been successfully decrypted, which allows in case of error to retry. 
 All keys created with this feature on sessionStorage/localStorage have an default expire time daly set to 24 hours, just cause ...
 
 However *(optionally)*, its possible to change the default expire time by setting options `default_expire_delay: <number>` in your `mkdocs.yml`. Your configuration should look like this when you enabled this feature :
 ```yaml
 plugins:
     - encryptcontent:
         remember_password: True
         default_expire_delay: 24   # <-- Default expire delay in hours (optional)
 ```
 
-> **NOTE** The expired elements of the localStorage are only deleted by the execution of the decrypt-content.js scripts and therefore by the navigation on the site. Secret items can therefore remain visible in local storage after their expiration dates. 
-> Now The default is to use sessionStorage instead of localStorage, so the browser forgets the password after the current tab was closed. However it can be set to use localStorage by setting `session_storage: False`
+> **NOTE** The expired elements of the localStorage are only deleted by the execution of the decrypt-content.js
+> scripts and therefore by the navigation on the site. Secret items can therefore remain visible in local storage
+> after their expiration dates. 
+> Now The default is to use sessionStorage instead of localStorage, so the browser forgets the password after
+> the current tab was closed. However it can be set to use localStorage by setting `session_storage: False`
 
 ### Encrypt something
 
 Related to [issue #9](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin/issues/9)
 
-The [tag encrypted page feature](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin#tag-encrypted-page) **MUST** be enabled (it's default) for this feature to work properly.
-
 Add `encrypted_something: {}` in the plugin configuration variable, to encrypt something else.
 
 The syntax of this new variable **MUST** follow the yaml format of a dictionary. 
 Child elements of `encrypted_something` are build with a key `<unique name>` in string format and a list as value. 
 The list have to be contructed with the name of an HTML element `<html tag>` as first item and `id` or `class` as the second item.
 
 ```yaml
@@ -319,15 +358,15 @@
 ```yaml
 plugins:
     - encryptcontent:
         encrypted_something:
             mkdocs-encrypted-toc: [div, id]
 ```
 
-2. Other example, with multiples target. In you Material Theme, you want to encrypt ToC content and Footer.
+2. Other example, with multiples target. In your custom Material theme, you want to encrypt ToC content and Footer.
 
 Materiel generate 2 `<nav>` structure with the same template `toc.html`, so you need to use a `class` instead of an id for this part.
 The footer part, is generated by the `footer.html` template in a classic div so an `id` is sufficient
 
 After modification, your template looks like this :
 ```jinja (toc.html)
 <nav class="md-nav md-nav--secondary {% if page.encrypted %}mkdocs-encrypted-toc{% endif %}" aria-label="{{ lang.t('toc.title') }}">
@@ -338,25 +377,26 @@
 ```jinja (footer.html)
 <footer class="md-footer">
     <div class="md-footer-nav" {% if page.encrypted %}id="mkdocs-encrypted-footer"{% endif %}> ... </div>
     <div class="md-footer-meta md-typeset" {% if page.encrypted %}id="mkdocs-encrypted-footer-meta"{% endif %}>
 </footer>
 ```
 
-Your configuration like this :
+Your configuration would look like this :
 ```yaml
 plugins:
     - encryptcontent:
         encrypted_something:
             mkdocs-encrypted-toc: [nav, class]
             mkdocs-encrypted-footer: [div, id]
             mkdocs-encrypted-footer-meta: [div, id]
 ```
 
-3. If you are using mkdocs-material, then this example will also encrypt menu, toc and footer
+3. If you are using unmodified mkdocs-material, then this example will encrypt menu, toc and footer
+But you'd need the Navigation pruning feature to hide the title of encrypted pages from navigation (or see 2.).
 
 ```yaml
 plugins:
     - encryptcontent:
         encrypted_something:
             md-footer__inner: [nav, class]
             md-nav: [nav, class]
@@ -383,14 +423,16 @@
         encrypted_something:
             md-footer__inner: [nav, class] #Footer
             md-nav: [nav, class] #Menu and toc
         inject:
             md-content: [div, class]
 ```
 
+> This feature overrides the normal practice of replacing the rendered content of a page.
+
 ### Search index encryption
 
 > **Default value is "encrypted"**
 
 Related to [issue #13](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin/issues/13)
 
 > :warning: **The configuration mode "clear" of this functionality can cause DATA LEAK**
@@ -400,41 +442,47 @@
 > You have been warned 
 
 This feature allows you to control the behavior of the encryption plugin with the search index. 
 Three configuration modes are possible:
 
  * **clear** : Search index is not encrypted. Search is possible even on protected pages.
  * **dynamically** : Search index is encrypted on build. Search is possible once the pages have been decrypted.
- * **encrypted** : Search index of encrypted pages is removed on build. Search is not possible on all encrypted pages.
+ * **encrypted** : Search index of encrypted pages is removed on build. Search is not possible on encrypted pages.
 
 You can set `search_index: '<mode_name>'` in your `mkdocs.yml` to change the search index encryption mode. Possible values are `clear`, `dynamically`, `encrypted`. The default mode is "**encrypted**".
 
 ```yaml
 plugins:
     - encryptcontent:
         search_index: 'dynamically'
 ```
 
 This functionality modifies the search index created by the “search” plug-in.
-Some themes might override the default “search” plug-in provided by mkdocs, but so far the structure of the `search/search_index.json` file is consistent.
+Some themes might override the default search plug-in provided by mkdocs, 
+but so far the structure of the `search/search_index.json` file is consistent.
 
 > The modification of the search index is carried out last (if `encryptcontent` is also last in `plugins`).
 > But always double-check the generated index after `mkdocs build` to see if your information is protected.
 
-When the configuration mode is set to "**dynamically**", the [javascripts contribution files](https://github.com/unverbuggt/mkdocs-encryptcontent-plugin/tree/master/encryptcontent/contrib/templates/search)
-are used to override the default search plugin files provided by MkDocs. They include a process of decrypting and keeping the search index in a SessionStorage.
+When the configuration mode is set to "**dynamically**", the 
+[javascripts contribution files](https://github.com/unverbuggt/mkdocs-encryptcontent-plugin/tree/master/encryptcontent/contrib/templates/search)
+are used to override the default search plugin files provided by MkDocs. 
+They include a process of decrypting and keeping the search index in a SessionStorage.
 
 ### Search index encryption for mkdocs-material
 
-[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) uses a different search plugin that cannot "easily" be overridden like the default search plugin.
-However this Plugin will still remove encrypted pages (`encrypted`) or encrypt the search entries (`dynamically`) for `mkdocs-material`.
+[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) uses a different search plugin that
+cannot "easily" be overridden like the default search plugin.
+However this Plugin will still remove encrypted pages (`encrypted`) or encrypt the search entries (`dynamically`)
+for `mkdocs-material`.
 
 In order to be able to decrypt the search index (`dynamically`) `mkdocs-material` needs to be customized (patched).
 
-You'll need some [prerequisites](https://squidfunk.github.io/mkdocs-material/customization/#environment-setup) and also execute these commands:
+You'll need some [prerequisites](https://squidfunk.github.io/mkdocs-material/customization/#environment-setup)
+and also execute these commands:
 
 ```bash
 git clone https://github.com/squidfunk/mkdocs-material
 cd mkdocs-material
 pip install mkdocs-minify-plugin
 pip install mkdocs-redirects
 npm install
@@ -448,24 +496,33 @@
 
 > Note: this currently doesn't work with mkdocs-material-9.x.x
 
 ### Override default templates
 
 Related to [issue #32](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin/issues/32)
 
-You can override the default templates with your own templates by providing an actual replacement path in the `html_template_path` *(HTML)* and `js_template_path` *(JS)* directives. Overridden templates **completely** replace the default templates. You **must** therefore copy the default templates to keep this module working.
+You can override the default templates with your own templates by providing an actual replacement
+path in the `html_template_path` *(HTML)* and `js_template_path` *(JS)* directives. 
+Overridden templates **completely** replace the default templates. You **must** therefore copy the
+default templates to keep this module working.
 
 ```yaml
 plugins:
     - encryptcontent:
         html_template_path: "/root/real/path/mkdocs_poc/my_html_template.html"
         js_template_path: "/root/real/path/mkdocs_poc/my_js_template.js"
+        input_class: 'md-search__form md-search__input'
+        button_class: 'md-search__icon'
 ```
 
-When you overriding the default templates, you can add and use your own Jinja variables to condition and enrich your template, by defining `html_extra_vars` and `js_extra_vars` directives in key/value format. Added values can be used in your Jinja templates via the variable `extra`.
+Use `input_class` and `button_class` to optionally set a CSS class for the password input field and the button.
+
+When you overriding the default templates, you can add and use your own Jinja variables to condition
+and enrich your template, by defining `html_extra_vars` and `js_extra_vars` directives in key/value format.
+Added values can be used in your Jinja templates via the variable `extra`.
 
 ```yaml
 plugins:
     - encryptcontent:
         html_extra_vars:
             my_extra: "extra value"
             <key>: <value>
@@ -478,15 +535,17 @@
 
 ```jinja
 [ ... ] 
 <h2>{{ extra.my_extra }}</h2>
 [ ... ]
 ```
 
-> **NOTE** You must avoid replacing/overwriting the variables used by default by this module. The limitations are the same as those of the jinja models. Issues related to template override will not be addressed.
+> **NOTE** You must avoid replacing/overwriting the variables used by default by this module.
+> The limitations are the same as those of the jinja models.
+> Issues related to template override will not be addressed.
 
 ### Add button
 
 Add `password_button: True` in plugin configuration variable, to add button to the right of the password field.
 
 When enable, it allows to decrypt the content just like the classic keypress ENTER. If remember password feature is activated, use button to decrypt generate a 'relative' key on your local storage. You cannot use password button to create global password value.
 
@@ -516,42 +575,71 @@
 This feature now doesn't use JQuery anymore.
 
 It is also possible to reload a script id like `<script id="autoexec">console.log('test');</script>` that was encrypted within the page (related to [issue #30](https://github.com/unverbuggt/mkdocs-encryptcontent-plugin/issues/30)).
 
 ### Self-host crypto-js
 
 If you enable `selfhost` then you'll choose to upload crypto-js to your web server rather than using cloudflare CDN.
+The self-host location is "SITE_URL/assets/javascripts/cryptojs/".
 
-Additionally if you set `selfhost_download` then the required files will be downloaded **every time** on `mkdocs serve` or `mkdocs build`. 
-Be aware that this costs additional build time and it is better to copy the files from `site/assets/javascripts/cryptojs/*` to `docs/assets/javascripts/cryptojs/*` to speed things up.
+Additionally if you set `selfhost_download` then the required files will be automatically downloaded if needed.
+The files are checked for their MD5 hash and saved to `docs_dir` or `selfhost_dir` (relative to `mkdocs.yml`).
 
 ```yaml
 plugins:
     - encryptcontent:
         selfhost: true
         selfhost_download: false
+        selfhost_dir: 'theme_overrides'
 ```
 
-### Translations
+### File name obfuscation
 
-If the plugin is used in conjunction with the [static-i18n](https://ultrabug.github.io/mkdocs-static-i18n/) plugin you can provide `translations` for the used `i18n_page_file_locale`.
+Imagine your pages contain many images and you labeled them "1.jpg", "2.jpg" and so on for some reason.
+If you'd like to encrypt one of these pages, an attacker could try guessing the image file names
+and would be able to download them despite not having the password to the page.
+
+This feature should make it impossible or at least way harder for an external attacker to guess the file names.
+Please also check and disable directory listing for that matter.
+Keep in mind that you hosting provider is still able to see all your images and files.
+
+To counter file name guessing you could active the feature like this:
 
 ```yaml
+plugins:
     - encryptcontent:
-        #...
-        translations:
-          de:
-            title_prefix: '[Verschlüsselt] '
-            summary: 'Der Inhalt dieser Seite ist mit AES verschlüsselt. '
-            placeholder: 'Mit Strg+Enter wird das Passwort global gesetzt'
-            password_button_text: 'Entschlüsseln'
-            decryption_failure_message: 'Falsches passwort.'
-            encryption_info_message: 'Bitte wenden Sie sich an den Systemadministrator um auf diese Seite zuzugreifen.'
-```
+        selfhost: true
+        selfhost_download: false
+        hash_filenames:
+          extensions:
+            - 'png'
+            - 'jpg'
+            - 'jpeg'
+            - 'svg'
+          except:
+            - 'lilien.svg'
+```
+
+At `extensions` we define which file name extensions to obfuscate
+(extension is taken from the part after the last ".",
+so the extension of "image.jpg" is "jpg" and of "archive.tar.gz" is "gz").
+
+You can define multiple exceptions at the `except` list.
+The file names that end with these strings will be skipped.
+You should use this if some images are used by themes or other plugins.
+Otherwise, you'd need to change these file names to the obfuscated ones.
+
+The file names are obfuscated in a way that the corresponding file is hashed with MD5
+and the hash is added to the file name
+(If the file content is not changed the file name also not changes), like this:
+
+some_image_1_bb80db433751833b8f8b4ad23767c0fc.jpg
+("bb80db433751833b8f8b4ad23767c0fc" being the MD5 hash of said image.)
 
+> The file name obfuscation is currently applied to the whole site - not just the encrypted pages...
 
 # Contributing
 
 From reporting a bug to submitting a pull request: every contribution is appreciated and welcome.
 
 Report bugs, ask questions and request features using [Github issues][github-issues].
```

### Comparing `mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/contrib/templates/search/lunr.js` & `mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/lunr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/contrib/templates/search/main.js` & `mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/main.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/contrib/templates/search/worker.js` & `mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/contrib/templates/search/worker.js`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/decrypt-contents.tpl.js` & `mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/decrypt-contents.tpl.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -399,15 +399,17 @@
     }
 }
 
 /* Trigger decryption process */
 function init_decryptor() {
     var password_input = document.getElementById('mkdocs-content-password');
     // adjust password field width to placeholder length
-    password_input.setAttribute('size', password_input.getAttribute('placeholder').length);
+    if (password_input.hasAttribute('placeholder')) {
+        password_input.setAttribute('size', password_input.getAttribute('placeholder').length);
+    }
     var encrypted_content = document.getElementById('mkdocs-encrypted-content');
     var decrypted_content = document.getElementById('mkdocs-decrypted-content'); {
         %
         if remember_password - %
     }
     /* If remember_password is set, try to use sessionStorage/localstorage item to decrypt content when page is loaded */
     let password_cookie = getItemExpiry(encryptcontent_path);
```

### Comparing `mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/decrypt-form.tpl.html` & `mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/decrypt-form.tpl.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 <div id="mkdocs-encrypted-content" style="display:none">{{ ciphertext_bundle }}</div>
 <div id="mkdocs-decrypted-content">
     <form id="mkdocs-decrypt-form">
         <h1>{{ summary }}</h1>
         {% if encryption_info_message %}<p>{{ encryption_info_message }}</p>{% endif %}
+        {%- if obfuscate %}
+        <input type="hidden" id="mkdocs-content-password" value="{{ obfuscate_password }}" />
+        {%- else %}
         <input{% if input_class %} class="{{ input_class }}"{% endif %} type="password" id="mkdocs-content-password" placeholder="{{ placeholder }}" />
+        {%- endif %}
         {% if password_button %}<button{% if button_class %} class="{{ button_class }}"{% endif %} id="mkdocs-decrypt-button">{{ password_button_text }}</button>{% endif %}
         <p id="mkdocs-decrypt-msg"></p>
     </form>
 </div>
 
 <script type="text/javascript">
 var encryptcontent_path = "{{ encryptcontent_path }}";
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {{ ciphertext_bundle }}
 ****** {{ summary }} ******
 {% if encryption_info_message %}
 {{ encryption_info_message }}
-{% endif %}
+{% endif %} {%- if obfuscate %}  {%- else %}
 % if input_class %} class="{{ input_class }}"{% endif %} type="password"
-id="mkdocs-content-password" placeholder="{{ placeholder }}" /> {% if
-password_button %}
+id="mkdocs-content-password" placeholder="{{ placeholder }}" /> {%- endif %} {%
+if password_button %}
 % if button_class %} class="{{ button_class }}"{% endif %} id="mkdocs-decrypt-
 button">{{ password_button_text }}{% endif %}
  {% for library in js_libraries %}
  {%- endfor %}
```

### Comparing `mkdocs-encryptcontent-plugin-2.4.5/encryptcontent/plugin.py` & `mkdocs-encryptcontent-plugin-2.5.0/encryptcontent/plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
 import os
 import re
 import base64
 import hashlib
 import logging
 import json
+import math
 from pathlib import Path
+from os.path import exists
 from Crypto import Random
 from jinja2 import Template
 from Crypto.Cipher import AES
 from bs4 import BeautifulSoup
 from mkdocs.plugins import BasePlugin
 from mkdocs.config import config_options
 from urllib.parse import urlsplit
@@ -17,20 +19,20 @@
 
 try:
     from mkdocs.utils import string_types
 except ImportError:
     string_types = str
 
 JS_LIBRARIES = [
-    '//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/core.js',
-    '//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/enc-base64.js',
-    '//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/cipher-core.js',
-    '//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/pad-nopadding.js',
-    '//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/md5.js',
-    '//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/aes.js'
+    ['//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/core.js','b55ae8027253d4d54c4f1ef3b6254646'],
+    ['//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/enc-base64.js','f551ce1340a86e5edbfef4a6aefa798f'],
+    ['//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/cipher-core.js','dfddc0e33faf7a794e0c3c140544490e'],
+    ['//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/pad-nopadding.js','e288e14e2cd299c3247120114e1178e6'],
+    ['//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/md5.js','349498f298a6e6e6a85789d637e89109'],
+    ['//cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/aes.js','da81b91b1b57c279c29b3469649d9b86'],
 ]
 
 PLUGIN_DIR = os.path.dirname(os.path.realpath(__file__))
 
 SETTINGS = {
     'title_prefix': '[Protected] ',
     'summary': 'This content is protected with AES encryption. ',
@@ -58,15 +60,14 @@
         ('password_button', config_options.Type(bool, default=False)),
         ('input_class', config_options.Type(string_types, default=None)),
         ('button_class', config_options.Type(string_types, default=None)),
         # password feature
         ('global_password', config_options.Type(string_types, default=None)),
         ('use_secret', config_options.Type(string_types, default=None)),
         ('ignore_missing_secret', config_options.Type(bool, default=False)),
-        ('password', config_options.Type(string_types, default=None)),
         ('remember_password', config_options.Type(bool, default=False)),
         ('session_storage', config_options.Type(bool, default=True)),
         ('default_expire_delay', config_options.Type(int, default=int(24))),
         # default features enabled
         ('arithmatex', config_options.Type(bool, default=True)),
         ('hljs', config_options.Type(bool, default=True)),
         ('mermaid2', config_options.Type(bool, default=True)),
@@ -79,27 +80,50 @@
         # others features
         ('encrypted_something', config_options.Type(dict, default={})),
         ('search_index', config_options.Choice(('clear', 'dynamically', 'encrypted'), default='encrypted')),
         ('reload_scripts', config_options.Type(list, default=[])),
         ('inject', config_options.Type(dict, default={})),
         ('selfhost', config_options.Type(bool, default=False)),
         ('selfhost_download', config_options.Type(bool, default=True)),
+        ('selfhost_dir', config_options.Type(string_types, default='')),
         ('translations', config_options.Type(dict, default={}, required=False)),
+        ('hash_filenames', config_options.Type(dict, default={}, required=False)),
         # legacy features, doesn't exist anymore
-        ('disable_cookie_protection', config_options.Type(bool, default=False)),
-        ('decrypt_search', config_options.Type(bool, default=False)),
-        ('experimental', config_options.Type(bool, default=False)),
     )
 
+    setup = {}
+
     def __hash_md5__(self, text):
         """ Creates an md5 hash from text. """
         key = hashlib.md5()
         key.update(text.encode('utf-8'))
         return key.digest()
 
+    def __hash_md5_file__(self, fname):
+        hash_md5 = hashlib.md5()
+        with open(fname, "rb") as f:
+            for chunk in iter(lambda: f.read(4096), b""):
+                hash_md5.update(chunk)
+        return hash_md5.hexdigest()
+
+    def __download_and_check__(self, filename, url, hash):
+        hash_md5 = hashlib.md5()
+        if not exists(filename):
+            with urlopen(url) as response:
+                filecontent = response.read()
+                hash_md5.update(filecontent)
+                hash_check = hash_md5.hexdigest()
+                if hash == hash_check:
+                    with open(filename, 'wb') as file:
+                        file.write(filecontent)
+                        logger.info('Downloaded external asset "' + filename.name + '"')
+                else:
+                    logger.error('Error downloading asset "' + filename.name + '" hash mismatch!')
+                    os._exit(1)
+
     def __encrypt_text_aes__(self, text, password):
         """ Encrypts text with AES-256. """
         BLOCK_SIZE = 32
         PADDING_CHAR = b'^'
         iv = Random.new().read(16)
         # key must be 32 bytes for AES-256, so the password is hashed with md5 first
         cipher = AES.new(self.__hash_md5__(password), AES.MODE_CBC, iv)
@@ -109,86 +133,134 @@
         ciphertext = cipher.encrypt(plaintext_padded)
         return (
             base64.b64encode(iv),
             base64.b64encode(ciphertext),
             PADDING_CHAR
         )
 
-    def __encrypt_content__(self, content, password, base_path, encryptcontent_path):
+    def __encrypt_content__(self, content, base_path, encryptcontent_path, encryptcontent):
         """ Replaces page or article content with decrypt form. """
-        ciphertext_bundle = self.__encrypt_text_aes__(content, password)
+        ciphertext_bundle = self.__encrypt_text_aes__(content, encryptcontent['password'])
 
         # optionally selfhost cryptojs
-        if self.config["selfhost"]:
-            js_libraries = []
-            for jsurl in JS_LIBRARIES:
-                js_libraries.append(base_path + 'assets/javascripts/cryptojs/' + jsurl.rsplit('/',1)[1])
+        js_libraries = []
+        for jsurl in JS_LIBRARIES:
+            if self.config["selfhost"]:
+                js_libraries.append(base_path + 'assets/javascripts/cryptojs/' + jsurl[0].rsplit('/',1)[1])
+            else:
+                js_libraries = jsurl[0]
+
+        obfuscate = encryptcontent.get('obfuscate')
+        if obfuscate:
+            obfuscate_password = encryptcontent['password']
         else:
-            js_libraries = JS_LIBRARIES
+            obfuscate_password = None
 
-        decrypt_form = Template(self.config['html_template']).render({
+        decrypt_form = Template(self.setup['html_template']).render({
             # custom message and template rendering
-            'summary': self.config['summary'],
-            'placeholder': self.config['placeholder'],
+            'summary': encryptcontent['summary'],
+            'placeholder': encryptcontent['placeholder'],
             'password_button': self.config['password_button'],
-            'password_button_text': self.config['password_button_text'],
-            'encryption_info_message': self.config['encryption_info_message'],
-            'decryption_failure_message': json.dumps(self.config['decryption_failure_message']),
+            'password_button_text': encryptcontent['password_button_text'],
+            'encryption_info_message': encryptcontent['encryption_info_message'],
+            'decryption_failure_message': json.dumps(encryptcontent['decryption_failure_message']),
             'input_class': self.config['input_class'],
             'button_class': self.config['button_class'],
+            'obfuscate': obfuscate,
+            'obfuscate_password': obfuscate_password,
             # this benign decoding is necessary before writing to the template,
             # otherwise the output string will be wrapped with b''
             'ciphertext_bundle': b';'.join(ciphertext_bundle).decode('ascii'),
             'js_libraries': js_libraries,
             'base_path': base_path,
             'encryptcontent_path': encryptcontent_path,
             # add extra vars
             'extra': self.config['html_extra_vars']
         })
         return decrypt_form
 
     def __generate_decrypt_js__(self):
         """ Generate JS file with enable feature. """
-        decrypt_js = Template(self.config['js_template']).render({
+        decrypt_js = Template(self.setup['js_template']).render({
             # custom message and template rendering
             'password_button': self.config['password_button'],
             # enable / disable features
             'arithmatex': self.config['arithmatex'],
             'hljs': self.config['hljs'],
             'mermaid2': self.config['mermaid2'],
             'remember_password': self.config['remember_password'],
             'session_storage': self.config['session_storage'],
             'default_expire_delay': int(self.config['default_expire_delay']),
-            'encrypted_something': self.config['encrypted_something'],
+            'encrypted_something': self.setup['encrypted_something'],
             'reload_scripts': self.config['reload_scripts'],
             'experimental': self.config['search_index'] == 'dynamically',
-            'site_path': self.config['site_path'],
+            'site_path': self.setup['site_path'],
             # add extra vars
             'extra': self.config['js_extra_vars']
         })
         return decrypt_js
 
+    def __get_entropy_from_password__(self, password):
+        #          123456789012345678901234567890
+        lcase =   "abcdefghijklmnopqrstuvwxyz"
+        ucase =   "ABCDEFGHIJKLMNOPQRTSUVWXYZ"
+        number =  "0123456789"
+        special = "!*#,;?+-_.=~^%()[]{}|:/"
+        other = ""
+        lcase_used = False
+        ucase_used = False
+        number_used = False
+        special_used = False
+        other_used = 0
+        for character in password:
+            if character in lcase:
+                lcase_used = True
+            elif character in ucase:
+                ucase_used = True
+            elif character in number:
+                number_used = True
+            elif character in special:
+                special_used = True
+            elif character not in other:
+                other_used += 1
+                other += character
+        ent = 0
+        if lcase_used:
+            ent += len(lcase)
+        if ucase_used:
+            ent += len(ucase)
+        if number_used:
+            ent += len(number)
+        if special_used:
+            ent += len(special)
+        ent += other_used
+        ent_max = len(lcase) + len(ucase) + len(number) + len(special) + len(other)
+        enttropy_spied_on = math.log( pow(ent, len(password)) ) / math.log(2)
+        enttropy_secret = math.log( pow(ent_max, len(password)) ) / math.log(2)
+        return enttropy_spied_on, enttropy_secret
+
     # MKDOCS Events builds
 
     def on_config(self, config, **kwargs):
         """
         The config event is the first event called on build and is run immediately after the user
         configuration is loaded and validated. Any alterations to the config should be made here.
         Configure plugin self.config from configuration file (mkdocs.yml)
 
         :param config: global configuration object (mkdocs.yml)
         :return: global configuration object modified to include templates files
         """
         # Override default template
         logger.debug('Load HTML template from file: "{file}".'.format(file=str(self.config['html_template_path'])))
         with open(self.config['html_template_path'], 'r') as template_html:
-            self.config['html_template'] = template_html.read()
+            self.setup['html_template'] = template_html.read()
         logger.debug('Load JS template from file: "{file}".'.format(file=str(self.config['js_template_path'])))
         with open(self.config['js_template_path'], 'r') as template_js:
-            self.config['js_template'] = template_js.read()
+            self.setup['js_template'] = template_js.read()
+
         # Optionnaly use Github secret
         if self.config.get('use_secret'):
             if os.environ.get(str(self.config['use_secret'])):
                 self.config['global_password'] = os.environ.get(str(self.config['use_secret']))
             else:
                 if self.config['ignore_missing_secret'] and self.config['global_password']:
                     logger.warning('Cannot get global password from environment variable: {var}. Using global_password as fallback!'.format(
@@ -222,38 +294,38 @@
             logger.debug('"mermaid2" value detected on extensions config, enable rendering after decryption.')
             self.config['mermaid2'] = True
         else:
             logger.info('"mermaid2" feature is disabled in your plugin configuration.')
             self.config['mermaid2'] = False
         # Warn about deprecated features on Vervion 2.0.0
         deprecated_options_detected = False
-        if self.config.get('disable_cookie_protection'):
-            logger.warning('DEPRECATED: Feature "disable_cookie_protection" is no longer supported. Can by remove.')
-            deprecated_options_detected = True
-        if self.config.get('decrypt_search'):
-            logger.warning('DEPRECATED: Feature "decrypt_search" is no longer supported. Use search_index on "clear" mode instead.')
-            deprecated_options_detected = True
-            logger.info('Fallback "decrypt_search" configuraiton to "search_index" mode clear.')
-            self.config['search_index'] = 'clear'
+
         if deprecated_options_detected:
             logger.warning('DEPRECATED: Features marked as deprecated will be remove in next minor version !')
-        # Re order plugins to be sure search-index are not encrypted
-        if self.config['search_index'] == 'clear':
-            logger.debug('Reordering plugins loading and put search and encryptcontent at the end of the event pipe.')
-            try: #PluginCollection is no instance of OrderedDict anymore since MkDocs 1.4
-                config['plugins'].move_to_end('search')
-                config['plugins'].move_to_end('encryptcontent')
-            except:
-                logger.warning('Could not reorder plugins. Please check that "search" and "encryptcontent" are at the end of plugins')
         # Enable experimental code .. :popcorn:
         elif self.config['search_index'] == 'dynamically':
             logger.info("EXPERIMENTAL search index encryption enabled.")
-        self.config['encrypted_something'] = {**self.config['inject'], **self.config['encrypted_something']} #add inject to encrypted_something
+        self.setup['encrypted_something'] = {**self.config['inject'], **self.config['encrypted_something']} #add inject to encrypted_something
         # Get path to site in case of subdir in site_url
-        self.config['site_path'] = urlsplit(config.data["site_url"] or '/').path[1::]
+        self.setup['site_path'] = urlsplit(config.data["site_url"] or '/').path[1::]
+
+        self.setup['search_plugin_found'] = False
+        encryptcontent_plugin_found = False
+        for plugin in config['plugins']:
+            if plugin.endswith('search'):
+                if encryptcontent_plugin_found:
+                    logger.error('Plugins need to be reordered ("search" ahead of "encryptcontent" in the end)! Otherwise search index might leak sensitive data.')
+                    os._exit(1) # prevent build without search index modification
+                self.setup['search_plugin_found'] = True
+            if plugin == 'encryptcontent':
+                encryptcontent_plugin_found = True
+        if not self.setup['search_plugin_found']:
+            logger.warning('"search" plugin wasn\'t enabled. Search index isn\'t generated or modified.')
+
+        self.setup['locations'] = {}
 
     def on_pre_build(self, config, **kwargs):
         """
         The pre_build event does not alter any variables. Use this event to call pre-build scripts.
         Overwrite default mkdocs-search contrib plugin with experimental one for work with
         encrypted search index.
 
@@ -277,52 +349,100 @@
                             config['theme'].dirs.append(path)
                             if 'search/main.js' not in config['extra_javascript']:
                                 config['extra_javascript'].append('search/main.js')
                             break
         except Exception as exp:
             logger.exception(exp)
 
+    def on_files(self, files, config, **kwargs):
+        """
+        The files event is called after the files collection is populated from the docs_dir.
+        Use this event to add, remove, or alter files in the collection.
+        Note that Page objects have not yet been associated with the file objects in the collection.
+        Use Page Events to manipulate page specific data.
+        """
+        if 'extensions' in self.config['hash_filenames']:
+            for file in files:
+
+                if 'except' in self.config['hash_filenames']:
+                    skip = False
+                    for check in self.config['hash_filenames']['except']:
+                        if file.src_path.endswith(check):
+                            skip = True
+                    if skip:
+                        continue
+
+                ext = file.src_path.rsplit('.',1)[1].lower()
+                if ext in self.config['hash_filenames']['extensions']:
+                    hash = self.__hash_md5_file__(file.abs_src_path)
+                    filename, ext =  file.abs_dest_path.rsplit('.',1)
+                    filename = filename + "_" + hash
+                    file.abs_dest_path = filename + "." + ext
+                    filename, ext =  file.url.rsplit('.',1)
+                    filename = filename + "_" + hash
+                    file.url = filename + "." + ext
+
     def on_page_markdown(self, markdown, page, config, **kwargs):
         """
         The page_markdown event is called after the page's markdown is loaded from file and
         can be used to alter the Markdown source text. The meta- data has been stripped off
         and is available as page.meta at this point.
         Load password from meta header *.md pages and override global_password if defined.
 
         :param markdown: Markdown source text of page as string
         :param page: mkdocs.nav.Page instance
         :param config: global configuration object
         :param site_navigation: global navigation object
         :return: Markdown source text of page as string
         """
 
+        encryptcontent = {} #init page data dict
+
         # Set global password as default password for each page
-        self.config['password'] = self.config['global_password']
+        encryptcontent['password'] = self.config['global_password']
 
         if 'password' in page.meta.keys():
             # If global_password is set, but you don't want to encrypt content
             page_password = str(page.meta.get('password'))
-            self.config['password'] = None if page_password == '' else page_password
+            encryptcontent['password'] = None if page_password == '' else page_password
             # Delete meta password information before rendering to avoid leak :]
             del page.meta['password']
 
         if 'use_secret' in page.meta.keys():
             if os.environ.get(str(page.meta.get('use_secret'))):
-                self.config['password'] = os.environ.get(str(page.meta.get('use_secret')))
+                encryptcontent['password'] = os.environ.get(str(page.meta.get('use_secret')))
             else:
-                if self.config['ignore_missing_secret'] and self.config['password']:
+                if self.config['ignore_missing_secret'] and encryptcontent['password']:
                     logger.warning('Cannot get password for "{page}" from environment variable: {var}. Using password from config or meta key as fallback!'.format(
                         var=str(page.meta.get('use_secret')), page=page.title)
                     )
                 else:
                     logger.error('Cannot get password for "{page}" from environment variable: {var}. Abort !'.format(
                         var=str(page.meta.get('use_secret')), page=page.title)
                     )
                     os._exit(1)                                 # prevent build without password to avoid leak0
 
+        if 'obfuscate' in page.meta.keys():
+            if encryptcontent['password'] is None: # Only allow obfuscation if no password defined
+                encryptcontent['obfuscate'] = True
+                encryptcontent['password'] = str(page.meta.get('obfuscate'))
+            del page.meta['obfuscate']
+
+        if encryptcontent.get('password'):
+            # Custom per-page strings
+            if 'encryption_summary' in page.meta.keys():
+                encryptcontent['summary'] = str(page.meta.get('encryption_summary'))
+                del page.meta['encryption_summary']
+
+            if 'encryption_info_message' in page.meta.keys():
+                encryptcontent['encryption_info_message'] = str(page.meta.get('encryption_info_message'))
+                del page.meta['encryption_info_message']
+
+            setattr(page, 'encryptcontent', encryptcontent)
+
         return markdown
 
     def on_page_content(self, html, page, config, **kwargs):
         """
         The page_content event is called after the Markdown text is rendered to HTML (but before
         being passed to a template) and can be used to alter the HTML body of the page. Generate
         encrypt content with AES and add form to decrypt this content with JS. Keep the generated
@@ -330,25 +450,24 @@
 
         :param html: HTML rendered from Markdown source as string
         :param page: mkdocs.nav.Page instance
         :param config: global configuration object
         :param site_navigation: global navigation object
         :return: HTML rendered from Markdown source as string encrypt with AES
         """
-        if self.config['password'] is not None:
-            if self.config['title_prefix']:
-                page.title = str(self.config['title_prefix']) + str(page.title)
+
+        if hasattr(page, 'encryptcontent'):
             if self.config['tag_encrypted_page']:
                 # Set attribute on page to identify encrypted page on template rendering
                 setattr(page, 'encrypted', True)
-            # Set password attributes on page for other mkdocs events
-            setattr(page, 'password', str(self.config['password']))
+
             # Keep encrypted html to encrypt as temporary variable on page
             if not self.config['inject']:
-                setattr(page, 'html_to_encrypt', html)
+                page.encryptcontent['html_to_encrypt'] = html
+
         return html
 
     def on_page_context(self, context, page, config, **kwargs):
         """
         The page_context event is called after the context for a page is created and
         can be used to alter the context for that specific page only.
         Replace clear HTML content with encrypted content and remove temporary attribute.
@@ -356,46 +475,68 @@
 
         :param context: dict of template context variables
         :param page: mkdocs.nav.Page instance
         :param config: global configuration object
         :param nav: global navigation object
         :return: dict of template context variables
         """
-        if hasattr(page, 'html_to_encrypt') or self.config['inject']:
+        if hasattr(page, 'encryptcontent'):
             if 'i18n_page_file_locale' in context:
                 locale = context['i18n_page_file_locale']
                 if locale in self.config['translations']:
                     translations = self.config['translations'][locale]
-                    if 'title_prefix' in translations:
-                        self.config['title_prefix'] = translations['title_prefix']
-                    if 'summary' in translations:
-                        self.config['summary'] = translations['summary']
-                    if 'placeholder' in translations:
-                        self.config['placeholder'] = translations['placeholder']
-                    if 'password_button_text' in translations:
-                        self.config['password_button_text'] = translations['password_button_text']
-                    if 'decryption_failure_message' in translations:
-                        self.config['decryption_failure_message'] = translations['decryption_failure_message']
-                    if 'encryption_info_message' in translations:
-                        self.config['encryption_info_message'] = translations['encryption_info_message']
-        if hasattr(page, 'html_to_encrypt'):
-            page.content = self.__encrypt_content__(
-                page.html_to_encrypt, 
-                str(page.password),
-                context['base_url']+'/',
-                self.config['site_path']+page.url
-            )
-            delattr(page, 'html_to_encrypt')
-        if self.config['inject']:
-            setattr(page, 'decrypt_form', self.__encrypt_content__(
-                '<!-- dummy -->', 
-                str(page.password),
-                context['base_url']+'/',
-                self.config['site_path']+page.url
-            ))
+
+                    #apply translation if defined
+                    if 'title_prefix' in translations and 'title_prefix' not in page.encryptcontent:
+                        page.encryptcontent['title_prefix'] = translations['title_prefix']
+                    if 'summary' in translations and 'summary' not in page.encryptcontent:
+                        page.encryptcontent['summary'] = translations['summary']
+                    if 'placeholder' in translations and 'placeholder' not in page.encryptcontent:
+                        page.encryptcontent['placeholder'] = translations['placeholder']
+                    if 'password_button_text' in translations and 'password_button_text' not in page.encryptcontent:
+                        page.encryptcontent['password_button_text'] = translations['password_button_text']
+                    if 'decryption_failure_message' in translations and 'decryption_failure_message' not in page.encryptcontent:
+                        page.encryptcontent['decryption_failure_message'] = translations['decryption_failure_message']
+                    if 'encryption_info_message' in translations and 'encryption_info_message' not in page.encryptcontent:
+                        page.encryptcontent['encryption_info_message'] = translations['encryption_info_message']
+
+            #init default strings from config
+            if 'title_prefix' not in page.encryptcontent:
+                page.encryptcontent['title_prefix'] = self.config['title_prefix']
+            if 'summary' not in page.encryptcontent:
+                page.encryptcontent['summary'] = self.config['summary']
+            if 'placeholder' not in page.encryptcontent:
+                page.encryptcontent['placeholder'] = self.config['placeholder']
+            if 'password_button_text' not in page.encryptcontent:
+                page.encryptcontent['password_button_text'] = self.config['password_button_text']
+            if 'decryption_failure_message' not in page.encryptcontent:
+                page.encryptcontent['decryption_failure_message'] = self.config['decryption_failure_message']
+            if 'encryption_info_message' not in page.encryptcontent:
+                page.encryptcontent['encryption_info_message'] = self.config['encryption_info_message']
+
+            if page.encryptcontent['title_prefix']: 
+                page.title = str(self.config['title_prefix']) + str(page.title)
+
+            if 'html_to_encrypt' in page.encryptcontent:
+                page.content = self.__encrypt_content__(
+                    page.encryptcontent['html_to_encrypt'], 
+                    context['base_url']+'/',
+                    self.setup['site_path']+page.url,
+                    page.encryptcontent
+                )
+                page.encryptcontent['html_to_encrypt'] = None
+
+            if self.config['inject']:
+                page.encryptcontent['decrypt_form'] = self.__encrypt_content__(
+                    '<!-- dummy -->', 
+                    context['base_url']+'/',
+                    self.setup['site_path']+page.url,
+                    page.encryptcontent
+                )
+
         return context
 
     def on_post_page(self, output_content, page, config, **kwargs):
         """
         The post_page event is called after the template is rendered, but before it is written to
         disc and can be used to alter the output of the page. If an empty string is returned, the
         page is skipped and nothing is written to disc. Finds other parts of HTML that need to be
@@ -403,18 +544,18 @@
 
         :param output_content: output of rendered template as string
         :param page: mkdocs.nav.Page instance
         :param config: global configuration object
         :return: output of rendered template as string
         """
         # Limit this process only if encrypted_something feature is enable *(speedup)*
-        if (self.config['encrypted_something'] and hasattr(page, 'encrypted')
-                and len(self.config['encrypted_something']) > 0):  # noqa: W503
+        if (self.setup['encrypted_something'] and hasattr(page, 'encryptcontent')
+                and len(self.setup['encrypted_something']) > 0):  # noqa: W503
             soup = BeautifulSoup(output_content, 'html.parser')
-            for name, tag in self.config['encrypted_something'].items():
+            for name, tag in self.setup['encrypted_something'].items():
                 # logger.debug({'name': name, 'html tag': tag[0], 'type': tag[1]})
                 something_search = soup.findAll(tag[0], {tag[1]: name})
                 if something_search is not None and len(something_search) > 0:
                     # Loop for multi child tags on target element
                     for item in something_search:
                         # Remove '\n', ' ' useless content generated by bs4 parsing...
                         item.contents = [
@@ -424,91 +565,110 @@
                         if len(item.contents) > 1:
                             merge_item = ''.join([str(s) for s in item.contents])
                         elif len(item.contents) == 1:
                             merge_item = item.contents[0]
                         else:
                             merge_item = ""
                         # Encrypt child items on target tags with page password
-                        cipher_bundle = self.__encrypt_text_aes__(merge_item, str(page.password))
+                        cipher_bundle = self.__encrypt_text_aes__(merge_item, str(page.encryptcontent['password']))
                         encrypted_content = b';'.join(cipher_bundle).decode('ascii')
                         # Replace initial content with encrypted one
-                        bs4_encrypted_content = BeautifulSoup(encrypted_content, 'html.parser')
-                        item.contents = [bs4_encrypted_content]
+                        item.string = encrypted_content
                         if item.has_attr('style'):
                             if isinstance(item['style'], list):
                                 item['style'].append("display:none")
                             else:
                                 # if style contains a single element (str)
                                 item['style'] = item['style'] + "display:none"
                         else:
                             item['style'] = "display:none"
+
             if self.config['inject'] and len(self.config['inject']) == 1:
                 name, tag = list(self.config['inject'].items())[0]
                 injector = soup.new_tag("div")
                 something_search = soup.find(tag[0], {tag[1]: name})
                 something_search.insert_before(injector)
-                injector.append(BeautifulSoup(page.decrypt_form, 'html.parser'))
-                delattr(page, 'decrypt_form')
+                injector.append(BeautifulSoup(page.encryptcontent['decrypt_form'], 'html.parser'))
+                page.encryptcontent['decrypt_form'] = None
+
             output_content = str(soup)
 
-        #TODO: Move search index processing to on_post_build to be less likely to fail due to incompatible search plugins
-        if hasattr(page, 'encrypted'):
-            #encrypt or exclude encrypted pages from search_index.json
-            for plugin in config['plugins']:
-                if plugin.endswith('search'):
-                    try:
-                        if hasattr(config['plugins'][plugin].search_index, '_entries'):
-                            search_entries = config['plugins'][plugin].search_index._entries
-                        elif hasattr(config['plugins'][plugin].search_index, 'entries'):
-                            search_entries = config['plugins'][plugin].search_index.entries
-                        else:
-                            logger.error('The search plugin "' + plugin + '" is currently unknown!')
+        if hasattr(page, 'encryptcontent'):
+            location = page.url.lstrip('/')
+            self.setup['locations'][location] = [page.encryptcontent['password'], page.encryptcontent.get('obfuscate')]
+            delattr(page, 'encryptcontent')
 
-                        for entry in search_entries.copy(): #iterate through all entries of search_index
-                            location = page.url.lstrip('/')
-                            if entry['location'] == location or entry['location'].startswith(location+"#"): #find the ones located at encrypted pages
-                                if self.config['search_index'] == 'encrypted':
-                                    search_entries.remove(entry)
-                                elif self.config['search_index'] == 'dynamically' and page.password is not None:
-                                    #encrypt text/title/location(anchor only)
-                                    text = entry['text']
-                                    title = entry['title']
-                                    toc_anchor = entry['location'].replace(location, '')
-                                    code = self.__encrypt_text_aes__(text, page.password)
-                                    entry['text'] = b';'.join(code).decode('ascii')
-                                    code = self.__encrypt_text_aes__(title, page.password)
-                                    entry['title'] = b';'.join(code).decode('ascii')
-                                    code = self.__encrypt_text_aes__(toc_anchor, page.password)
-                                    entry['location'] = location + ';' + b';'.join(code).decode('ascii')
-
-                        if hasattr(config['plugins'][plugin].search_index, '_entries'):
-                            config['plugins'][plugin].search_index._entries = search_entries
-                        elif hasattr(config['plugins'][plugin].search_index, 'entries'):
-                            config['plugins'][plugin].search_index.entries = search_entries
-
-                    except:
-                        logger.error('Could not encrypt search index of "' + page.title + '" for "' + plugin+ '" plugin! Abort !')
-                        os._exit(1)                                 # prevent build with possible plaintext in search_index
         return output_content
 
     def on_post_build(self, config, **kwargs):
         """
         The post_build event does not alter any variables.
         Use this event to call post-build scripts.
 
         :param config: global configuration object
         """
         Path(config.data["site_dir"] + '/assets/javascripts/').mkdir(parents=True, exist_ok=True)
         decrypt_js_path = Path(config.data["site_dir"] + '/assets/javascripts/decrypt-contents.js')
         with open(decrypt_js_path, "w") as file:
             file.write(self.__generate_decrypt_js__())
 
+        #modify search_index in the style of mkdocs-exclude-search
+        if self.setup['search_plugin_found'] and self.config['search_index'] != 'clear':
+            search_index_filename = Path(config.data["site_dir"] + "/search/search_index.json")
+            #TODO: Check if search_index.json exists and error if not found (moved its location)
+            with open(search_index_filename, "r") as f:
+                search_entries = json.load(f)
+
+            for entry in search_entries['docs'].copy(): #iterate through all entries of search_index
+                for location in self.setup['locations'].keys():
+                    if entry['location'] == location or entry['location'].startswith(location+"#"): #find the ones located at encrypted pages
+                        page_password = self.setup['locations'][location][0]
+                        if self.config['search_index'] == 'encrypted':
+                            search_entries.remove(entry)
+                        elif self.config['search_index'] == 'dynamically' and page_password is not None:
+                            #encrypt text/title/location(anchor only)
+                            text = entry['text']
+                            title = entry['title']
+                            toc_anchor = entry['location'].replace(location, '')
+                            code = self.__encrypt_text_aes__(text, page_password )
+                            entry['text'] = b';'.join(code).decode('ascii')
+                            code = self.__encrypt_text_aes__(title, page_password)
+                            entry['title'] = b';'.join(code).decode('ascii')
+                            code = self.__encrypt_text_aes__(toc_anchor, page_password)
+                            entry['location'] = location + ';' + b';'.join(code).decode('ascii')
+                        break
+
+            with open(search_index_filename, "w") as f:
+                json.dump(search_entries, f)
+            logger.info('Modified search_index.')
+
         # optionally download cryptojs
-        if self.config["selfhost"] and self.config["selfhost_download"]:
-            logger.info('Downloading cryptojs for self-hosting... Please consider copying "assets/javascripts/cryptojs/" to "doc/" and setting "selfhost_download: false" to decrease build time.')
-            Path(config.data["site_dir"] + '/assets/javascripts/cryptojs/').mkdir(parents=True, exist_ok=True)
+        if self.config['selfhost'] and self.config['selfhost_download']:
+            logger.info('Downloading cryptojs for self-hosting (if needed)...')
+            if self.config['selfhost_dir']:
+                configpath = Path(config['config_file_path']).parents[0]
+                dlpath = configpath.joinpath(self.config['selfhost_dir'] + '/assets/javascripts/cryptojs/')
+            else:
+                dlpath = Path(config.data['docs_dir'] + '/assets/javascripts/cryptojs/')
+            dlpath.mkdir(parents=True, exist_ok=True)
             for jsurl in JS_LIBRARIES:
-                dlurl = "https:" + jsurl
-                filepath = Path(config.data["site_dir"] + '/assets/javascripts/cryptojs/' + jsurl.rsplit('/',1)[1])
-                with urlopen(dlurl) as response:
-                    with open(filepath, 'wb') as file:
-                        file.write(response.read())
+                dlurl = "https:" + jsurl[0]
+                filepath = dlpath.joinpath(jsurl[0].rsplit('/',1)[1])
+                self.__download_and_check__(filepath, dlurl, jsurl[1])
+
+        passwords = set() #get all unique passwords
+        for location in self.setup['locations'].keys():
+            if not self.setup['locations'][location][1]:
+                passwords.add(self.setup['locations'][location][0])
+        self.setup['locations'].clear()
+        min_enttropy_spied_on, min_enttropy_secret = 0, 0
+        for password in passwords:
+            enttropy_spied_on, enttropy_secret = self.__get_entropy_from_password__(password)
+            if min_enttropy_spied_on == 0 or enttropy_spied_on < min_enttropy_spied_on:
+                min_enttropy_spied_on = enttropy_spied_on
+            if min_enttropy_secret == 0 or enttropy_secret < min_enttropy_secret:
+                min_enttropy_secret = enttropy_secret
+        if min_enttropy_spied_on < 100 and min_enttropy_spied_on > 0:
+            logger.warning('mkdocs-encryptcontent-plugin will always be vulnerable to brute-force attacks!'
+                           ' Your weakest password only got {spied_on} bits of entropy, if someone watched you while typing'
+                           ' (and a maximum of {secret} bits total)!'.format(spied_on = math.ceil(enttropy_spied_on), secret = math.ceil(min_enttropy_secret))
+                    )
```

### Comparing `mkdocs-encryptcontent-plugin-2.4.5/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO` & `mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-encryptcontent-plugin
-Version: 2.4.5
+Version: 2.5.0
 Summary: A MkDocs plugin that encrypt/decrypt markdown content with AES
 Home-page: https://github.com/unverbuggt/mkdocs-encryptcontent-plugin
 Author: unverbuggt
 Author-email: unverbuggt@xn--rthlein-n2a.de
 License: MIT
 Description: # mkdocs-encryptcontent-plugin
         
@@ -28,37 +28,43 @@
         >
         > If a password is defined in an article or a page, it is always used even if there is a global password.
         >
         > If a password is defined as an empty character string, the content is not protected.
         
         ![encryptcontent_demo](https://user-images.githubusercontent.com/12155947/177001700-f0920d4b-0c41-4d11-8164-9f63d29d8a6a.gif)
         
+        # Todo for 2.6.x
+        
+        * Rework password handling or inventory of some sort
+        * ...to be defined
         
         # Table of Contents
         
           * [Installation](#installation)
           * [Usage](#usage)
             * [Global password protection](#global-password-protection)
-            * [Secret from environment](#secret-from-environment) **(UPDATE)**
+            * [Secret from environment](#secret-from-environment)
             * [Customization](#default-vars-customization)
+            * [Translations](#translations)
+            * [Obfuscate pages](#obfuscate-pages) **NEW**
           * [Features](#features)
             * [HighlightJS support](#highlightjs-support) *(default)*
             * [Arithmatex support](#arithmatex-support) *(default)*
             * [Mermaid2 support](#mermaid-support) *(default)*
             * [Tag encrypted page](#tag-encrypted-page) *(default)*
             * [Remember password](#remember-password)
             * [Encrypt something](#encrypt-something)
-            * [Inject decrypt-form.tpl to theme](#inject-decrypt-formtpl-to-theme) **(NEW)**
+            * [Inject decrypt-form.tpl to theme](#inject-decrypt-formtpl-to-theme)
             * [Search index encryption](#search-index-encryption)
-            * [Search index encryption for mkdocs-material](#search-index-encryption-for-mkdocs-material) **(NEW)**
+            * [Search index encryption for mkdocs-material](#search-index-encryption-for-mkdocs-material)
             * [Override default templates](#override-default-templates)
             * [Add button](#add-button)
             * [Reload scripts](#reload-scripts)
-            * [Self-host crypto-js](#self-host-crypto-js) **(NEW)**
-            * [Translations](#translations) **(NEW)**
+            * [Self-host crypto-js](#self-host-crypto-js) *UPDATE*
+            * [File name obfuscation](#file-name-obfuscation) **NEW**
           * [Contributing](#contributing)
         
         
         # Installation
         
         Install the package with pip:
         
@@ -67,15 +73,15 @@
         ```
         
         Install the package from source with pip:
         
         ```bash
         cd mkdocs-encryptcontent-plugin/
         python setup.py sdist bdist_wheel
-        pip install dist/mkdocs_encryptcontent_plugin-2.4.5-py3-none-any.whl
+        pip install --force-reinstall --no-deps dist/mkdocs_encryptcontent_plugin-2.5.0-py3-none-any.whl
         ```
         
         Enable the plugin in your `mkdocs.yml`:
         
         ```yaml
         plugins:
             - search: {}
@@ -97,15 +103,16 @@
         plugins:
             - encryptcontent:
                 global_password: 'your_password'
         ```
         
         If a password is defined in an article, it will **ALWAYS** overwrite the global password. 
         
-        > **NOTE** Keep in mind that if the `password:` tag exists without value in an article, it will **not be protected** !
+        > **NOTE** Keep in mind that if the `password:` tag exists without value in a page, it will **not be protected** !
+        > Use this to **disable** `global_password` on specific pages.
         
         
         ### Secret from environment
         
         Instead of specifying a password in the mkdocs.yml file, you can use an environment variable to load your secret. 
         
         This process is in two steps:
@@ -122,28 +129,28 @@
         
         > **NOTE** Keep in mind that if the `use_secret:` configuration is set, it will always be used even if you have also set a global password with the `global_password` variable.
         >
         > If this environment variable is empty or missing, then the build will fail to prevent the unwanted leak of information.
         > However this can be converted into a warning by setting `ignore_missing_secret: true`. 
         > Use this only if you use a secret environment variable for production and a plain password for testing. You have been warned.
         
-        > **NEW** The meta tag `use_secret` can also be set to achieve the same functionality on page level.
+        > The meta tag `use_secret` can also be set to achieve the same functionality on page level.
         
         ### Default vars customization
         
         Optionally you can use some extra variables in plugin configuration to customize default messages.
         
         ```yaml
         plugins:
             - encryptcontent:
                 title_prefix: '[LOCK]'
                 summary: 'another informational message to encrypted content'
                 placeholder: 'another password placeholder'
-                decryption_failure_message: 'another informational message when decryption fail'
-                encryption_info_message: 'another information message when you dont have acess !'
+                decryption_failure_message: 'another informational message when decryption fails'
+                encryption_info_message: "another information message when you don't have access !"
                 input_class: 'md-search__form md-search__input'
                 button_class: 'md-search__icon'
         ```
         
         Default prefix title is `[Protected]`.
         
         Default summary message is `This content is protected with AES encryption.`.
@@ -152,15 +159,46 @@
         
         Default decryption failure message is `Invalid password.`.
         
         Defaut encryption information message is `Contact your administrator for access to this page.`.
         
         > **NOTE** Adding a prefix to the title does not change the default navigation path !
         
-        Use `input_class` and `button_class` to optionally set a CSS class for the password field and the button.
+        ### Translations
+        
+        If the plugin is used in conjunction with the [static-i18n](https://ultrabug.github.io/mkdocs-static-i18n/) plugin you can provide `translations` for the used `i18n_page_file_locale`.
+        
+        ```yaml
+            - encryptcontent:
+                #...
+                translations:
+                  de:
+                    title_prefix: '[Verschlüsselt] '
+                    summary: 'Der Inhalt dieser Seite ist mit AES verschlüsselt. '
+                    placeholder: 'Mit Strg+Enter wird das Passwort global gesetzt'
+                    password_button_text: 'Entschlüsseln'
+                    decryption_failure_message: 'Falsches passwort.'
+                    encryption_info_message: 'Bitte wenden Sie sich an den Systemadministrator um auf diese Seite zuzugreifen.'
+        ```
+        
+        #### Custom per-page strings
+        
+        You can set the  meta tag `encryption_summary` to customize `summary` and `encryption_info_message` on every page.
+        
+        ### Obfuscate pages
+        
+        If you want to make it harder for search engines to scrape you pages content,
+        you can set `obfuscate: SomeNotSoSecretPassword` meta tag in markdown.
+        
+        The page than will display `summary` and `encryption_info_message` together with a button labeled with.
+        `password_button_text`. In order to view the pages content one hast to press the button first.
+        
+        If a `password` or `use_secret` is set, then the `obfuscate` feature will be disabled.
+        If you want to use `obfuscate` in a configuration where `global_password` is defined, 
+        you'll need to set `password:` meta tag (with no password defined) to undefine the password on this page.
         
         # Features
         
         ### HighlightJS support
         
         > **Enable by default**
         
@@ -216,16 +254,15 @@
         
         > **Enable by default**
         
         Related to [issue #7](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin/issues/7)
         
         This feature add an additional attribute `encrypted` with value `True` to the mkdocs type `mkdocs.nav.page` object.
         
-        You can add `tag_encrypted_page: False` in plugin configuration, to disable tagging of encrypted pages. **BUT** This feature is neccessary for others feature working correctly. 
-        If you disable this feature, f.ex. [Encrypt something](#encrypt-something) and [Search index encryption](#search-index-encryption) won't work.
+        You can add `tag_encrypted_page: False` in plugin configuration, to disable tagging of encrypted pages. 
         
         When enable, it becomes possible to use `encrypted` attribute in the jinja template of your theme, as a condition to perform custom modification.
         
         ```jinja
         {%- for nav_item in nav %}
             {% if nav_item.encrypted %}
                 <!-- Do something --> 
@@ -253,37 +290,39 @@
         When enabled, each time you fill password form and press `Enter` a key on session storage is create with your password
         as value. When you reload the page, if you already have an 'encryptcontent' key in the session storage of your browser,
         the page will be automatically decrypted using the value previously created.
         
         By default, the key is created with a name relative to the page on which it was generated.
         This 'relative' key will always be used as first attempt to decrypt the current page when loading.
         
-        If your password is a [global password](#global-password-protection), you can fill in the form field  `mkdocs-content-password`, then use the keyboard shortcut `CTRL + ENTER` instead of the classic `ENTER`. 
+        If your password is a [global password](#global-password-protection), you can fill in the form
+        field  `mkdocs-content-password`, then use the keyboard shortcut `CTRL + ENTER` instead of the classic `ENTER`. 
         The key that will be created with a generic name to making it accessible, by default, on all the pages of your site.
         
         The form of decryption remains visible as long as the content has not been successfully decrypted, which allows in case of error to retry. 
         All keys created with this feature on sessionStorage/localStorage have an default expire time daly set to 24 hours, just cause ...
         
         However *(optionally)*, its possible to change the default expire time by setting options `default_expire_delay: <number>` in your `mkdocs.yml`. Your configuration should look like this when you enabled this feature :
         ```yaml
         plugins:
             - encryptcontent:
                 remember_password: True
                 default_expire_delay: 24   # <-- Default expire delay in hours (optional)
         ```
         
-        > **NOTE** The expired elements of the localStorage are only deleted by the execution of the decrypt-content.js scripts and therefore by the navigation on the site. Secret items can therefore remain visible in local storage after their expiration dates. 
-        > Now The default is to use sessionStorage instead of localStorage, so the browser forgets the password after the current tab was closed. However it can be set to use localStorage by setting `session_storage: False`
+        > **NOTE** The expired elements of the localStorage are only deleted by the execution of the decrypt-content.js
+        > scripts and therefore by the navigation on the site. Secret items can therefore remain visible in local storage
+        > after their expiration dates. 
+        > Now The default is to use sessionStorage instead of localStorage, so the browser forgets the password after
+        > the current tab was closed. However it can be set to use localStorage by setting `session_storage: False`
         
         ### Encrypt something
         
         Related to [issue #9](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin/issues/9)
         
-        The [tag encrypted page feature](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin#tag-encrypted-page) **MUST** be enabled (it's default) for this feature to work properly.
-        
         Add `encrypted_something: {}` in the plugin configuration variable, to encrypt something else.
         
         The syntax of this new variable **MUST** follow the yaml format of a dictionary. 
         Child elements of `encrypted_something` are build with a key `<unique name>` in string format and a list as value. 
         The list have to be contructed with the name of an HTML element `<html tag>` as first item and `id` or `class` as the second item.
         
         ```yaml
@@ -327,15 +366,15 @@
         ```yaml
         plugins:
             - encryptcontent:
                 encrypted_something:
                     mkdocs-encrypted-toc: [div, id]
         ```
         
-        2. Other example, with multiples target. In you Material Theme, you want to encrypt ToC content and Footer.
+        2. Other example, with multiples target. In your custom Material theme, you want to encrypt ToC content and Footer.
         
         Materiel generate 2 `<nav>` structure with the same template `toc.html`, so you need to use a `class` instead of an id for this part.
         The footer part, is generated by the `footer.html` template in a classic div so an `id` is sufficient
         
         After modification, your template looks like this :
         ```jinja (toc.html)
         <nav class="md-nav md-nav--secondary {% if page.encrypted %}mkdocs-encrypted-toc{% endif %}" aria-label="{{ lang.t('toc.title') }}">
@@ -346,25 +385,26 @@
         ```jinja (footer.html)
         <footer class="md-footer">
             <div class="md-footer-nav" {% if page.encrypted %}id="mkdocs-encrypted-footer"{% endif %}> ... </div>
             <div class="md-footer-meta md-typeset" {% if page.encrypted %}id="mkdocs-encrypted-footer-meta"{% endif %}>
         </footer>
         ```
         
-        Your configuration like this :
+        Your configuration would look like this :
         ```yaml
         plugins:
             - encryptcontent:
                 encrypted_something:
                     mkdocs-encrypted-toc: [nav, class]
                     mkdocs-encrypted-footer: [div, id]
                     mkdocs-encrypted-footer-meta: [div, id]
         ```
         
-        3. If you are using mkdocs-material, then this example will also encrypt menu, toc and footer
+        3. If you are using unmodified mkdocs-material, then this example will encrypt menu, toc and footer
+        But you'd need the Navigation pruning feature to hide the title of encrypted pages from navigation (or see 2.).
         
         ```yaml
         plugins:
             - encryptcontent:
                 encrypted_something:
                     md-footer__inner: [nav, class]
                     md-nav: [nav, class]
@@ -391,14 +431,16 @@
                 encrypted_something:
                     md-footer__inner: [nav, class] #Footer
                     md-nav: [nav, class] #Menu and toc
                 inject:
                     md-content: [div, class]
         ```
         
+        > This feature overrides the normal practice of replacing the rendered content of a page.
+        
         ### Search index encryption
         
         > **Default value is "encrypted"**
         
         Related to [issue #13](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin/issues/13)
         
         > :warning: **The configuration mode "clear" of this functionality can cause DATA LEAK**
@@ -408,41 +450,47 @@
         > You have been warned 
         
         This feature allows you to control the behavior of the encryption plugin with the search index. 
         Three configuration modes are possible:
         
          * **clear** : Search index is not encrypted. Search is possible even on protected pages.
          * **dynamically** : Search index is encrypted on build. Search is possible once the pages have been decrypted.
-         * **encrypted** : Search index of encrypted pages is removed on build. Search is not possible on all encrypted pages.
+         * **encrypted** : Search index of encrypted pages is removed on build. Search is not possible on encrypted pages.
         
         You can set `search_index: '<mode_name>'` in your `mkdocs.yml` to change the search index encryption mode. Possible values are `clear`, `dynamically`, `encrypted`. The default mode is "**encrypted**".
         
         ```yaml
         plugins:
             - encryptcontent:
                 search_index: 'dynamically'
         ```
         
         This functionality modifies the search index created by the “search” plug-in.
-        Some themes might override the default “search” plug-in provided by mkdocs, but so far the structure of the `search/search_index.json` file is consistent.
+        Some themes might override the default search plug-in provided by mkdocs, 
+        but so far the structure of the `search/search_index.json` file is consistent.
         
         > The modification of the search index is carried out last (if `encryptcontent` is also last in `plugins`).
         > But always double-check the generated index after `mkdocs build` to see if your information is protected.
         
-        When the configuration mode is set to "**dynamically**", the [javascripts contribution files](https://github.com/unverbuggt/mkdocs-encryptcontent-plugin/tree/master/encryptcontent/contrib/templates/search)
-        are used to override the default search plugin files provided by MkDocs. They include a process of decrypting and keeping the search index in a SessionStorage.
+        When the configuration mode is set to "**dynamically**", the 
+        [javascripts contribution files](https://github.com/unverbuggt/mkdocs-encryptcontent-plugin/tree/master/encryptcontent/contrib/templates/search)
+        are used to override the default search plugin files provided by MkDocs. 
+        They include a process of decrypting and keeping the search index in a SessionStorage.
         
         ### Search index encryption for mkdocs-material
         
-        [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) uses a different search plugin that cannot "easily" be overridden like the default search plugin.
-        However this Plugin will still remove encrypted pages (`encrypted`) or encrypt the search entries (`dynamically`) for `mkdocs-material`.
+        [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) uses a different search plugin that
+        cannot "easily" be overridden like the default search plugin.
+        However this Plugin will still remove encrypted pages (`encrypted`) or encrypt the search entries (`dynamically`)
+        for `mkdocs-material`.
         
         In order to be able to decrypt the search index (`dynamically`) `mkdocs-material` needs to be customized (patched).
         
-        You'll need some [prerequisites](https://squidfunk.github.io/mkdocs-material/customization/#environment-setup) and also execute these commands:
+        You'll need some [prerequisites](https://squidfunk.github.io/mkdocs-material/customization/#environment-setup)
+        and also execute these commands:
         
         ```bash
         git clone https://github.com/squidfunk/mkdocs-material
         cd mkdocs-material
         pip install mkdocs-minify-plugin
         pip install mkdocs-redirects
         npm install
@@ -456,24 +504,33 @@
         
         > Note: this currently doesn't work with mkdocs-material-9.x.x
         
         ### Override default templates
         
         Related to [issue #32](https://github.com/CoinK0in/mkdocs-encryptcontent-plugin/issues/32)
         
-        You can override the default templates with your own templates by providing an actual replacement path in the `html_template_path` *(HTML)* and `js_template_path` *(JS)* directives. Overridden templates **completely** replace the default templates. You **must** therefore copy the default templates to keep this module working.
+        You can override the default templates with your own templates by providing an actual replacement
+        path in the `html_template_path` *(HTML)* and `js_template_path` *(JS)* directives. 
+        Overridden templates **completely** replace the default templates. You **must** therefore copy the
+        default templates to keep this module working.
         
         ```yaml
         plugins:
             - encryptcontent:
                 html_template_path: "/root/real/path/mkdocs_poc/my_html_template.html"
                 js_template_path: "/root/real/path/mkdocs_poc/my_js_template.js"
+                input_class: 'md-search__form md-search__input'
+                button_class: 'md-search__icon'
         ```
         
-        When you overriding the default templates, you can add and use your own Jinja variables to condition and enrich your template, by defining `html_extra_vars` and `js_extra_vars` directives in key/value format. Added values can be used in your Jinja templates via the variable `extra`.
+        Use `input_class` and `button_class` to optionally set a CSS class for the password input field and the button.
+        
+        When you overriding the default templates, you can add and use your own Jinja variables to condition
+        and enrich your template, by defining `html_extra_vars` and `js_extra_vars` directives in key/value format.
+        Added values can be used in your Jinja templates via the variable `extra`.
         
         ```yaml
         plugins:
             - encryptcontent:
                 html_extra_vars:
                     my_extra: "extra value"
                     <key>: <value>
@@ -486,15 +543,17 @@
         
         ```jinja
         [ ... ] 
         <h2>{{ extra.my_extra }}</h2>
         [ ... ]
         ```
         
-        > **NOTE** You must avoid replacing/overwriting the variables used by default by this module. The limitations are the same as those of the jinja models. Issues related to template override will not be addressed.
+        > **NOTE** You must avoid replacing/overwriting the variables used by default by this module.
+        > The limitations are the same as those of the jinja models.
+        > Issues related to template override will not be addressed.
         
         ### Add button
         
         Add `password_button: True` in plugin configuration variable, to add button to the right of the password field.
         
         When enable, it allows to decrypt the content just like the classic keypress ENTER. If remember password feature is activated, use button to decrypt generate a 'relative' key on your local storage. You cannot use password button to create global password value.
         
@@ -524,42 +583,71 @@
         This feature now doesn't use JQuery anymore.
         
         It is also possible to reload a script id like `<script id="autoexec">console.log('test');</script>` that was encrypted within the page (related to [issue #30](https://github.com/unverbuggt/mkdocs-encryptcontent-plugin/issues/30)).
         
         ### Self-host crypto-js
         
         If you enable `selfhost` then you'll choose to upload crypto-js to your web server rather than using cloudflare CDN.
+        The self-host location is "SITE_URL/assets/javascripts/cryptojs/".
         
-        Additionally if you set `selfhost_download` then the required files will be downloaded **every time** on `mkdocs serve` or `mkdocs build`. 
-        Be aware that this costs additional build time and it is better to copy the files from `site/assets/javascripts/cryptojs/*` to `docs/assets/javascripts/cryptojs/*` to speed things up.
+        Additionally if you set `selfhost_download` then the required files will be automatically downloaded if needed.
+        The files are checked for their MD5 hash and saved to `docs_dir` or `selfhost_dir` (relative to `mkdocs.yml`).
         
         ```yaml
         plugins:
             - encryptcontent:
                 selfhost: true
                 selfhost_download: false
+                selfhost_dir: 'theme_overrides'
         ```
         
-        ### Translations
+        ### File name obfuscation
         
-        If the plugin is used in conjunction with the [static-i18n](https://ultrabug.github.io/mkdocs-static-i18n/) plugin you can provide `translations` for the used `i18n_page_file_locale`.
+        Imagine your pages contain many images and you labeled them "1.jpg", "2.jpg" and so on for some reason.
+        If you'd like to encrypt one of these pages, an attacker could try guessing the image file names
+        and would be able to download them despite not having the password to the page.
+        
+        This feature should make it impossible or at least way harder for an external attacker to guess the file names.
+        Please also check and disable directory listing for that matter.
+        Keep in mind that you hosting provider is still able to see all your images and files.
+        
+        To counter file name guessing you could active the feature like this:
         
         ```yaml
+        plugins:
             - encryptcontent:
-                #...
-                translations:
-                  de:
-                    title_prefix: '[Verschlüsselt] '
-                    summary: 'Der Inhalt dieser Seite ist mit AES verschlüsselt. '
-                    placeholder: 'Mit Strg+Enter wird das Passwort global gesetzt'
-                    password_button_text: 'Entschlüsseln'
-                    decryption_failure_message: 'Falsches passwort.'
-                    encryption_info_message: 'Bitte wenden Sie sich an den Systemadministrator um auf diese Seite zuzugreifen.'
-        ```
+                selfhost: true
+                selfhost_download: false
+                hash_filenames:
+                  extensions:
+                    - 'png'
+                    - 'jpg'
+                    - 'jpeg'
+                    - 'svg'
+                  except:
+                    - 'lilien.svg'
+        ```
+        
+        At `extensions` we define which file name extensions to obfuscate
+        (extension is taken from the part after the last ".",
+        so the extension of "image.jpg" is "jpg" and of "archive.tar.gz" is "gz").
+        
+        You can define multiple exceptions at the `except` list.
+        The file names that end with these strings will be skipped.
+        You should use this if some images are used by themes or other plugins.
+        Otherwise, you'd need to change these file names to the obfuscated ones.
+        
+        The file names are obfuscated in a way that the corresponding file is hashed with MD5
+        and the hash is added to the file name
+        (If the file content is not changed the file name also not changes), like this:
+        
+        some_image_1_bb80db433751833b8f8b4ad23767c0fc.jpg
+        ("bb80db433751833b8f8b4ad23767c0fc" being the MD5 hash of said image.)
         
+        > The file name obfuscation is currently applied to the whole site - not just the encrypted pages...
         
         # Contributing
         
         From reporting a bug to submitting a pull request: every contribution is appreciated and welcome.
         
         Report bugs, ask questions and request features using [Github issues][github-issues].
```

### Comparing `mkdocs-encryptcontent-plugin-2.4.5/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt` & `mkdocs-encryptcontent-plugin-2.5.0/mkdocs_encryptcontent_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-encryptcontent-plugin-2.4.5/setup.py` & `mkdocs-encryptcontent-plugin-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     with open(file_path) as file:
         content = file.read()
     return content if content else 'no content read'
 
 
 setup(
     name='mkdocs-encryptcontent-plugin',
-    version='2.4.5',
+    version='2.5.0',
     author='unverbuggt',
     author_email='unverbuggt@xn--rthlein-n2a.de',
     description='A MkDocs plugin that encrypt/decrypt markdown content with AES',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown encrypt decrypt content',
     url='https://github.com/unverbuggt/mkdocs-encryptcontent-plugin',
```

